# 从零实现分布式 KV数据库

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.dyqufx.com/posts?id=2466

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515184012/6644910c8fc5c.jpg" width="500" alt="">

  从零实现分布式 KV数据库



 ├──kv视频

 | ├──01. Raft 论文解读.mp4 91.51M

 | ├──04. Raft PartA 状态转换.mp4 34.98M

 | ├──15. Raft PartC 实现和优化.mp4 120.59M

 | ├──20. Raft PartD 调试和小结.mp4 38.79M

 | ├──22 基于 raft 的分布式 KV 概述.mp4 23.99M

 | ├──23 kvraft Client 端处理.mp4 530.08M

 | ├──24 kvraft Server 端处理.mp4 1.07G

 | ├──26 带 snapshot 的 kvraft 实现.mp4 42.18M

 | ├──29 shard controller 的 Server 端处理.mp4 60.92M

 | ├──31 shardkv 单 Group 逻辑.mp4 1.47G

 | ├──32 shardkv 配置变更.mp4 865.19M

 | ├──33 shardkv 分片迁移.mp4 1019.99M

 | ├──35 shardkv 补充修改.mp4 501.39M

 | ├──‌‬‍‌⁡⁣‍⁤‬‬‬⁤⁡⁣‍‬‍⁤⁡⁤⁡⁢‬⁢⁤‍‍‬⁡‌‍⁡‌‬07. Raft PartA 调试和小结.mov 190.70M

 | ├──‍⁤⁡⁡⁢‍⁤⁡⁢‍‬⁣⁡‬⁡⁡‌⁣‬‬⁢⁡⁤⁢⁤‬‬‌⁤‬⁢⁡13. Raft PartB 调试和小结.mov 1.20G

 | ├──‍‌⁣⁢⁡‌⁡⁡‌⁡⁡⁡‌‍‍⁢⁤⁡⁤‬‌‌⁡⁣‍‍‍⁢‌‬‌11. Raft PartB 选举日志比较.mov 355.93M

 | ├──‍‬‬‍‬⁡‍‌⁣⁡⁡‌‌‍⁢‌⁡‌⁤⁤⁡⁢⁣⁡⁣⁢⁤⁡‌‬‌⁤⁣18. Raft PartD 日志重构.mov 2.16G

 | ├──⁡⁢‬‌⁡‍⁡‬⁢⁤⁤⁡⁤‌‍‌‍‌⁢⁡‌‬⁢⁢⁡⁤⁣‬⁤⁣⁤‌09. Raft PartB 结构调整.mp4 23.44M

 | ├──‬⁤‍⁢‌⁡⁢⁢⁤⁤‍‬‌⁣⁣‍⁢‍‍⁢⁢⁤⁤⁡‌‬⁡⁤‌⁤⁣⁣‬⁣‍‌⁤28 shard controller 的 Client 端处理.mp4 376.13M

 | ├──‌⁢⁣‍‬⁡⁤⁡⁤⁤⁢⁤⁤⁢⁣‌⁤⁢‍‍⁢⁤⁡⁢⁢‍⁡⁣⁡‬⁤⁣05. Raft PartA 选举逻辑.mov 639.31M

 | ├──‍⁡‬‍‌⁡⁢‬⁢⁣‌⁢⁤‌‍‌⁣⁤⁢‌⁣‌⁢⁢⁢‍⁡‌‍⁢‬⁡‬⁢06. Raft PartA 心跳逻辑.mp4 49.27M

 | ├──‌‌‌⁢‌‍⁣⁡⁡⁢‬‍⁤‌‌⁤⁣⁢⁢‍⁣‍‌‍‌⁡⁡⁡⁡‌‬‌⁢‬⁢⁣10. Raft PartB 日志复制.mp4 92.49M

 | ├──⁣⁣⁡⁢⁤‍⁣‍‍‍⁢⁢⁤⁣⁡⁢⁤⁢‌⁣‍⁤⁣⁡‬‌⁣⁤⁣⁡⁢12. Raft PartB 日志应用.mov 711.64M

 | ├──‬⁤⁣⁢‌⁣⁡⁡‬⁢‌‍‍‍‌‌⁣⁢‍⁣‬⁢⁢‍⁤⁣‌‬⁤‌⁤‍⁤⁢16. Raft PartC 调试和小结.mp4 112.33M

 | ├──‌‍‬⁢‬⁣⁡⁢⁢⁣⁡‬⁡‍‌‬⁣‍⁢⁡⁣⁢‌‬⁢⁣⁡⁣‬‬⁢⁣‍‌⁡19. Raft PartD 快照数据流.mp4 94.09M

 | ├──‍⁢⁣‍⁡⁡⁡⁡⁢‍‌⁣‌⁣‬‬‌‬⁡‍‍‌‍⁢‍‌⁡‌⁣⁣⁢‬‬‬⁣34 shardkv 分片清理.mp4 494.21M

 | ├──‌⁣⁢⁡‌⁤‍⁤‍⁡⁡‌‬⁣⁢⁢‍⁡‌⁣⁤⁣‍⁣⁡⁢⁢‍‬⁣‌⁤‍⁢⁤‌‌‌‍25 kvraft 的节点故障与重复请求.mp4 661.59M

 | ├──‍⁢⁡‍⁣‌⁤⁤⁢‌‌⁢‬⁢‌⁤⁤⁤⁣‌‍⁤⁤‌⁣⁡⁣‬⁣‬⁣⁢‌⁤‬⁤⁣‍⁤⁢02. Raft 代码总览.mp4 59.50M

 | ├──‍⁣‌‬⁣⁡⁡⁤‍⁢⁤⁡‍⁣‍⁤⁡⁤‬‌‬⁣⁣‍‍‌‍‌⁣‬‬‌⁡⁣⁡⁡⁡⁤27 基于 multi raft 的 shardkv 概述.mp4 586.80M

 | ├──‌⁣⁣‌⁤⁡⁣⁣⁤‬‌⁤⁡‌⁤⁡‌‌‍‌⁢‌⁡‬⁢⁣‬⁡⁢‌‌⁢‌‍‬⁡⁤⁣⁣30 shard controller 的状态机处理_1.mp4 272.26M

 | └──‌⁣⁣​‌⁤⁡⁣⁣⁤‬‌⁤⁡‌⁤​​⁡‌‌‍‌⁢‌⁡‬​​⁢⁣‬⁡​⁢​‌‌⁢‌​‍‬⁡⁤⁣⁣30 shard controller 的状态机处理_2.mp4 993.64M

 └──kv资料

 | ├──doc

 | | └──kv_doc.zip 5.93M

 | └──repo

 | | ├──raft-course-example.zip 98.46kb

 | | ├──raft-course-main.zip 34.35kb

 | | ├──raft-course-raft.zip 42.80kb

 | | └──raft-course-stash.zip 91.61kb

  