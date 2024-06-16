# 极客时间React实战进阶45讲（React实战进阶45讲百度云）

## 联系方式

客服微信号：itziyuan_xiaozhi

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/common/20240614073449/666b82192834a.jpg" width="200" height="200" alt="二维码">

## 课程简介

下载链接：https://it.dyqufx.com/posts?id=2308

<img src="https://ziyuanyun.oss-cn-guangzhou.aliyuncs.com/yun/20240515183814/66449096e7aaf.jpg" width="500" alt="">

  ─jk09301-React实战进阶45讲

 极客时间React实战进阶45讲（React实战进阶45讲百度云）



 | ├──01丨React出现的历史背景及特性介绍_.mp4 27.73M

 | ├──02丨以组件方式考虑UI的构建_.mp4 39.57M

 | ├──03丨JSX 的本质 不是模板引擎，而是语法糖_.mp4 27.01M

 | ├──04丨React组件的生命周期及其使用场景_.mp4 54.03M

 | ├──05丨理解 Virtual DOM 及 key 属性的作用_.mp4 37.14M

 | ├──06丨组件设计模式 高阶组件和函数作为子组件_.mp4 45.93M

 | ├──07丨理解新的 Context API 及其使用场景_.mp4 37.37M

 | ├──08丨使用脚手架工具创建 React 项目_.mp4 31.53M

 | ├──09丨打包和部署_.mp4 41.47M

 | ├──10丨Redux(1) 前端为何需要状态管理库_.mp4 22.90M

 | ├──11丨Redux(2) 深入理解 Store, Action, Reducer_.mp4 56.64M

 | ├──12丨Redux(3) 在React中使用Redux_.mp4 36.32M

 | ├──13丨Redux(4) 理解异步 Action，Redux 中间件_.mp4 47.48M

 | ├──14丨Redux(5) 如何组织Action和Reducer_.mp4 26.85M

 | ├──15丨Redux(6) 理解不可变数据（Immutability）)_.mp4 25.85M

 | ├──16丨React Router（1）：路由不只是页面切换，更是代码组织方式_.mp4 49.80M

 | ├──17丨React Router（2）：参数定义，嵌套路由的使用场景_.mp4 36.02M

 | ├──18丨UI组件库对比和介绍：Ant_.mp4 39.36M

 | ├──19丨使用Next_.mp4 45.89M

 | ├──20丨使用Jest，Enzyme等工具进行单元测试_.mp4 73.00M

 | ├──21丨常用开发调试工具：ESLint，Prettier，React DevTool，Redux DevTool_.mp4 53.99M

 | ├──22丨前端项目的理想架构：可维护，可扩展，可测试，易开发，易建构_.mp4 17.95M

 | ├──23丨拆分复杂度（1）：按领域模型（feature）组织代码，降低耦合度_.mp4 21.08M

 | ├──24丨拆分复杂度（2）：如何组织component，action和reducer_.mp4 36.70M

 | ├──25丨拆分复杂度（3）：如何组织React Router的路由配置_.mp4 44.14M

 | ├──26丨使用Rekit（1）：创建项目，代码生成和重构_.mp4 69.37M

 | ├──27丨使用Rekit（2）：遵循最佳实践，保持代码一致性_.mp4 58.49M

 | ├──28丨使用React Router管理登录和授权_.mp4 74.08M

 | ├──29丨实现表单（1）：初始数据，提交和跳转_.mp4 72.90M

 | ├──30丨实现表单（2）：错误处理，动态表单元素，内容动态加载_.mp4 49.60M

 | ├──31丨列表页（1）：搜索，数据缓存和分页_.mp4 54.94M

 | ├──32丨列表页（2）：缓存更新，加载状态，错误处理_.mp4 47.05M

 | ├──33丨页面数据需要来源多个请求的处理_.mp4 59.32M

 | ├──34丨内容页的加载与缓存_.mp4 41.37M

 | ├──35丨基于React Router实现分步操作_.mp4 51.17M

 | ├──36丨常见页面布局的实现_.mp4 72.25M

 | ├──37丨使用 React Portals 实现对话框，使用 antd 对话框_.mp4 44.72M

 | ├──38丨集成第三方JS库：以 d3_.mp4 64.01M

 | ├──39丨基于路由实现菜单导航_.mp4 38.78M

 | ├──40丨React 中拖放的实现_.mp4 107.36M

 | ├──41丨性能永远是第一需求：时刻考虑性能问题_.mp4 27.08M

 | ├──42丨网络性能优化：自动化按需加载_.mp4 56.23M

 | ├──43丨使用Reselect避免重复计算_.mp4 86.28M

 | ├──44丨下一代 React：异步渲染_.mp4 74.25M

 | └──45丨使用Chrome DevTool进行性能调优_.mp4 56.66M

 React进阶（十一）实战演练之Button组件(1) button作为最常见的页面元素，几乎所有的UI库都会将其封装为一个基础组件。

 React性能优化指南 使用React开发的项目，可以从加载性能和运行时性能两个方面进行优化。加载性能优化的目标是让用户更早地看到界面、更早地和应用交互。运行时性能优化目标是降低卡顿，交互更流畅我们知道React的setState会触发diff和更新。默认是将整个组件树进行对比，但很多情况下diff是不必要的，因为一个子组件的props没有改变，就不需要进行diff工作。为了避免这种对没有改变props的子组件进行多余的diff工作的情况，React提供了shouldComponentUpdate这个生命周期钩子， shouldComponentUpdate(nextProps, nextState) 。 这个生命周期钩子如果返回true，则会执行后面的render和diff工作，如果返回false，则React不会向下继续。用户可以在这个生命周期钩子中进行state和props的对比，判断是否需要更新。通常一个组件当前的props与nextProps属性值相同，并且state的属性值也相同，则不需要更新。React.PureComponent实现了shouldComponentUpdate这个方法，PureComponent采用了浅比较，【 前端面试刷题网站 ： 灵题库 ，收集大厂面试真题，相关知识点详细解析。】对应class组件的PureComponent，函数组件有React.memo方法实现类似的效果。React.memo由于默认的PureComponent和memo都是默认用的浅比较。因此如果对象层级较深，会导致漏更新。解决办法是，如果对象改变，重新创建一个对象，如果数组改变，重新创建一个数组，解构赋值可以很容易地实现这一点： {&#8230;oldData}；[&#8230;oldArr] 。用户可以自己实现shouldComponentUpdate以自定义比较逻辑，对于函数式组件，则可以通过React.memo的第二个参数来定义比较逻辑。如果想要精确地判断区别，除了手动判断，还有一个自动化程度比较高的方式：不可变数据，这时一个不可变数据的JS实现： immutable-js 。只有发生改动的节点会创建新的引用，因此相应的组件才会执行render和diff。结论：最佳实践是PureComponent/React.memo + 不可变数据。Fragment可以避免不必要的dom节点。JSX的标签表达式要求有一个根节点如果就想让表达式返回一个标签列表，不应该在最外层加一个根节点，应该使用Fragment。在注册事件回调时候，不要用匿名函数或者用bind生成新函数，应该用箭头函数或者构造里面bind，最好是构造函数里面bind（因为可以继承）。当我们需要注册事件回调时候，可以写成这样写：上面这两种：匿名函数和bind表达式，都不推荐。因为匿名函数的写法会在每次调用render时候都创建新的函数，而bind表达式也会在每次调用时候创建一个新的函数，React做diff时候发现事件回调函数不同，就会将旧的函数解绑（这样还会触发GC）并且绑定新的函数。因此最好这样实现更推荐后者，因为我们知道：class Test ;} 和 class Test }这两种写法的区别在于前者log是类的实例方法，而后者是原型方法，因此在构造函数中绑定，能让其他使用原型继承方法继承Test的组件可以继承到log方法。如果使用函数式组件，应该使用useCallback这个hook。关于useCallback的使用，请参考本知识库的React进阶一文。因为React在解析JSX时候需要将style对象解析成css style字符串。更推荐将样式写在CSS中。如果在render方法进行setState，可能导致循环地进行diff工作。让条件分支中只包含需要改动的元素，不包含不需要改动的元素，防止diff子节点和更新节点时候增加不必要的操作，消耗性能。应该改成下面这种写法：我们知道，Vue中有计算属性的能力，能够根据依赖的数据计算出我们关心的数据，而且有缓存的能力：依赖的值不变的话，不需要计算，直接返回结果。React如果想要实现根据依赖的数据计算我们关心的数据，方法很简单。但是这样实现没有缓存值的能力，当计算耗时较长时候会影响性能。如何实现缓存值的能力呢？可以使用memorize-one这个库： 如果使用函数式组件，可以使用useMemo来实现。关于useMemo库的使用，请参考本讲义中React进阶一文。react-vitualize启用concurrent mode之后，React会采取可中断渲染，让大规模的diff计算不会影响到界面的渲染，保证渲染和交互的流畅性。使用Suspense组件可以在加载局部组件时候有更好的切换加载体验。concurrent详细的介绍请阅读本系列concurrent mode文章。不使用key或者用index作为key，都可能使列表在变化时候，让React无法辨别前后item对应关系，只能遍历对比，更新属性，这样可能会有多余的操作，造成性能损耗。为什么需要key呢？我会单独写一篇文章详细讲解。React官方提供了一个性能检测工具： react-addons-perf 。这个工具可以在渲染React应用时候打印各个组件的各种耗时，用来分析性能浪费。其中比较重要的一个方法是printWasted()，可以打印并未更新组件的渲染操作，如果发现你的组件花了很长时间render和diff，但组件视图实际并未发生变化，那就要考虑是否需要引入PureComponent等优化渲染性能了。

   