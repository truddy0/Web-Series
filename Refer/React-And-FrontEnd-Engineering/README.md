> 本系列文章从属于[]()，本书的首要目标即是以 React 为核心的技术体系为主线，为读者构建完整的前端技术知识体系，探讨前端工程化的思想，并且能使不同技术水准的读者都有所得；更多 React 技术栈相关学习资料参考。


# 前言

近年来，随着浏览器性能的提升与移动互联网浪潮的汹涌而来，Web 前端开发进入了高歌猛进，日新月异的时代。这是最好的时代，我们永远在前行，这也是最坏的时代，无数的前端开发框架、技术体系争妍斗艳，让开发者们陷入困惑，乃至于无所适从。Web 前端开发可以追溯于 1991 年蒂姆·伯纳斯-李公开提及 HTML 描述，而后 1999 年 W3C 发布 HTML4 标准，这个阶段主要是 B/S 架构，没有所谓的前端开发概念，网页只不过是后端工程师的顺手之作，服务端渲染是主要的数据传递方式。接下来的几年间随着互联网的发展与 REST 等架构标准的提出，前后端分离与富客户端的概念日渐为人认同，我们需要在语言与基础的 API 上进行扩充，这个阶段出现了以 jQuery 为代表的一系列前端辅助工具。2009 年以来，智能手机开发普及，移动端大浪潮势不可挡，SPA 单页应用的设计理念也大行其道，相关联的前端模块化、组件化、响应式开发、混合式开发等等技术需求甚为迫切。这个阶段催生了 Angular 1、Ionic 等一系列优秀的框架以及 AMD、CMD、UMD 与RequireJS、SeaJS 等模块标准与加载工具，前端工程师也成为了专门的开发领域，拥有独立于后端的技术体系与架构模式。而近两年间随着Web应用复杂度的提升、团队人员的扩充、用户对于页面交互友好与性能优化的需求，我们需要更加优秀灵活的开发框架来协助我们更好的完成前端开发。这个阶段涌现出了很多关注点相对集中、设计理念更为优秀的框架，譬如 React、Vue.js、Angular 2 等组件框架允许我们以声明式编程来替代以DOM操作为核心的命令式编程，加快了组件的开发速度，并且增强了组件的可复用性与可组合性。而遵循函数式编程的Redux与借鉴了响应式编程理念的MobX都是非常不错的状态管理辅助框架，辅助开发者将业务逻辑与视图渲染剥离，更为合理地划分项目结构，更好地贯彻单一职责原则与提升代码的可维护性。在项目构建工具上，以 Grunt、Gulp 为代表的任务运行管理与以 Webpack、Rollup、JSPM 为代表的项目打包工具各领风骚，帮助开发者更好的搭建前端构建流程，自动化地进行预处理、异步加载、Polyfill、压缩等操作。

总结而言，目前前端工具化已经进入到了非常繁荣的时代，而很多前端开发者也甚为苦恼，疲于学习。本书的首要目标即是以 React 为核心的技术体系为主线，介绍目前前端开发的基本概念，帮助初级前端开发者搭建前端知识体系，能够迅速进入前端开发的工作中。而蕴藏在工具化之中的是抽象而出的设计理念与编程范式，总结而言即是对于前端工程化的思考。工具的变革会非常迅速，很多优秀的工具可能都只是历史长河中的一朵浪花，而总结而出的工程化思维则会恒久长存。本书希望为读者构建完整的前端技术体系概念，并且能使不同技术水准的读者都有所得：

（1）希望对于没有经验的开发者能够在本书选定的最短路径上快速成为一名合格的能够利用React快速开发Web应用的现代前端开发者。每一小节都会讲解最基础的语法或者使用要点，但是不会长篇大论地介绍语法细节这些应该查看文档的内容。通过简单的示例快速上手之后，笔者会介绍很多工程当中的具体实践。可能刚入门的开发者并不能理解这些实践的意义或者价值，但是首先保证能用，而后在自己的实践中慢慢回味，逐渐明了。

（2）而对于有一定前端开发经验的开发者，本书能够帮你梳理现代纷繁复杂的前端开发状况，探寻以React为代表的百花齐放的工具库背后蕴藏的设计理念与编程范式，最终融会贯通，形成自己的前端工程化思想与体系。



> 为了方便检索目录，原书的章-节-小节三级结构以一级目录-列表键-列表项目方式呈现。

- [React 初窥](React 初窥/index.md)
  - [React 思维模式](React 初窥/https://github.com/wxyyxc1992/Web-Development-And-Engineering-Practices/blob/master/Refer/React-And-FrontEnd-Engineering/React%20%E5%88%9D%E7%AA%A5/React%20%E6%80%9D%E7%BB%B4%E6%A8%A1%E5%BC%8F.md)
  - [JSX](React 初窥/JSX.md)
  - [搭建 React 脚手架](React 初窥/搭建 React 脚手架.md)
  - [Webpack](React 初窥/Webpack.md)
- [React 组件](./React 组件/index.md)
  - [组件化](React 组件/组件化.md)
  - [组件声明](React 组件/组件声明.md)
  - [列表组件](React 组件/列表组件.md)
  - [表单组件](React 组件/表单组件.md)
  - [React 与 DOM](React 组件/React 与 DOM.md)
- [React 组件样式](React 组件样式/index.md)
  - [CSS in JS](React 组件样式/CSS-in-JS.md)
  - [CSS 样式](React 组件样式/CSS 样式.md)
  - [Flexbox](React 组件样式/Flexbox.md)
- [组件的数据流](组件的数据流/index.md)
  - [Props](组件的数据流/Props.md)
  - [State](组件的数据流/State.md)
  - [Context](组件的数据流/Context.md)
  - [组件间通信](组件的数据流/组件间通信.md)
  - [用户列表详情页](组件的数据流/构建列表详情页.md)
  - [组件的生命周期](组件的数据流/组件的生命周期.md)
- [React 事件系统](React 事件系统/index.md)
  - [原生事件处理](React 事件系统/原生事件处理.md)
  - [React 事件系统](React 事件系统/React 事件系统.md)
  - [React 事件列表](React 事件系统/React 事件列表.md)
- [React 动画](React 动画/index.md)
  - [CSS 动画](React 动画/CSS 动画.md)
  - [React 动画](React 动画/React 动画.md)
- [React 路由](React 路由.md)
  - [单页应用路由](React 路由/单页应用路由.md)
  - [React Router 概念](React 路由/React Router 概念.md)
  - [路由配置与匹配](React 路由/路由配置与匹配.md)
  - [路由控制](React 路由/路由控制.md)
- [Webpack 工程实战](Webpack 工程实战/index.md)
  - [资源处理](Webpack 工程实战/资源处理.md)
  - [代码分割与异步加载](Webpack 工程实战/代码分割与异步加载.md)
  - [发布到生产环境](Webpack 工程实战/发布到生产环境.md)
- [NodeJS](NodeJS/index.md) 【Z】
  - [NodeJS 初窥](NodeJS/NodeJS 初窥.md)
- [GUI 应用程序架构变迁](GUI 应用程序架构变迁/index.md)
  - [MV*](GUI应用程序架构变迁/MV*.md)
  - [Flux](GUI应用程序架构变迁/Flux.md)
- [MobX:响应式状态管理](MobX 响应式状态管理/index.md)
  - [响应式编程与 MobX](MobX 响应式状态管理/响应式编程与 MobX.md)
  - [Observable](MobX:响应式状态管理/Observable/index.md)
  - [渐进的状态管理](MobX:响应式状态管理/渐进的状态管理/index.md)
- [Redux](Redux/index.md)
  - [Flux 的不足与 Redux 三大原则](Redux/Flux 的不足与 Redux 三大原则/index.md)
  - [Redux 基本语法](Redux/Redux 基本语法/index.md)
  - [Redux 异步处理](Redux/Redux 异步处理/index.md)
  - [Redux 工程实践](Redux/Redux 工程实践/index.md)
- [React 服务端渲染](React 服务端渲染/index.md)
  - [服务端渲染概述](React 服务端渲染/服务端渲染概述.md)
  - [基于Express的渲染服务器](React 服务端渲染/基于Express的渲染服务器/index.md)
  - [基于 Next.js 快速搭建渲染服务器](React 服务端渲染/基于 Next.js 快速搭建渲染服务器/index.md)
  - [服务端渲染性能概述](React 服务端渲染/服务端渲染性能浅析.md)
- [React 工程实践](React 工程实践/index.md)
  - [Flow](React 工程实践/Flow/index.md)
  - [React 设计模式与样式指南](React 工程实践/React 设计模式与样式指南/index.md)
  - [React 性能优化](React 工程实践/React 性能优化/index.md)
  - [基于 React 的模式库](React 工程实践/基于 React 的模式库/index.md)
- [前端质量保障](前端质量保障/index.md)
  - [调试与错误追踪](前端质量保障/调试与错误追踪/index.md)
  - [单元测试](前端质量保障/单元测试/index.md)
  - [组件测试](前端质量保障/组件测试/index.md)
  - [自动化端到端测试](前端质量保障/自动化端到端测试/index.md)
- [深入 React 内部原理](深入 React 内部原理/index.md)
  - [再谈 Virtual DOM](深入 React 内部原理/再谈 Virtual DOM/index.md)
  - [React Diff 算法](深入 React 内部原理/React Diff算法/index.md)
  - [React setState](深入 React 内部原理/React setState/index.md)
  - [React Fiber](深入 React 内部原理/React Fiber/index.md)
  - [Preact](深入 React 内部原理/Preact/index.md)
- [前端工程化](前端工程化/index.md)
  - [前后端分离与全栈](前端工程化/前后端分离与全栈/index.md)
  - [工具化与工程化](前端工程化/工具化与工程化/index.md)
  - [状态管理](前端工程化/状态管理/index.md)
  - [微服务与微前端](前端工程化/微服务与微前端/index.md)
  - [渐进式的工程架构](前端工程化/渐进式的工程架构/index.md)