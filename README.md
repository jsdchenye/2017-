# 2017个人总结
2016年这一年，刚开始工作。如果用一句话来形容今年的话就是：
快速迭代前端技术，打磨一套开发方案；
大量开发前端项目，历练工作实践能力；


2016.4.7号正式入职加入百度外卖。经历了部门前端从独挑大梁到，互相扶持到游刃有余，蓬勃发展。目前总人数已经达到5人。
开发方案从：fis3+smarty+jquery+bootstrap+css，到fis3+vue+vuex+jquery+bootstrap+less+es6，到目前最终统一的高效开发方案：
webpack+react+react-redux+react-router+antd+less+es6的方案；并且最终统一了我们前端这边的开发方案。在此基础之上对于这套方案的
性能进行优化，最大化的提高开发效率，优化工作性能。
开发的新项目有10多个，加上一些重构和迭代的项目。总体上这一年开发了很多项目，并且为了促进自己的提高，并没有一套方案用到老。
基本每次开发完一个项目都会对开发方案、数据结构、功能、性能等方面进行一些总结和反思。并将好的可以提高、优化的点加入到下一次
的项目开发中。所以这么多项目开发下来，对于各方面的知识都有一个提高。
对于明年也就是2017年自己也有一些规划。今年的目标是：知其所以然。从原理、为什么这样触发，不仅要知道这样开发，还要知道背后的原因。
所以会深入js的原理、框架的实现方面来提高自己。

我记得3月份刚过来的时候，那时候用的还是jquery、bootstrap这一套方案。那时候还只听过angular框架，但是一直没有使用过。所以基本上
用的还是html，script引进js文件这样子的比较传统的实现方案。jquery对于dom的一些基本操作封装的还是比较不错的。基本上的一些关于css
的操作，事件的操作还是很方便的。bootstrap作为一套全面的开发方案。link引入之后，按照你需要使用的一些功能标签基本上可以实现。当时
就用这一套开发第一个项目：商户标签。
这个项目是一个大的系统级的平台，说实话作为一个实习生来做，确实给了我很大的压力。但是也从另一方面让我感受到，遇到问题不要慌，一点
点的进行拆解，逐个击破，问题就是慢慢得到解决。有时候说来容易，确实需要一定的耐心和勇气。
后来慢慢接手到导师分配我的项目的时候，开始学习和使用fis3，因为这边项目的编译，上线都是走的fis编译这一套流程。fis作为百度内部自己研发的
一个大型的工具。对于文件路径依赖的解决，对于项目目录中文件的编译，发到到远端odp机器确实做得挺好。使用fis的时候需要安装对应的工具。
然后需要配置对应的page、template、static的开发目录结构。配合fis-conf.js文件，对上述目录中的文件进行压缩、md5处理，然后发布到测试机。
配合fis，比较常用的就是smarty开发模板。作为模板他有自己的一套语言规范在里面，反正开发起来感觉怪怪的。这套方案的开发体验不是很好，
后来就摒弃了。
后来在重构do平台的时候，部门有个大牛推荐使用vue，说是比较好上手，开发体验、性能也都能满足这个项目的需求。于是看了vue的官网，学习
了vue的基本使用。很快就用vue开发完了这个项目，体验非常的棒。vue独特的按照功能模块进行开发。将每一个功能模块拆分开。用heml和new一个vue对象来实现。
其中比较出彩的就是它的简单的双向数据流操作。通过js对象操作的发发defineProperty中的getter和settet来实现双向绑定。轻便、好用。
html的编写基本上和原生的html编写没啥差别。只不过会有一些vue的表标识符v-for，v-if之类的逻辑语句操作符。方便页面内容的呈现和展示。
然后通过new的一个vue的对象中的，data进行数据的管理。其中的生命周期函数以及各式的方法也提供了很好的交互操作体验。后来随着项目的
结构变得复杂，加入了vuex用来管理其中的数据流。这样子项目结构以及对应的流程操作就更加清晰并且方面管理。vuex中约束好的immutable才能
修改数据状态使得数据流的动向更加清晰并方便管理。总之这一套开发方案对于以前老项目的重构也是特别的友好。后来这一套方案开发了一段时间。
直到有一天对于前端UI的组件支持的不是很好。vue的生态不像现在这么好，各类支持vue的前端组件层出不穷，我们公司的B端相应的维护了一套基于
vue的前端组件。当时其实有打算开发一些基于vue的组件的，但是由于项目排期太紧急，基本上两个项目之间根本没啥时间来弄一套这个方案。
加上组里新来的一个工作两年的同事，一直力推我们react。主要当时react的升天已经特别好，antd简直好用到爆。所以就尝试了一下用react。
变成jsx的编写语法，一开始的确不舒服，后来webpack+react+antd的开发方案月开发越爽。不仅效率很高，而且界面风格很统一很优美。所以后半年
大部分项目的开发方案就确定下来了。统一为webpack+react+redux+router+es6+less+antd的开发方案。
我是不太喜欢各种换框架的，觉得还是从提高项目开发效率、项目的性能、UI风格、后期维护等角度来确定自己适合的开发方案。这东西在与深度，
所以基本上就确定了我们这边前端额开发技术栈。redux的数据流管理想当的直观。项目开发多了之后，你就会有一个体会：一个项目基本上就是用
jsx语法写好了页面架子，然后通过数据流来填充对应架子空出的部分，形成一个有血有肉的项目。特别清晰。antd的使用简直方便到死，基本上
你所需要的功能标签都能找到。而且ui统一，开发体验特别棒。
然后es6部分的一些语法，let，promise，箭头函数以及es7中的async、await对于将异步开发变为同步开发的体验也特别棒。更少的代码，更加清晰的
逻辑和结构。webpack配置那块其实做了蛮多优化。因为当你可以随意很低成本的引入模块的时候，会导致打包出来的文件特别大，到了上线使用的
时候，加载会比较慢，体验会很差。回来对webpack的js文件进行了压缩、合并、分文件进行处理，大大优化了项目的性能体验。基本上一个js文件维持在
不超过300kb左右。体验还挺不错。

写的比较匆忙，很多东西都没有细细拎出来写。待会儿得去赶车了，2017加油！
