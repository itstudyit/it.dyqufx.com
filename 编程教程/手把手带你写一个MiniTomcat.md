# 手把手带你写一个MiniTomcat

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.bcwex.shop/posts?id=5554

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20241201163018/674c1e9ab822c.jpg" width="500" alt="">

  【资源介绍】：

 众所周知，Tomcat 是应用最广泛的 Web 应用服务器，不过在实际使用 Tomcat 过程中，我们总是会遇到各种复杂问题，比如：

 如何管理多个 Servlet？

 如何支持多个独立的应用？

 大量用户请求的性能问题如何解决？

 处理高并发请求时的内存泄漏问题怎么处理？

 手把手带你写一个MiniTomcat



 ……

 这些复杂的问题出现时，如果仅仅是会使用 Tomcat 是万万不能解决的，我们需要深入 Tomcat 原理，从底层的视角审视问题，并彻底解决问题。而掌握一项技术最好也是最扎实的方式就是重造轮子。

 为此我们邀请了前 Sun Microsystems Java 研发工程师郭屹老师，他会带你一步步剖析源码，深入 Tomcat 底层原理，并让你从中领悟 Tomcat 的设计哲学，帮助你在面对复杂的生产问题时快速找到解决方案，同时也为你自己设计系统提供思路与最佳实践。

 课程设计

 MiniTomcat 的课程大体上分成四大块：HTTP Server、Connector、Container 和扩展部分。熟悉 Tomcat 的人想必更加清楚，Connector + Container 就是 Tomcat 的核心了。学习这些内容，会为进一步的研究打下良好的基础。

 【资源目录】:

 ├──01｜持久的传奇：Tomcat的发展历程与框架演进.md 10.68kb

 ├──01｜持久的传奇：Tomcat的发展历程与框架演进.mp3 10.31M

 ├──01｜持久的传奇：Tomcat的发展历程与框架演进.pdf 9.72M

 ├──02｜初出茅庐：构造一个极简的HttpServer.md 15.46kb

 ├──02｜初出茅庐：构造一个极简的HttpServer.mp3 9.34M

 ├──02｜初出茅庐：构造一个极简的HttpServer.pdf 10.24M

 ├──03｜动态Response：按照规范构造返回流.md 19.20kb

 ├──03｜动态Response：按照规范构造返回流.mp3 9.53M

 ├──03｜动态Response：按照规范构造返回流.pdf 10.20M

 ├──04｜各司其职的Server：拆分响应模块与处理模块.md 22.45kb

 ├──04｜各司其职的Server：拆分响应模块与处理模块.mp3 7.61M

 ├──04｜各司其职的Server：拆分响应模块与处理模块.pdf 9.26M

 ├──05｜Server性能提升：设计多个Processor.md 19.98kb

 ├──05｜Server性能提升：设计多个Processor.mp3 9.20M

 ├──05｜Server性能提升：设计多个Processor.pdf 9.74M

 ├──06｜规范化：引入HttpRequest与HttpResponse.md 27.08kb

 ├──06｜规范化：引入HttpRequest与HttpResponse.mp3 9.11M

 ├──06｜规范化：引入HttpRequest与HttpResponse.pdf 9.16M

 ├──07｜对内的保护：引入门面模式封装内部实现类.md 22.48kb

 ├──07｜对内的保护：引入门面模式封装内部实现类.mp3 7.61M

 ├──07｜对内的保护：引入门面模式封装内部实现类.pdf 8.55M

 ├──08｜解析参数：通过引入Cookie和Session避免反复登录.md 40.20kb

 ├──08｜解析参数：通过引入Cookie和Session避免反复登录.mp3 11.70M

 ├──08｜解析参数：通过引入Cookie和Session避免反复登录.pdf 8.12M

 ├──09｜有状态的Response：实现Session传递与Keep-alive.md 26.11kb

 ├──09｜有状态的Response：实现Session传递与Keep-alive.mp3 9.61M

 ├──09｜有状态的Response：实现Session传递与Keep-alive.pdf 8.22M

 ├──10｜ServletWrapper：如何维护Servlet生命周期及实现容器管理？.md 17.74kb

 ├──10｜ServletWrapper：如何维护Servlet生命周期及实现容器管理？.mp3 6.86M

 ├──10｜ServletWrapper：如何维护Servlet生命周期及实现容器管理？.pdf 7.89M

 ├──11｜多层容器：如何通过实现Context与Wrapper形成多层容器？.md 26.76kb

 ├──11｜多层容器：如何通过实现Context与Wrapper形成多层容器？.mp3 6.35M

 ├──11｜多层容器：如何通过实现Context与Wrapper形成多层容器？.pdf 7.86M

 ├──12｜Pipeline与Valve：如何实现容器间的调用、事务管理、权限验证？.md 44.56kb

 ├──12｜Pipeline与Valve：如何实现容器间的调用、事务管理、权限验证？.mp3 9.54M

 ├──12｜Pipeline与Valve：如何实现容器间的调用、事务管理、权限验证？.pdf 9.70M

 ├──13｜Filter与Listener：如何实现过滤和持续监听？.md 45.50kb

 ├──13｜Filter与Listener：如何实现过滤和持续监听？.mp3 8.09M

 ├──13｜Filter与Listener：如何实现过滤和持续监听？.pdf 8.02M

 ├──14｜多应用支持：拆分Context、BootStrap与路由转发.md 23.69kb

 ├──14｜多应用支持：拆分Context、BootStrap与路由转发.mp3 7.11M

 ├──15｜类加载机制的改变：如何自定义ClassLoader？.md 33.86kb

 ├──15｜类加载机制的改变：如何自定义ClassLoader？.mp3 11.09M

 ├──16｜大功告成：完成MiniTomcat.md 20.79kb

 ├──16｜大功告成：完成MiniTomcat.mp3 6.57M

 ├──开篇词｜重造轮子，探究Tomcat的秘密.md 9.35kb

 ├──开篇词｜重造轮子，探究Tomcat的秘密.mp3 9.70M

 └──开篇词｜重造轮子，探究Tomcat的秘密.pdf 10.18M

  