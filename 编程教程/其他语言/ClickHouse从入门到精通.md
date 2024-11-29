# ClickHouse从入门到精通

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.bcwex.shop/posts?id=3421

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515185149/664493c5c55e2.jpg" width="500" alt="">

  ClickHouse是一个真正面向列的DBMS，采用列式存储，提供超高压缩比的压缩算法，轻松存储海量数据。多样化的引擎方案、类LSM Tree的结构、极致的并行处理能力，可以为用户提供高吞吐实时数据处理，其单表查询能力更是尤其亮眼。

 ClickHouse多方面的优秀表现使其成为构建离线数仓、实时数仓的不二选择，深受大厂青睐，成为了近年来一个异军突起的OLAP引擎，一匹真正的黑马。

 尚硅谷不负粉丝期待，深入研发探索，解锁大家最感兴趣的ClickHouse知识点！从入门级别的单机安装、分片集群部署、数据类型讲解、多样化表引擎介绍，以及不可或缺的SQL操作详细讲解；到深入级别的执行计划操作、建表优化、表参数调优、CPU参数调优、内存参数调优，以及多种语法优化规则讲解、多种单表查询优化策略讲解；再到进阶级别的与Prometheus和Grafana集成监控详解、手动实现备份与恢复等……

 整套教程有四大特点：“新”，采用ClickHouse最新稳定版21.3.7.14；“细”，提供全部配置文档、随堂笔记、工具软件；“全”，几乎涵盖ClickHouse全部内容，一条龙搞定；“真”，以真实的生产环境场景讲解，所有知识点都围绕实用性展开，拳拳到肉，步步深入，让你从0到1轻松掌握ClickHouse！

 主讲老师：

 鹏哥 学生们亲切地称呼他：陈教授

 此人印堂发红，面带桃花，骨骼惊奇，天赋异禀，是高考数学考了150分的非人类，国防科大的高材生，修炼大数据的小天才，妥妥的人类高质量男性。

 ClickHouse教程详细目录

 01.ClickHouse总体-课程介绍

 02.ClickHouse入门-课程介绍

 03.ClickHouse入门-介绍&amp;特点

 04.ClickHouse入门-安装_准备工作

 05.ClickHouse入门-安装_单机安装

 06.ClickHouse入门-数据类型

 07.ClickHouse入门-表引擎介绍

 08.ClickHouse入门-MergeTree引擎_简单使用

 09.ClickHouse入门-MergeTree引擎_分区详解

 10.ClickHouse入门-MergeTree引擎_主键

 11.ClickHouse入门-MergeTree引擎_Order by

 12.ClickHouse入门-MergeTree引擎_二级索引

 13.ClickHouse入门-MergeTree引擎_TTL

 14.ClickHouse入门-ReplacingMergeTree引擎

 15.ClickHouse入门-SummingMergeTree引擎

 16.ClickHouse入门-开发中引擎的选择

 17.ClickHouse入门-SQL操作_Update和Delete

 18.ClickHouse入门-SQL操作_查询和函数介绍

 19.ClickHouse入门-SQL操作_多维分析函数

 20.ClickHouse入门-SQL操作_alter&amp;导出

 21.ClickHouse入门-副本引擎

 22.ClickHouse入门-分片集群介绍

 23.ClickHouse入门-分片集群实操

 24.ClickHouse高级-课程简介

 25.ClickHouse高级-新版本安装&amp;.官网在线demo介绍

 26.ClickHouse高级-执行计划_plan&amp;AST

 27.ClickHouse高级-执行计划_syntax&amp;pipeline

 28.ClickHouse高级-执行计划_老版本如何查看

 29.ClickHouse高级-建表优化_注意数据类型

 30.ClickHouse高级-建表优化_分区和索引

 31.ClickHouse高级-表参数&amp;写入和删除优化

 32.ClickHouse高级-CPU参数设置

 33.ClickHouse高级-内存参数设置

 34.ClickHouse高级-存储优化

 35.ClickHouse高级-语法优化规则_准备测试用表

 36.ClickHouse高级-语法优化规则_count优化

 37.ClickHouse高级-语法优化规则_子查询重复字段&amp;谓词下推

 38.ClickHouse高级-语法优化规则_聚合计算外推&amp;聚合函数消除

 39.ClickHouse高级-语法优化规则_删除重复字段(不同语法下)

 40.ClickHouse高级-语法优化规则_标量替换&amp;三元运算优化

 41.ClickHouse高级-单表查询优化_prewhere&amp;采样

 42.ClickHouse高级-单表查询优化_数据裁剪&amp;Orderby用法

 43.ClickHouse高级-单表查询优化_避免构建虚拟列

 44.ClickHouse高级-单表查询优化_使用uniqCombined

 45.ClickHouse高级-单表查询优化_使用物化视图&amp;其他事项

 46.ClickHouse高级-多表关联_使用IN代替JOIN

 47.ClickHouse高级-多表关联_大小表JOIN

 48.ClickHouse高级-多表关联_谓词下推

 49.ClickHouse高级-多表关联_字典表&amp;其他

 50.ClickHouse高级-数据一致性_数据准备

 51.ClickHouse高级-数据一致性_手动执行

 52.ClickHouse高级-数据一致性_通过Group by去重

 53.ClickHouse高级-数据一致性_使用Final&amp;总结

 54.ClickHouse高级-物化视图_概述

 55.ClickHouse高级-物化视图_实操

 56.ClickHouse高级-MaterializeMySQL引擎_概述

 57.ClickHouse高级-MaterializeMySQL引擎_实操

 58.ClickHouse高级-常见问题排查

 59.ClickHouse监控-概述

 60.ClickHouse监控-Prometheus&amp;Grafana安装

 61.ClickHouse监控-ClickHouse配置

 62.ClickHouse监控-配置监控实现

 63.ClickHouse备份-手动实现备份及恢复

 64.ClickHouse备份-使用clickhouse-backup

  