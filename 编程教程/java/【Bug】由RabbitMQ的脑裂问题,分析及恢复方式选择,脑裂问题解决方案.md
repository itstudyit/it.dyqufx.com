# 【Bug】由RabbitMQ的脑裂问题,分析及恢复方式选择,脑裂问题解决方案

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.bcwex.shop/posts?id=3873

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515185403/6644944b2b1b9.jpg" width="500" alt="">

           RabbitMQ脑裂错误日志          2020-03-11 11:55:16 =ERROR REPORT====

 Mnesia(rabbit@EZoMQ1): ** ERROR ** mnesia_event got 

 &nbsp;

 2020-03-11 11:55:15.046 [error] &lt;0.4723.25&gt; ** Node rabbit@EZoMQ3 not responding **

 ** Removing (timedout) connection **

 2020-03-11 11:55:15.047 [info] &lt;0.398.0&gt; rabbit on node rabbit@EZoMQ3 down

 2020-03-11 11:55:15.054 [info] &lt;0.398.0&gt; Node rabbit@EZoMQ3 is down, deleting its listeners

 2020-03-11 11:55:15.078 [info] &lt;0.398.0&gt; node rabbit@EZoMQ3 down: net_tick_timeout

 2020-03-11 11:55:15.079 [error] &lt;0.398.0&gt; Partial partition detected:

 * We saw DOWN from rabbit@EZoMQ3

 * We can still see rabbit@EZoMQ1 which can see rabbit@EZoMQ3

 We will therefore intentionally disconnect from rabbit@EZoMQ1

 【Bug】由RabbitMQ的脑裂问题,分析及恢复方式选择,脑裂问题解决方案



          什么是脑裂？          所谓的脑裂问题，就是在多机集群中节点与节点之间失联，都认为对方出现故障，而自身裂变为独立的个体，各自为政，那么就出现了抢夺对方的资源，争抢启动，至此就发生了事故。rabbitmq 脑裂问题，实质上是个网络分区问题，rabbitmq集群的网络分区容错性不好，在网络比较差的情况下容易出错，最明显的就是脑裂问题了。

 举个栗子：

 A和B是集群上的两个节点，分别拥有一部分集群的数据a,b， 如果这时发生分区问题，两个节点无法通信，A以为B宕机，B以为A宕机，于是就出现了：

 （1）如果A存在B的备份，那就以完整数据运行，B存在A的数据备份，也是同样， 那这里就造成共享数据损坏。

 （2）如果 A,B 各自仅拥有a,b 的数据，那要么都无法恢复/启动，要么就瓜分数据运行。

          出现脑裂的现象          在RabbitMQ的Web管理界面会看到如下信息提示：

    Network partition detected Mnesia reports that this RabbitMQ cluster has experienced a network partition. There is a risk of losing data. Please read RabbitMQ documentation about network partitions and the possible solutions.

  &nbsp;

             判断条件          默认情况下，一个节点在60s之内不能连接上另一个节点（可用net_ticktime 参数调整），就判定这个节点挂了。即使之后节点网络又连通了，由于节点都认为对方挂了，所以Mnesia 还是会发送网络分区的情况并且将情况记录在日志中。（许多围绕网络分区的细节都与Mnesia的行为相关。Mnesia是一个分布式数据库管理系统(DBMS),适合于电信和其它需要持续运行和具备软实时特性的Erlang应用，是构建电信应用的控制系统平台开放式电信平台(OTP)的一部分。）

 除了网络失败原因，操作系统的挂起和恢复也会导致集群内部节点发生分区， 因为发生挂起的节点不会认为自己已经失败或者不能工作，但是其他节点会这么认为。比如：将节点运行在你的电脑上，你合上电脑；或者你将节点运行在虚拟机里，系统管理程序将节点挂起了。

          恢复方式                1.人工方式       （1）部分重启。选择受信分区即网络环境好的分区，重启其他分区，让他们重新加入受信分区中，之后再重启受信分区，消除警告⚠️

 （2）全部重启。停掉整个集群，然后启动，不过要保证第一个启动的是受信分区。不然还没等所有节点加入，自己就挂了。

        2.自动处理 （1）ignore 默认配置，即分区不做任何处理。发生网络分区时，需要人工介入。要使用这种，就要保证网络高可用，例如，节点都在一个机架上，用的同一个交换机，这个交换机连上一个WAN，保证网络稳定。       （2）pause_minority，优先暂停‘少数派’。就是节点判断自己在不在‘少数派’（少于或者等于集群中一半的节点数），在就自动关闭，保证稳定区的大部分节点可以继续运行。一般情况下，可应用于非跨机架、奇数节点的集群中。

 （3）pause-if-all-down，对于受信节点的选择尤为考究，尤其是在集群中所有节点硬件配置相同的情况下。此种模式可以处理对等分区的情形。

 （4）autoheal， 关闭客户端连接数最多的节点。 这里比较有意思，rabbitmq 会自动挑选一个‘获胜’分区，即连接数最小的，重启其他分区。（如果平手，就选节点多的，如果节点也一致，那就以未知方式挑选‘获胜者’）。这个更关心服务的连续性而不是数据的完整性。但是如果集群中有节点处于非运行状态，则此种模式会失效。

 &nbsp;

 &nbsp;

  