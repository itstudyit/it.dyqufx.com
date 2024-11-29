# Python3商业爬虫案例实战(二期)-廖雪峰

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.bcwex.shop/posts?id=2337

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515183833/664490a98cfb6.jpg" width="500" alt="">

  ├──-Python3商业爬虫案例实战(二期)-廖雪峰

 | ├──1爬虫的基本框架及知识

 | ├──2scapy框架及爬虫进阶

 | ├──3爬虫高级知识及就业培训

 | ├──资料

 | | ├──1

 | | ├──2

 | | ├──3

 | | └──课件

 | └──总结.mp4 3.68M

 京东商业化数据分析师



 这里我们定义了一个 scrape_index 方法，它接收一个参数 page，该参数代表列表页的页码。

 这里我们先构造了一个 url，通过字符串的 format 方法，传入 limit 和 offset 的值。这里 limit 就直接使用了全局变量 LIMIT 的值；offset 则是动态计算的，就是页码数减一再乘以 limit，比如第一页 offset 就是 0，第二页 offset 就是 10，以此类推。构造好了 url 之后，直接调用 scrape_api 方法并返回结果即可。

 这样我们就完成了列表页的爬取，每次请求都会得到一页 10 部的电影数据。

 由于这时爬取到的数据已经是 JSON 类型了，所以我们不用像之前那样去解析 HTML 代码来提取数据了，爬到的数据就是我们想要的结构化数据，因此解析这一步就可以直接省略啦。

 到此为止，我们能成功爬取列表页并提取出电影列表信息了。

 5. 爬取详情页 这时候我们已经可以拿到每一页的电影数据了，但是看看这些数据实际上还缺少了一些我们想要的信息，如剧情简介等信息，所以需要进一步进入到详情页来获取这些内容。

 这时候点击任意一部电影，如《教父》，进入其详情页，这时可以发现页面的 URL 已经变成了 https://spa1.scrape.center/detail/40，页面也成功展示了详情页的信息，如图所示：

  