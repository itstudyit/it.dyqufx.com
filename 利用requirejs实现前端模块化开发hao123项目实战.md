# 利用requirejs实现前端模块化开发hao123项目实战

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.dyqufx.com/posts?id=3574

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515185227/664493eb4c4d8.jpg" width="500" alt="">

  

 课程目标：

 利用requirejs实现前端模块化开发hao123项目实战

 适应人群：

 前端开发人员

 课程介绍：

 What is RequireJS？ 在说明什么是RequireJS之前，不得不提的就是Javascript模块化历史的背景。其实在早期，javascript作为一门新兴的脚本语言出现，有着庞大的愿景，它并不是作为一门仅仅针对客户端设计的语言。只是说后来web应用的流行，javascript作为浏览器端脚本语言而迅速传开，加上Netscape和微软的竞争将其过早的标准化。所以就导致了JS的诸多缺陷，其中一个就是模块化(但是你可以惊奇地发现其实javascript有将import,export等作为保留字，说明设计的时候其实是有考虑的，新的标准es6也让原生支持模块化了)。然后随着web应用越来越复杂，嵌入的javascript代码越来越多，还有node的兴起，模块化编程就变成了必须。

 所以就有了后来Dojo工具包和Google的Closure库支持的模块系统。还有两个非常通用的标准规范，CommonJS和AMD。这里就不展开说了，我们只需要知道，实现CommonJS规范的API是同步加载模块的，而实现AMD规范的API是则是异步加载模块。

 所以理论上来说，AMD规范的非阻塞加载更加适合浏览器端。而RequireJS就是AMD规范的最好实现。抄一段官方文档对RequireJS的描述：

 RequireJS 是一个JavaScript模块加载器。它非常适合在浏览器中使用, 它非常适合在浏览器中使用，但它也可以用在其他脚本环境, 就像 Rhino and Node. 使用RequireJS加载模块化脚本将提高代码的加载速度和质量。

 Why RequireJS？ 所以，知道了RequireJS是干什么的，也差不多知道为什么我们要使用RequireJS了。不过还是总结一下用RequireJS的好处吧。

 异步“加载”。我们知道，通常网站都会把script脚本的放在html的最后，这样就可以避免浏览器执行js带来的页面阻塞。使用RequireJS，会在相关的js加载后执行回调函数，这个过程是异步的，所以它不会阻塞页面。

 按需加载。通过RequireJS，你可以在需要加载js逻辑的时候再加载对应 的js模块，这样避免了在初始化网页的时候发生大量的请求和数据传输，或许对于一些人来说，某些模块可能他根本就不需要，那就显得没有必要。

 更加方便的模块依赖管理。相信你曾经一定遇到过因为script标签顺序问题而导致依赖关系发生错误，这个函数未定义，那个变量undefine之类的。通过RequireJS的机制，你能确保在所有的依赖模块都加载以后再执行相关的文件，所以可以起到依赖管理的作用。

 更加高效的版本管理。想一想，如果你还是用的script脚本引入的方式来引入一个jQuery2.x的文件，然后你有100个页面都是这么引用的，那当你想换成jQuery3.x，那你就不得不去改这100个页面。但是如果你的requireJS有在config中做jQuery的path映射，那你只需要改一处地方即可。

 当然还有一些诸如cdn加载不到js文件，可以请求本地文件等其它的优点，这里就不一一列举了。

 RequireJS 使用需要在页面中引入的文件 &lt;script data-main=”js/main” src=”xxx/xxxx/require.js”&gt;&lt;/script&gt;使用RequireJS，你只需要引入一个require.js即可。需要说明的是，一个比较好的实践，就是你的页面上面应该也只需要通过\&lt;script\&gt;标签引入这一个js即可。然后你这个页面的所有业务逻辑只需要在main.js里面写(data-main属性作用后面会有讲)就可以了。其它引用的依赖怎么办？当然是通过require按需引入啊！

 Require基本概述其实Requirejs整个源文件包括注释就2000来行，其对外暴露的变量其实就三个,requirejs,require,define。

 这其中requirejs 只是require的一个别名，目的是如果页面中有require其它实现了，你还是能通过使用requirejs来使用requireJS API的(本文中没有相关冲突，所以还是使用require)。

 所以这意味着作为入门，你只需要掌握require,require.config,define这三样就可以了。

 本文将以介绍require,require.config,data-main,define的顺序来介绍RequireJS。让比较简单的RequireJS更加简单，争取让大家只看这篇文章就能用好RequireJS。至于RequireJS是如何解决循环依赖,对于没有实现amd的模块如何通过shim来导出，如何在node中使用等问题。本文并没有提及，详细有需要可以去官方查阅。

  