# 基于区块链技术的超级账本(Hyperledger) &#8211; 从理论到实战

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.dyqufx.com/posts?id=2748

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515184256/664491b09b82b.jpg" width="500" alt="">

  什么是区块链？简单来说区块链就是一个分布式的记账本，或者分布式的数据库。

 区块链的数据结构是一个链表，交易数据被存储到链表的区块中，区块链的第一个区块叫创世区块，除了创世块以外，每个区块还包含前一个区块的哈希指针，这个哈希指针的值是根据前一个区块的实际数据计算出来的。哈希指针指向前一个区块，后面的区块可以查找前面所有区块的信息。

 账本的数据结构就是这样的一个链表，那么分布式的含义是什么呢？

 基于区块链技术的超级账本(Hyperledger) &#8211; 从理论到实战



 区块链的众多参与者组成了一个松散自治的 P2P 网络，我们把区块链网络的参与者叫做节点，每个节点都拥有一个账本拷贝，所有账本的信息都是一致的，在区块链里没有中心节点。每当有新的交易进来，所有节点的账本都会更新，并且最终保持一致。更新的方式不是去修改某个区块的值，而是保存交易记录。比如在比特币系统中，它没有用户资产记录这样的概念，不像普通数据库那样用一条数据存储资产，比特币用户资产的值是通过把所有的交易记录串联聚合后得到的，账户里资产的来源可以一直向上追溯，直到创世块为止。区块链里的交易数据根据具体场景，可以是任何需要记录的信息。

 【资源目录】:

 ├──第二部分

 | ├──01_开发环境复习.mp4 92.26M

 | ├──02_hyperledger开发环境脚本分析.mp4 105.31M

 | ├──03_byfn脚本分析.mp4 120.40M

 | ├──04_cryptogen的配置(定义谁是谁).mp4 76.19M

 | ├──05_在创世区块里面声明orderer和peer所在的org.mp4 66.80M

 | ├──06_orderer节点的配置(性能调优).mp4 62.89M

 | ├──07_创建orderer节点的创世区块和channel.mp4 112.94M

 | ├──08_更新通讯的锚节点.mp4 26.73M

 | ├──09_手动创建网络手动执行e2e的逻辑.mp4 243.27M

 | ├──10_手动创建channel,加入channel.mp4 99.85M

 | ├──11_chaincode的编写和部署.mp4 85.38M

 | ├──12_invoke逻辑的编写.mp4 106.94M

 | ├──13_开发环境nodejs搭建.mp4 98.92M

 | ├──14_nodejs开发调试环境的搭建.mp4 178.02M

 | ├──15_nodejs 链码的架构.mp4 96.43M

 ├──第三部分

 | ├──01_hyperledger fabirc的工作流程.mp4 136.33M

 | ├──02_fabirc架构流程分析.mp4 22.07M

 | ├──03_hyperledger的其他重要概念.mp4 42.35M

 | ├──04_hyperledger前后端开发环境搭建.mp4 88.44M

 | ├──05_区块链技术的使用场景.mp4 34.83M

 | ├──06_fabirc项目分析和简历书写.mp4 63.93M

 | ├──07_渔业管理系统智能合约的编写.mp4 105.29M

 | ├──08_nodejs链码和go语言链码的类比.mp4 65.81M

 | ├──09_网络环境配置.mp4 77.29M

 | ├──10_网络的docker-composer文件讲解.mp4 32.97M

 | ├──11_环境问题的debug.mp4 214.71M

 | ├──12_hyperledger的环境搭建完成.mp4 107.01M

 | ├──13_注册用户.mp4 171.85M

 | ├──14_nodejs的sdk演示.mp4 161.10M

 | ├──15_nodejs中间件获取服务器数据.mp4 93.62M

 | ├──16_coachdb的配置.mp4 167.02M

 └──第一部分

 | ├──01_hyperledger简介.mp4 38.89M

 | ├──02_hyperledger的参与人和合作伙伴.mp4 16.93M

 | ├──03_hyperledger重建信任.mp4 36.68M

 | ├──04_hyperledger的重要概念.mp4 58.63M

 | ├──05_资产&amp;链码和账本.mp4 26.58M

 | ├──06_hyperledger解决现实问题.mp4 35.73M

 | ├──07_msp和fabirc ca概念入门.mp4 28.01M

 | ├──08_hyperledger中的peer,client和orderer节点.mp4 40.45M

 | ├──09_hyperleger业务分析.mp4 42.69M

 | ├──10_channel详解.mp4 53.38M

 | ├──11_chaincode详解.mp4 53.99M

 | ├──12_hyperledger的工作流程.mp4 75.31M

 | ├──13_术语回顾.mp4 14.95M

 | ├──14_渔业系统业务复盘.mp4 61.42M

 | ├──15_docker简介.mp4 73.81M

 | ├──16_docker的原理和工作模式.mp4 38.32M

 | ├──17_docker的安装.mp4 77.61M

 | ├──18_docker常用指令快速入门.mp4 57.10M

 | ├──19_hyperledger的环境搭建.mp4 209.50M

 | ├──20_hyperledger fabirc end 2 end案例解析.mp4 145.12M

 | ├──21_hyperledger的end2end业务复盘.mp4 48.91M

  