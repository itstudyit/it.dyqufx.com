# Kafka核心源码解读  

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.dyqufx.com/posts?id=2188

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515183720/66449060aff65.jpg" width="500" alt="">

  从底层到实战，深度解析源码

 系统高效的源码阅读方法

 深入理解 Kafka 的底层原理

 快速定位线上问题并制定调优方案

 25 个典型案例分享 + 面试题讲解

 课程主体分为 7 个模块。

  日志模块：详细介绍消息是如何被定义和组织的，帮你掌握 Kafka 消息在底层被读写的方法代码是怎么实现的。 请求处理模块：分析各类 Kafka 请求在网络层传输以及被处理的逻辑代码，尤其是 Reactor 模式在 Kafka 中的实现。 副本管理模块：主要阐述分区副本对象的管理逻辑代码，包括副本的创建、状态流转、删除等操作，帮你搞懂副本在 Kafka 中的状态流转路径。 延迟操作模块：重点讲解 Kafka 如何实现延迟操作，以及一个 O(N) 时间复杂度的时间轮算法，带你搞懂延迟操作底层的实现架构。 消费者组管理模块：详细分析消费者组协调器的各类管理功能代码，比如创建、管理、删除等，GroupCoordinator 是 Kafka 中最核心的组件之一。 Controller 模块：结合一些实际案例，给你分享 Controller 组件管理 Kafka 集群元数据的代码和基于 ZooKeeper 的 Controller 选举。 状态机模块：重点分析副本和分区的状态流转逻辑，以及 Kafka 集群是如何管理副本对象和分区对象的。  除此之外，还设置了“特别放送”模块，与你分享一些经典的学习资料、参与开源社区的全部流程，解析经典的面试题等，全方位提升你的源码阅读能力和 Kafka 实战能力。

 〖课程截图〗:

  ├──jk50101-Kafka核心源码解读

 | ├──01丨课前必学 (3讲)

 | | ├──00丨导读丨构建Kafka工程和源码阅读环境、Scala语言热身.html 2.93M

 | | ├──00丨导读丨构建Kafka工程和源码阅读环境、Scala语言热身.m4a 10.23M

 | | ├──00丨导读丨构建Kafka工程和源码阅读环境、Scala语言热身.pdf 1.82M

 | | ├──00丨开篇词丨阅读源码，逐渐成了职业进阶道路上的“必选项”.html 4.82M

 | | ├──00丨开篇词丨阅读源码，逐渐成了职业进阶道路上的“必选项”.m4a 9.87M

 | | ├──00丨开篇词丨阅读源码，逐渐成了职业进阶道路上的“必选项”.pdf 6.22M

 | | ├──重磅加餐丨带你快速入门Scala语言.html 2.63M

 | | ├──重磅加餐丨带你快速入门Scala语言.m4a 10.53M

 | | └──重磅加餐丨带你快速入门Scala语言.pdf 1.41M

 | ├──02丨日志模块 (5讲)

 | | ├──01丨日志段：保存消息文件的对象是怎么实现的？.html 7.25M

 | | ├──01丨日志段：保存消息文件的对象是怎么实现的？.m4a 13.15M

 | | ├──01丨日志段：保存消息文件的对象是怎么实现的？.pdf 4.86M

 | | ├──02丨日志（上）：日志究竟是如何加载日志段的？.html 5.87M

 | | ├──02丨日志（上）：日志究竟是如何加载日志段的？.m4a 10.49M

 | | ├──02丨日志（上）：日志究竟是如何加载日志段的？.pdf 3.88M

 | | ├──03丨日志（下）：彻底搞懂Log对象的常见操作.html 7.12M

 | | ├──03丨日志（下）：彻底搞懂Log对象的常见操作.m4a 23.70M

 | | ├──03丨日志（下）：彻底搞懂Log对象的常见操作.pdf 4.55M

 | | ├──04丨索引（上）：改进的二分查找算法在Kafka索引的应用.html 6.41M

 | | ├──04丨索引（上）：改进的二分查找算法在Kafka索引的应用.m4a 17.55M

 | | ├──04丨索引（上）：改进的二分查找算法在Kafka索引的应用.pdf 4.24M

 | | ├──05丨索引（下）：位移索引和时间戳索引的区别是什么？.html 6.32M

 | | ├──05丨索引（下）：位移索引和时间戳索引的区别是什么？.m4a 10.36M

 | | └──05丨索引（下）：位移索引和时间戳索引的区别是什么？.pdf 4.07M

 | ├──03丨请求处理模块 (5讲)

 | | ├──06丨请求通道：如何实现Kafka请求队列？.html 4.52M

 | | ├──06丨请求通道：如何实现Kafka请求队列？.m4a 15.64M

 | | ├──06丨请求通道：如何实现Kafka请求队列？.pdf 3.35M

 | | ├──07丨SocketServer（上）：Kafka到底是怎么应用NIO实现网络通信的？.html 9.16M

 | | ├──07丨SocketServer（上）：Kafka到底是怎么应用NIO实现网络通信的？.m4a 16.27M

 | | ├──07丨SocketServer（上）：Kafka到底是怎么应用NIO实现网络通信的？.pdf 9.03M

 | | ├──08丨SocketServer（中）：请求还要区分优先级？.html 7.03M

 | | ├──08丨SocketServer（中）：请求还要区分优先级？.m4a 15.46M

 | | ├──08丨SocketServer（中）：请求还要区分优先级？.pdf 7.89M

 | | ├──09丨SocketServer（下）：请求处理全流程源码分析.html 5.90M

 | | ├──09丨SocketServer（下）：请求处理全流程源码分析.m4a 14.66M

 | | ├──09丨SocketServer（下）：请求处理全流程源码分析.pdf 4.15M

 | | ├──10丨KafkaApis：Kafka最重要的源码入口，没有之一.html 6.26M

 | | ├──10丨KafkaApis：Kafka最重要的源码入口，没有之一.m4a 12.38M

 | | └──10丨KafkaApis：Kafka最重要的源码入口，没有之一.pdf 5.19M

 | ├──04丨Controller模块 (5讲)

 | | ├──11丨Controller元数据：Controller都保存有哪些东西？有几种状态？.html 3.78M

 | | ├──11丨Controller元数据：Controller都保存有哪些东西？有几种状态？.m4a 13.71M

 | | ├──11丨Controller元数据：Controller都保存有哪些东西？有几种状态？.pdf 2.70M

 | | ├──12丨ControllerChannelManager：Controller如何管理请求发送？.html 4.76M

 | | ├──12丨ControllerChannelManager：Controller如何管理请求发送？.m4a 13.58M

 | | ├──12丨ControllerChannelManager：Controller如何管理请求发送？.pdf 3.31M

 | | ├──13丨ControllerEventManager：变身单线程后的Controller如何处理事件？.html 5.53M

 | | ├──13丨ControllerEventManager：变身单线程后的Controller如何处理事件？.m4a 13.17M

 | | ├──13丨ControllerEventManager：变身单线程后的Controller如何处理事件？.pdf 6.01M

 | | ├──14丨Controller选举是怎么实现的？.html 7.18M

 | | ├──14丨Controller选举是怎么实现的？.m4a 16.24M

 | | ├──14丨Controller选举是怎么实现的？.pdf 4.99M

 | | ├──15丨如何理解Controller在Kafka集群中的作用？.html 5.40M

 | | ├──15丨如何理解Controller在Kafka集群中的作用？.m4a 11.78M

 | | └──15丨如何理解Controller在Kafka集群中的作用？.pdf 3.55M

 | ├──05丨状态机模块 (3讲)

 | | ├──16丨TopicDeletionManager：Topic是怎么被删除的？.html 5.09M

 | | ├──16丨TopicDeletionManager：Topic是怎么被删除的？.m4a 14.42M

 | | ├──16丨TopicDeletionManager：Topic是怎么被删除的？.pdf 4.46M

 | | ├──17丨ReplicaStateMachine：揭秘副本状态机实现原理.html 7.90M

 | | ├──17丨ReplicaStateMachine：揭秘副本状态机实现原理.m4a 15.71M

 | | ├──17丨ReplicaStateMachine：揭秘副本状态机实现原理.pdf 6.76M

 | | ├──18丨PartitionStateMachine：揭秘分区状态机实现原理.html 4.99M

 | | ├──18丨PartitionStateMachine：揭秘分区状态机实现原理.m4a 16.52M

 | | └──18丨PartitionStateMachine：揭秘分区状态机实现原理.pdf 3.98M

 | ├──06丨延迟操作模块 (2讲)

 | | ├──19丨TimingWheel：探究Kafka定时器背后的高效时间轮算法.html 3.58M

 | | ├──19丨TimingWheel：探究Kafka定时器背后的高效时间轮算法.m4a 16.37M

 | | ├──19丨TimingWheel：探究Kafka定时器背后的高效时间轮算法.pdf 2.58M

 | | ├──20丨DelayedOperation：Broker是怎么延时处理请求的？.html 3.31M

 | | ├──20丨DelayedOperation：Broker是怎么延时处理请求的？.m4a 19.12M

 | | └──20丨DelayedOperation：Broker是怎么延时处理请求的？.pdf 2.29M

 | ├──07丨副本管理模块 (6讲)

 | | ├──21丨AbstractFetcherThread：拉取消息分几步？.html 2.67M

 | | ├──21丨AbstractFetcherThread：拉取消息分几步？.m4a 13.02M

 | | ├──21丨AbstractFetcherThread：拉取消息分几步？.pdf 1.88M

 | | ├──22丨ReplicaFetcherThread：Follower拉取Leader消息是如何实现的？.html 6.61M

 | | ├──22丨ReplicaFetcherThread：Follower拉取Leader消息是如何实现的？.m4a 13.34M

 | | ├──22丨ReplicaFetcherThread：Follower拉取Leader消息是如何实现的？.pdf 4.12M

 | | ├──23丨ReplicaManager（上）：必须要掌握的副本管理类定义和核心字段.html 4.09M

 | | ├──23丨ReplicaManager（上）：必须要掌握的副本管理类定义和核心字段.m4a 12.22M

 | | ├──23丨ReplicaManager（上）：必须要掌握的副本管理类定义和核心字段.pdf 2.94M

 | | ├──24丨ReplicaManager（中）：副本管理器是如何读写副本的？.html 4.47M

 | | ├──24丨ReplicaManager（中）：副本管理器是如何读写副本的？.m4a 13.03M

 | | ├──24丨ReplicaManager（中）：副本管理器是如何读写副本的？.pdf 3.24M

 | | ├──25丨ReplicaManager（下）：副本管理器是如何管理副本的.html 5.07M

 | | ├──25丨ReplicaManager（下）：副本管理器是如何管理副本的？.m4a 18.53M

 | | ├──25丨ReplicaManager（下）：副本管理器是如何管理副本的？.pdf 4.50M

 | | ├──26丨MetadataCache：Broker是怎么异步更新元数据缓存的？.html 4.73M

 | | ├──26丨MetadataCache：Broker是怎么异步更新元数据缓存的？.m4a 13.75M

 | | └──26丨MetadataCache：Broker是怎么异步更新元数据缓存的？.pdf 5.64M

 | ├──08丨消费者组管理模块 (7讲)

 | | ├──27丨消费者组元数据（上）：消费者组都有哪些元数据？.html 5.73M

 | | ├──27丨消费者组元数据（上）：消费者组都有哪些元数据？.m4a 16.03M

 | | ├──27丨消费者组元数据（上）：消费者组都有哪些元数据？.pdf 3.99M

 | | ├──28丨消费者组元数据（下）：Kafka如何管理这些元数据？.html 3.70M

 | | ├──28丨消费者组元数据（下）：Kafka如何管理这些元数据？.m4a 15.47M

 | | ├──28丨消费者组元数据（下）：Kafka如何管理这些元数据？.pdf 3.12M

 | | ├──29丨GroupMetadataManager：组元数据管理器是个什么东西？.html 3.97M

 | | ├──29丨GroupMetadataManager：组元数据管理器是个什么东西？.m4a 14.51M

 | | ├──29丨GroupMetadataManager：组元数据管理器是个什么东西？.pdf 2.66M

 | | ├──30丨GroupMetadataManager：位移主题保存的只是位移吗？.html 4.52M

 | | ├──30丨GroupMetadataManager：位移主题保存的只是位移吗？.m4a 12.03M

 | | ├──30丨GroupMetadataManager：位移主题保存的只是位移吗？.pdf 4.05M

 | | ├──31丨GroupMetadataManager：查询位移时，不用读取位移主题？.html 3.40M

 | | ├──31丨GroupMetadataManager：查询位移时，不用读取位移主题？.m4a 11.16M

 | | ├──31丨GroupMetadataManager：查询位移时，不用读取位移主题？.pdf 2.46M

 | | ├──32丨GroupCoordinator：在Rebalance中，Coordinator如何处理成员入组？.html 5.04M

 | | ├──32丨GroupCoordinator：在Rebalance中，Coordinator如何处理成员入组？.m4a 16.83M

 | | ├──32丨GroupCoordinator：在Rebalance中，Coordinator如何处理成员入组？.pdf 3.66M

 | | ├──33丨GroupCoordinator：在Rebalance中，如何进行组同步？.html 5.37M

 | | ├──33丨GroupCoordinator：在Rebalance中，如何进行组同步？.m4a 13.10M

 | | └──33丨GroupCoordinator：在Rebalance中，如何进行组同步？.pdf 3.52M

 | ├──09丨特别放送 (5讲)

 | | ├──特别放送（二）丨一篇文章带你了解参与开源社区的全部流程.html 2.46M

 | | ├──特别放送（二）丨一篇文章带你了解参与开源社区的全部流程.m4a 6.57M

 | | ├──特别放送（二）丨一篇文章带你了解参与开源社区的全部流程.pdf 1.79M

 | | ├──特别放送（三）：我是怎么度过日常一天的？.html 2.85M

 | | ├──特别放送（三）：我是怎么度过日常一天的？.m4a 7.95M

 | | ├──特别放送（三）：我是怎么度过日常一天的？.pdf 2.32M

 | | ├──特别放送（四）丨20道经典的Kafka面试题详解.html 1.80M

 | | ├──特别放送（四）丨20道经典的Kafka面试题详解.m4a 20.18M

 | | ├──特别放送（四）丨20道经典的Kafka面试题详解.pdf 1.29M

 | | ├──特别放送（五）丨Kafka社区的重磅功能：移除ZooKeeper依赖.html 7.97M

 | | ├──特别放送（五）丨Kafka社区的重磅功能：移除ZooKeeper依赖.m4a 16.44M

 | | ├──特别放送（五）丨Kafka社区的重磅功能：移除ZooKeeper依赖.pdf 5.64M

 | | ├──特别放送（一）丨经典的Kafka学习资料有哪些？.html 4.33M

 | | ├──特别放送（一）丨经典的Kafka学习资料有哪些？.m4a 7.54M

 | | └──特别放送（一）丨经典的Kafka学习资料有哪些？.pdf 4.13M

 | ├──10丨期中、期末测试 (2讲)

 | | ├──期末测试丨一套习题，测试你的掌握程度.html 2.06M

 | | ├──期末测试丨一套习题，测试你的掌握程度.m4a 917.48kb

 | | ├──期末测试丨一套习题，测试你的掌握程度.pdf 1.36M

 | | ├──期中测试丨这些源码知识，你都掌握了吗？.html 1.75M

 | | └──期中测试丨这些源码知识，你都掌握了吗？.pdf 1.32M

 | └──11丨结束语 (1讲)

 | | ├──结束语丨源码学习，我们才刚上路呢.html 2.49M

 | | ├──结束语丨源码学习，我们才刚上路呢.m4a 5.95M

 | | └──结束语丨源码学习，我们才刚上路呢.pdf 1.64M

  