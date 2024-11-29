# 百战商城项目Spring Cloud最新架构

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.bcwex.shop/posts?id=3921

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515185418/6644945a497ba.jpg" width="500" alt="">

  〖课程介绍〗:

 百战商城项目是一个千万级综合性的B2C电子商务平台模块。用户可以在此系统中实现搜索商品、查看商品详情、将商品加入购物车、购买商品、生成订单、完成购物等一系列操作。开发此项目，我们采用前后端分离架构的方式，前端使用Vue.js开发，后端使用微服务架构方式开发，同时运用目前非常火爆的SpringCloud作为服务治理平台

 〖课程目录〗:

 

 01百战商城项目介绍.avi

 02百战商城项目架构介绍.avi

 03百战-前台系统环境.mp4

 04项目技术介绍.avi

 05创建数据库并导入sql文件.avi

 06创建bz_parent工程.avi

 07创建Mapper与Pojo项目.avi

 08使用工具生成mapper与pojo.avi

 09搭建注册中心.avi

 10将注册中心部署到linux环境中.avi

 11创建工具集项目.avi

 12后台系统项目架构设计.avi

 13创建common_item服务.avi

 14创建backend_item项目.avi

 15在common_item服务中实现查询商品.avi

 16在backend_item服务中实现查询商品.avi

 17在common_item服务中实现查询商品分类.avi

 18在backend_item服务中实现查询商品分类.avi

 19在common_item服务中实现查询商品规格参数模板.avi

 20在backend_item服务中实现查询商品规格参数模板.avi

 21在backend_item服务中实现图片上传.avi

 22在common_item服务中实现添加商品.avi

 23在common_item服务中实现添加商品描述.avi

 24在common_item服务中实现添加商品规格参数.avi

 25在backend_item服务中实现商品添加.avi

 26搭建TX-LCN服务端.avi

 27搭建TX-LCN客户端.avi

 28在common_item服务中添加分布式事务处理.avi

 29在backend_item服务中添加分布式事务处理.avi

 30在common_item服务中删除商品.avi

 31在backend_item服务中删除商品.avi

 32在common_item服务中添加商品预更新查询.avi

 33在backend_item服务中添加商品预更新查询.avi

 34解决在预更新时无法显示ItemDesc的内容.avi

 35在common_item服务中添加商品更新.avi

 36在backend_item服务中添加商品更新.avi

 37在common_item服务中添加查询全部规格参数模板.avi

 38在backend_item服务中添加查询全部规格参数模板.avi

 39在common_item服务中实现为商品分类添加规格参数模板.avi

 40在backend_item服务中实现为商品分类添加规格参数.avi

 41在common_item服务中实现删除规格参数模板.avi

 42在backend_item服务中实现删除规格参数模板.avi

 43测试添加商品与更新商品完整流程.avi

 44创建common_content服务.avi

 45创建backend_content服务.avi

 46在common_content服务中实现查询内容分类.avi

 47在backend_content服务中实现查询内容分类.avi

 48在common_content服务中实现添加内容分类.avi

 49在backend_content服务中实现添加内容分类.avi

 50在common_content服务中实现删除内容分类.avi

 51在backend_content服务中实现删除内容分类.avi

 52在common_content服务中实现修改内容分类.avi

 53在backend_content服务中实现修改内容分类.avi

 54在common_content服务中实现根据分类查询内容.avi

 55在backend_content服务中实现根据分类查询内容.avi

 56在common_content服务中实现根据分类添加内容.avi

 57在backend_content服务中实现根据分类添加内容.avi

 58在common_content服务中实现删除分类下的内容.avi

 59在backend_content服务中实现删除分类下的内容.avi

 60创建frontend_portabl项目.avi

 61在common_item服务中实现首页商品分类查询.avi

 100实现用户注册接口.avi

 101在common_redis服务中实将用户添加到缓存接口.avi

 102在frontend_sso服务中实现用户登录接口.avi

 103在common_redis服务中实现用户退出登录接口.avi

 104在frontend_sso服务中实现用户退出登录接口.avi

 105在common_redis服务中实现缓存购物车接口.avi

 106在common_redis服务中实现查询购物车接口.avi

 107在frontend_cart服务中实现用户登录状态下向购物车中添加商品.avi

 108在frontend_cart服务中实现用户登录状态下查看物车中商品.avi

 109在frontend_cart服务中实现用户登录状态下修改购物车商品数量.avi

 110在frontend_cart服务中实现用户登录状态下删除购物车中的商品.avi

 111在frontend_sso服务用户登录业务中实现同步购物车业务.avi

 112在frontend_sso服务用户登录业务中实现删除临时购物车.avi

 113在frontent_cart服务中实现结算接口.avi

 114创建frontend_order服务.avi

 115在common_redis服务中实现生成订单ID接口.avi

 116在frontend_order服务中实现创建订单接口.avi

 117提交订单后将订单中所包含的商品从购物车中删除.avi

 118在common_redis服务中实现检查用户是否登录接口.avi

 119在frontend_cart服务中添加校验用户是否登录的Interceptor.avi

 120创建网关服务.avi

 121在网关中配置后台服务代理.avi

 122在网关中配置前台服务代理.avi

 123在网关中配置超时调优.avi

 124在网关中实现对服务降级处理.avi

 125使用令牌桶算法实现限流.avi

 126使用Postman测试服务降级与网关限流.avi

 127创建分布式配置中心服务端.avi

 128安装rabbitmq.avi

 129在gitee中创建远程仓库.avi

 130在分布式配置中心服务端中添加消息总线.avi

 131在分布式配置中心客户端中添加消息总线.avi

 132将配置文件上传到gitee远程仓库中.avi

 133在每个客户端服务中创建bootstrap.yml文件.avi

 134测试分布式配置中心.avi

 135测试自动刷新配置信息.avi

 136通过Hystrix对下游服务做降级处理.avi

 137ELK分布式日志管理.avi

 138项目总结.avi

  