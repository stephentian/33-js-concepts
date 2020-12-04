<h1 align="center">
<br>
  <a href="https://github.com/stephentian/33-js-concepts"><img src="33_js_concepts.jpg" alt="每位 JS 开发应该懂的 33 个概念" width=200"></a>
  <br>
    <br>
  JavaScript开发者应懂的33个概念
  <br>
</h1>

## 简介

这个项目是为了帮助开发者掌握 JavaScript 概念而创立的。它不是必备，但在未来学习（JavaScript）中，可以作为一篇指南。

> 本篇文章是参照 @leonardomso 创立，英文版项目地址在[这里](https://github.com/leonardomso/33-js-concepts)。
> 由于原版资源都要翻墙，所以本人创立一个中文版，附上关于这些概念在国内的一些文章和视频。
> 若有觉得更好的文章或者视频，可以贡献出来，觉得有误的，请联系我删除。

## 更新

若有觉得更好的文章或者视频，可以贡献出来，觉得有误的，请联系我删除。

- 文章的排序优化，前面的文章是介绍概念，后面的文章是深入解读。
- 将原文的 "高阶函数" 和 "map, reduce, filter" 合并为 "map, reduce, filter 等高阶函数"
- 增加 "promise" 概念(替换删除的 "高阶函数")
- 2018-10-24 更新：@BuptStEve 贡献的三篇关于" 函数式编程 "方面的文章
- 2018-12-04 更新：@haner199401 贡献的 @冴羽 "JavaScript 深入之从原型到原型链"

---

## 目录

1. **[调用堆栈](#1-调用堆栈)**
2. **[原始类型](#2-原始类型)**
3. **[值类型和引用类型](#3-值类型和引用类型)**
4. **[隐式, 显式, 名义和鸭子类型](#4-隐式-显式-名义和鸭子类型)**
5. **[== 与 ===, typeof 与 instanceof](#5--vs--typeof-vs-instanceof)**
6. **[this, call, apply 和 bind](#6-this-call-apply-和-bind)**
7. **[函数作用域, 块级作用域和词法作用域](#7-函数作用域-块级作用域和词法作用域)**
8. **[闭包](#8-闭包)**
9. **[map, reduce, filter 等高阶函数](#9-map-reduce-filter-等高阶函数)**
10. **[表达式和语句](#10-表达式和语句)**
11. **[变量提升](#11-变量提升)**
12. **[Promise](#12-promise)**
13. **[立即执行函数, 模块化, 命名空间](#13-立即执行函数-模块化-命名空间)**
14. **[递归](#14-递归)**
15. **[算法](#15-算法)**
16. **[数据结构](#16-数据结构)**
17. **[消息队列和事件循环](#17-消息队列和事件循环)**
18. **[setTimeout, setInterval 和 requestAnimationFrame](#18-settimeout-setinterval-和-requestanimationframe)**
19. **[继承, 多态和代码复用](#19-继承-多态和代码复用)**
20. **[按位操作符, 类数组对象和类型化数组](#20-按位操作符-类数组对象和类型化数组)**
21. **[DOM 树和渲染过程](#21-dom-树和渲染过程)**
22. **[new 与构造函数, instanceof 与实例](#22-new-与构造函数-instanceof-与实例)**
23. **[原型继承与原型链](#23-原型继承与原型链)**
24. **[Object.create 和 Object.assign](#24-objectcreate-和-objectassign)**
25. **[工厂函数和类](#25-工厂函数和类)**
26. **[设计模式](#26-设计模式)**
27. **[Memoization](#27-memoization)**
28. **[纯函数, 函数副作用和状态变化](#28-纯函数-函数副作用和状态变化)**
29. **[耗性能操作和时间复杂度](#29-耗性能操作和时间复杂度)**
30. **[JavaScript 引擎](#30-javascript-引擎)**
31. **[二进制, 十进制, 十六进制, 科学记数法](#31-二进制-十六进制-十进制-科学记数法)**
32. **[偏函数, 柯里化, Compose 和 Pipe](#32-偏函数-柯里化-compose-和-pipe)**
33. **[代码整洁之道](#33-代码整洁之道)**

---

## 1. 调用堆栈

### 文章

- :book: [Call Stack — MDN](https://developer.mozilla.org/zh-CN/docs/Glossary/Call_stack)
- :book: [[译] JavaScript 如何工作：对引擎、运行时、调用堆栈的概述 —— 掘金](https://juejin.im/post/5a05b4576fb9a04519690d42)
- :book: [[译] 理解 JavaScript 中的执行上下文和执行栈 —— 掘金](https://juejin.im/post/5ba32171f265da0ab719a6d7)
- :book: [这一次，彻底弄懂 JavaScript 执行机制 —— 掘金](https://juejin.im/post/59e85eebf265da430d571f89)
- :book: [解读 JavaScript 之引擎、运行时和堆栈调用 —— 开源中国](https://www.oschina.net/translate/how-does-javascript-actually-work-part-1)
- :book: [Tasks, microtasks, queues and schedules —— Jake Archibald](https://jakearchibald.com/2015/tasks-microtasks-queues-and-schedules/)
- :book: [Tasks, microtasks, queues and schedules（译） —— 掘金](https://juejin.im/entry/55dbd51a60b2f3a92a8f5bff)

### 视频

- :tv: [What is the event loop anyway? —— 腾讯视频(英文字幕)](https://v.qq.com/x/page/h0372bld8re.html?ptag=qqbrowser)
- :tv: [Understanding The JavaScript Call Stack, Event Queue, Event Table, & Event Loop —— Bilibili](https://www.bilibili.com/video/av33824933/)
- :tv: [JS 中的变量提升、堆栈内存及闭包详解 —— Acfun](http://www.acfun.cn/v/ac4495641)
- :tv: [事件循环模型 —— PHP 中文网](http://www.php.cn/code/21194.html)
- :tv: [Javascript: the Call Stack explained — Coding Blocks India](https://www.youtube.com/watch?v=w6QGEiQceOM)
- :tv: [The JS Call Stack Explained In 9 Minutes — Colt Steele](https://www.youtube.com/watch?v=W8AeMrVtFLY)
- :tv: [JavaScript Execution Stack — Codecademy](https://www.youtube.com/watch?v=jT0USJeNFEA)
- :tv: [What is the Call Stack? — Eric Traub](https://www.youtube.com/watch?v=w7QWQlkLY_s)
- :tv: [The Call Stack — Kevin Drumm](https://www.youtube.com/watch?v=Q2sFmqvpBe0)
- :tv: [Understanding JavaScript Execution — Codesmith](https://www.youtube.com/watch?v=Z6a1cLyq7Ac&list=PLWrQZnG8l0E4kd1T_nyuVoxQUaYEWFgcD)
- :tv: [Call Stack & Event Loop — movies com](https://www.youtube.com/watch?v=mk0lu9MKBto)

**[:arrow_up: 返回目录](#目录)**

---

## 2. 原始类型

### 文章

- :book: [原始数据 —— MDN](https://developer.mozilla.org/zh-CN/docs/Glossary/Primitive)
- :book: [[译]JavaScript 是怎样编码数字的 —— SegmentFault](https://segmentfault.com/a/1190000017090272)
- :book: [每一个 JavaScript 开发者应该了解的浮点知识 —— 颜海镜](https://yanhaijing.com/javascript/2014/03/14/what-every-javascript-developer-should-know-about-floating-points/)
- :book: [JavaScript 标准参考教程(基本语法之数值) —— 阮一峰](https://wangdoc.com/javascript/types/number.html)
- :book: [The Secret Life of JavaScript Primitives —— Angus Croll](https://javascriptweblog.wordpress.com/2010/09/27/the-secret-life-of-javascript-primitives/)

### 视频

- :tv: [javascript 六种数据类型 —— 慕课网](https://www.imooc.com/video/5674)
- :tv: [javascript 视频教程(数据类型) —— PHP 中文网](http://www.php.cn/code/5808.html)
- :tv: [JavaScript Reference vs Primitive Types — Academind](https://www.youtube.com/watch?v=9ooYYRLdg_g)
- :tv: [JavaScript Primitive Types — Simon Sez IT](https://www.youtube.com/watch?v=HsbWQsSCE5Y)
- :tv: [Javascript Primitive and Reference Types — Baljeet Singh](https://www.youtube.com/watch?v=F7YbhKbpFic)
- :tv: [Value Types and Reference Types in JavaScript — Programming with Mosh](https://www.youtube.com/watch?v=e-_mDyqm2oU)
- :tv: [JavaScript Primitive Data Types — Avelx](https://www.youtube.com/watch?v=qw3j0A3DIzQ)
- :tv: [Everything you never wanted to know about JavaScript numbers — Bartek Szopka](https://www.youtube.com/watch?v=MqHDDtVYJRI)

**[:arrow_up: 返回目录](#目录)**

---

## 3. 值类型和引用类型

### 文章

- :book: [ECMAScript 引用类型 —— W3school](http://www.w3school.com.cn/js/pro_js_referencetypes.asp)
- :book: [js 中的值类型和引用类型的区别 —— 博客园](https://www.cnblogs.com/leiting/p/8081413.html)
- :book: [JavaScript 的值传递和引用传递 —— FunDebug](https://blog.fundebug.com/2017/08/09/explain_value_reference_in_js/)
- :book: [Primitive Types & Reference Types in JavaScript —— Bran van der Meer](https://docstore.mik.ua/orelly/webprog/jscript/ch04_04.htm)
- :book: [JavaScript: Passing by Value or by Reference —— CSDN](https://blog.csdn.net/xiaojia_boke/article/details/54906509)
- :book: [js 值引用和值复制 —— SegmentFault](https://segmentfault.com/a/1190000015411195)
- :book: [js- 引用和复制(传值和传址) —— CSDN](https://blog.csdn.net/zzzaquarius/article/details/4902235)

### 视频

- :tv: [Javascript Pass by Value vs Pass by Reference — techsith](https://www.youtube.com/watch?v=E-dAnFdq8k8)
- :tv: [JavaScript Value vs Reference Types — Programming with Mosh](https://www.youtube.com/watch?v=fD0t_DKREbE)

**[:arrow_up: 返回目录](#目录)**

---

## 4. 隐式, 显式, 名义和鸭子类型

### 文章

- :book: [ECMAScript 类型转换 —— W3school](http://www.w3school.com.cn/js/pro_js_typeconversion.asp)
- :book: [JavaScript 的怪癖 1：隐式类型转换 —— justjavac](http://justjavac.com/javascript/2013/04/08/javascript-quirk-1-implicit-conversion-of-values.html)
- :book: [JavaScript 运算符规则与隐式类型转换详解 —— 掘金](https://juejin.im/post/59ad2585f265da246a20e026)
- :book: [聊一聊 JS 中的隐式类型转换 —— SegmentFault](https://segmentfault.com/a/1190000004482388)
- :book: [有趣的 JavaScript 隐式类型转换 —— 博客园](https://www.cnblogs.com/yugege/p/5277883.html)
- :book: [JavaScript 显式类型转换与隐式类型转换 —— CSDN](https://blog.csdn.net/yangjvn/article/details/48284163)
- :book: [你不知道的 JavaScript（中卷）强制类型转换 —— 简书](https://www.jianshu.com/p/777a89b4ed9a)
- :book: [你懂 JavaScript 嗎？#8 強制轉型 —— cythilya](https://ithelp.ithome.com.tw/articles/10201512)
- :book: [动态类型语言和鸭子类型 —— 曾探](http://book.51cto.com/art/201505/475153.htm)
- :book: [Nominal & Structural Typing —— flow](https://flow.org/en/docs/lang/nominal-structural/)
- :book: [What exactly is Type Coercion in Javascript? —— stackoverflow](https://stackoverflow.com/questions/19915688/what-exactly-is-type-coercion-in-javascript)
- :book: [You Don't Know JS: Types & Grammar —— github](https://github.com/getify/You-Dont-Know-JS/blob/master/types%20&%20grammar/ch4.md)

### 视频

- :tv: [javascript 隐式转换 —— 慕课网](https://www.imooc.com/video/5675)
- :tv: [Javascript 基础加强-类型转换 —— 黑马程序员](http://www.le.com/ptv/vplay/27767009.html)

**[:arrow_up: 返回目录](#目录)**

---

<div id="5--vs--typeof-vs-instanceof"></div>

## 5. == vs ===, typeof vs instanceof

### 文章

- :book: [JavaScript 中的相等性判断 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Equality_comparisons_and_sameness)
- :book: [js 中 == 和 === 的区别 —— 掘金](https://juejin.im/entry/584918612f301e005716add6)
- :book: [== vs === in Javascript —— CSDN](https://blog.csdn.net/w97531/article/details/82255225)
- :book: [深入理解 javascript 之 typeof 和 instanceof —— CSDN](https://blog.csdn.net/mevicky/article/details/50353881)
- :book: [JavaScript 的 typeof 的用途 —— justjavac](http://justjavac.com/javascript/2012/12/23/what-is-javascripts-typeof-operator-used-for.html)
- :book: [一张图看懂 Function 和 Object 的关系及简述 instanceof 运算符 —— 掘金](https://juejin.im/post/58358606570c35005e4142bd)
- :book: [浅谈 instanceof 和 typeof 的实现原理 —— 掘金](https://juejin.im/post/5b0b9b9051882515773ae714)
- :book: [typeof 和 instanceOf 的区别](https://segmentfault.com/a/1190000000730982)

**[:arrow_up: 返回目录](#目录)**

---

## 6. this, call, apply 和 bind

### 文章

- :book: [Javascript 的 this 用法 —— 阮一峰](http://www.ruanyifeng.com/blog/2010/04/using_this_keyword_in_javascript.html)
- :book: [学会 JS 的 this 这一篇就够了，根本不用记 —— 慕课网](https://www.imooc.com/article/1758)
- :book: [[译] this（他喵的）到底是什么 — 理解 JavaScript 中的 this、call、apply 和 bind —— 掘金](https://juejin.im/post/5b9f176b6fb9a05d3827d03f)
- :book: [this、apply、call、bind —— 掘金](https://juejin.im/post/59bfe84351882531b730bac2)
- :book: [使用 call、apply 和 bind 解决 js 中烦人的 this，事件绑定时的 this 和传参问题 —— 博客园](https://www.cnblogs.com/tingyu-blog/p/6212392.html)
- :book: [call、apply 和 bind 的原生实现 —— github](https://github.com/Abiel1024/blog/issues/16)

### 视频

- :tv: [JavaScript 关于 this 关键字解释 —— 爱奇艺](https://www.iqiyi.com/w_19rr1augsd.html)
- :tv: [JS 关于作用域闭包和 this 的综合面试题 —— 百度视频](http://baidu.iqiyi.com/watch/845335533383874688.html?page=videoMultiNeed)
- :tv: [js 面向对象闭包数组 12.函数中的 this —— 乐视视频](http://www.le.com/ptv/vplay/27478413.html?ch=baidu_s)
- :tv: [1.3.10-this 指向及 this 应用 —— 乐视视频](http://www.le.com/ptv/vplay/24835911.html?ch=baidu_s)
- :tv: [珠峰培训 JavaScript 开发课程：关于 this 关键字、闭包作用域 —— 网易云课堂](https://study.163.com/course/introduction/590005.htm)

**[:arrow_up: 返回目录](#目录)**

---

## 7. 函数作用域, 块级作用域和词法作用域

### 文章

- :book: [变量作用域与解构赋值 —— 廖雪峰](https://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000/0014344993159773a464f34e1724700a6d5dd9e235ceb7c000)
- :book: [学习 Javascript 闭包（Closure） —— 阮一峰](http://www.ruanyifeng.com/blog/2009/08/learning_javascript_closures.html)
- :book: [JavaScript 中词法作用域、闭包与跳出闭包 —— SegmentFault](https://segmentfault.com/a/1190000006671020)
- :book: [JavaScript 深入之词法作用域和动态作用域 —— 掘金](https://juejin.im/entry/58e70077b123db15eb88dc7e)
- :book: [深入理解闭包之前置知识 → 作用域与词法作用域 —— 掘金](https://juejin.im/post/5afb0ae56fb9a07aa2138425)
- :book: [What is lexical scope? —— stackoverflow](https://stackoverflow.com/questions/1047454/what-is-lexical-scope)
- :book: [You Don't Know JS: Scope & Closures —— Kyle Simpson](https://github.com/fishenal/You-Dont-Know-JS/blob/master/scope%20&%20closures/ch2.md)

**[:arrow_up: 返回目录](#目录)**

---

## 8. 闭包

### 文章

- :book: [闭包 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Closures)
- :book: [ECMAScript 闭包（closure）—— w3school](http://www.w3school.com.cn/js/pro_js_functions_closures.asp)
- :book: [学习 Javascript 闭包（Closure） —— 阮一峰](http://www.ruanyifeng.com/blog/2009/08/learning_javascript_closures.html)
- :book: [闭包 —— 廖雪峰](https://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000/00143449934543461c9d5dfeeb848f5b72bd012e1113d15000)
- :book: [一次性搞懂 JavaScript 闭包 —— 简书](https://www.jianshu.com/p/796e903754f1)
- :book: [JavaScript 闭包 —— SegmentFault](https://segmentfault.com/a/1190000006875662)
- :book: [js 匿名自执行函数中闭包的高级使用 —— 掘金](https://juejin.im/entry/5800eb7da22b9d005b36156e)
- :book: [高效使用 JavaScript 闭包 —— 掘金](https://juejin.im/entry/59df405251882551bf7e58c6)
- :book: [深入理解 JavaScript 原型与闭包 —— 王福朋](https://www.cnblogs.com/wangfupeng1988/p/3977924.html)

### 视频

- :tv: [JavaScript 闭包和闭包面试题 —— 爱奇艺](http://www.iqiyi.com/w_19rr1amael.html)
- :tv: [js 面向对象闭包数组 11.闭包 —— 乐视](http://www.le.com/ptv/vplay/27478410.html)
- :tv: [白贺翔\_函数(闭包) —— 乐视](http://www.le.com/ptv/vplay/30505852.html)

**[:arrow_up: 返回目录](#目录)**

---

## 9. map, reduce, filter 等高阶函数

### 文章

- :book: [高阶函数 —— 廖雪峰](https://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000/001434499355829ead974e550644e2ebd9fd8bb1b0dd721000)
- :book: [ES5 中新增的 Array 方法详细说明 —— 张鑫旭](https://www.zhangxinxu.com/wordpress/2013/04/es5%e6%96%b0%e5%a2%9e%e6%95%b0%e7%bb%84%e6%96%b9%e6%b3%95/)
- :book: [一张图看懂 JavaScript 中数组的迭代方法：forEach、map、filter、reduce、every、some —— 掘金](https://juejin.im/post/5835808067f3560065ed4ab2)
- :book: [Transducing（上）－《JavaScript 轻量级函数式编程》 —— SegmentFault](https://segmentfault.com/a/1190000012127329)
- :book: [JavaScript 函数式编程（三） —— @BuptStEve](https://github.com/BuptStEve/blog/issues/15)

**[:arrow_up: 返回目录](#目录)**

---

## 10. 表达式和语句

### 文章

- :book: [js 表达式与语句 —— 博客园](https://www.cnblogs.com/xianshenglu/p/8386918.html)
- :book: [JS 表达式和语句的区别 —— SegmentFault](https://segmentfault.com/q/1010000004102804)
- :book: [JavaScript 中的表达式（expression）和语句/声明（statement） —— CSDN](https://blog.csdn.net/mett_smith/article/details/78761247)
- :book: [重讀 Axel 的 Javascript 中的 Expression vs Statement 一文 —— SegmentFault](https://segmentfault.com/a/1190000004565693)
- :book: [Expressions versus statements in JavaScript —— Dr. Axel](http://2ality.com/2012/09/expressions-vs-statements.html)

**[:arrow_up: 返回目录](#目录)**

---

## 11. 变量提升

### 文章

- :book: [JavaScript 变量提升 —— 菜鸟教程](http://www.runoob.com/js/js-hoisting.html)
- :book: [ES6 变量作用域与提升：变量的生命周期详解 —— 掘金](https://juejin.im/post/59905bea6fb9a03c34192c51)
- :book: [[翻译] JavaScript Scoping and Hoisting —— SegmentFault](https://segmentfault.com/a/1190000004345355#articleHeader5)
- :book: [JavaScript Scoping and Hoisting —— Ben Cherry](http://www.adequatelygood.com/JavaScript-Scoping-and-Hoisting.html)

**[:arrow_up: 返回目录](#目录)**

---

## 12. Promise

### 文章

- :book: [使用 promises —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide/Using_promises)
- :book: [Promise —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)
- :book: [Promise — 廖雪峰](https://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000/0014345008539155e93fc16046d4bb7854943814c4f9dc2000)
- :book: [JavaScript Promise：去而复返 —— 司徒正美](https://www.cnblogs.com/rubylouvre/p/3495286.html)
- :book: [(上面的原文)JavaScript Promise：简介 —— Web Fundamentals](https://developers.google.com/web/fundamentals/primers/promises#_1)
- :book: [1 分钟读完《10 分钟学会 JavaScript 的 Async/Await》 —— justjavac](https://segmentfault.com/a/1190000011813934)
- :book: [JavaScript Promise 迷你书（中文版）](https://juejin.im/entry/56499ae160b2d1404c4f8834)
- :book: [JavaScript 进阶之路——认识和使用 Promise，重构你的 Js 代码 —— 博客园](https://www.cnblogs.com/yunfeifei/p/4453690.html)

### 视频

- :tv: [Promise 入门 —— 慕课网](https://www.imooc.com/learn/949)

**[:arrow_up: 返回目录](#目录)**

---

## 13. 立即执行函数, 模块化, 命名空间

### 文章

- :book: [Javascript 模块化编程（一）：模块的写法 —— 阮一峰](http://www.ruanyifeng.com/blog/2012/10/javascript_module.html)
- :book: [javascript 模块化编程-详解立即执行函数表达式 —— 简书](https://www.jianshu.com/p/4dbf4a4c8ebb)
- :book: [Javascript 的匿名函数与自执行 —— 掘金](https://juejin.im/entry/57fee360a22b9d005b1d9ae3)
- :book: [前端模块化——技术选型 —— SegmentFault](https://segmentfault.com/a/1190000006966358)
- :book: [谈谈 Js 前端模块化规范 —— SegmentFault](https://segmentfault.com/a/1190000015991869#articleHeader8)
- :book: [函数声明与函数表达式的区别 —— 伯乐在线](http://web.jobbole.com/87534/)


**[:arrow_up: 返回目录](#目录)**

---

## 14. 递归

### 文章

- :book: [求解释 js 递归 —— SegmentFault](https://segmentfault.com/q/1010000003942347)
- :book: [JavaScript 中的递归 —— 掘金](https://juejin.im/post/5948c0d8fe88c2006a939e2a)
- :book: [递归（上）－《JavaScript 轻量级函数式编程》 —— 掘金](https://juejin.im/post/59c1d91d6fb9a00a53275f79)
- :book: [递归（下）－《JavaScript 轻量级函数式编程》 —— 掘金](https://juejin.im/post/59c87fb46fb9a00a437b1a2e)
- :book: [尾调用和尾递归 —— 掘金](https://juejin.im/post/5acdd7486fb9a028ca53547c)
- :book: [几个经典递归问题用 js 实现 —— CSDN](https://blog.csdn.net/qianqianstd/article/details/75807462)
- :book: [递归函数的几个例子 —— CSDN](https://blog.csdn.net/x_i_xw/article/details/72026868)

**[:arrow_up: 返回目录](#目录)**

---

## 15. 算法

### 文章

- :book: [十大经典排序算法总结（JavaScript 描述） —— 掘金](https://juejin.im/post/57dcd394a22b9d00610c5ec8)
- :book: [在 JavaScript 中学习数据结构与算法 —— 掘金](https://juejin.im/post/594dfe795188250d725a220a#comment)
- :book: [JS 中可能用得到的全部的排序算法 —— 掘金](https://juejin.im/post/58c9d5fb1b69e6006b686bce)
- :book: [JS 家的排序算法 —— 简书](https://www.jianshu.com/p/1b4068ccd505)
- :book: [前端常见算法的 JS 实现 —— SegmentFault](https://segmentfault.com/a/1190000008593715)
- :book: [前端面试中的常见的算法问题 ——蒲小花的博客](https://www.jackpu.com/qian-duan-mian-shi-zhong-de-chang-jian-de-suan-fa-wen-ti/)

### 视频

- :tv: [Javascript 实现二叉树算法 —— 慕课网](https://www.imooc.com/learn/888)

**[:arrow_up: 返回目录](#目录)**

---

## 16. 数据结构

### 文章

- :book: [来我们浅谈一下 js 的数据结构 —— 简书](https://www.jianshu.com/p/5e0e8d183102)
- :book: [JavaScript 中的算法与数据结构 —— 简书](https://www.jianshu.com/nb/16835496)
- :book: [学 JS 必看-JavaScript 数据结构深度剖析 —— 大道至简的博客](http://blog.sina.com.cn/s/blog_7b9c5e4101017mjt.html)
- :book: [js 中基础数据结构数组去重问题 —— 掘金](https://juejin.im/entry/586effe0da2f600053d85a9a)

### 视频

- :tv: :tv: [JavaScript 数据结构-运算符 —— 乐视](http://www.le.com/ptv/vplay/27606964.html)

**[:arrow_up: 返回目录](#目录)**

---

## 17. 消息队列和事件循环

### 文章

- :book: [并发模型与事件循环 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/EventLoop)
- :book: [JavaScript 运行机制详解：再谈 Event Loop —— 阮一峰](http://www.ruanyifeng.com/blog/2014/10/event-loop.html)
- :book: [深入理解 JavaScript 事件循环 —— 博客园](https://www.cnblogs.com/dong-xu/p/7000163.html)
- :book: [深入浅出 Javascript 事件循环机制 —— 知乎](https://zhuanlan.zhihu.com/p/26229293)
- :book: [JS 事件循环机制（event loop）之宏任务、微任务 —— SegmentFault](https://segmentfault.com/a/1190000014940904#articleHeader7)
- :book: [JavaScript：彻底理解同步、异步和事件循环 —— SegmentFault](https://segmentfault.com/a/1190000004322358)
- :book: [从浏览器多进程到 JS 单线程，JS 运行机制最全面的一次梳理 —— 掘金](https://juejin.im/post/5a6547d0f265da3e283a1df7)

**[:arrow_up: 返回目录](#目录)**

---

## 18. setTimeout, setInterval 和 requestAnimationFrame

### 文章

- :book: [Window setTimeout() 方法 —— 菜鸟教程](http://www.runoob.com/jsref/met-win-settimeout.html)
- :book: [Window setInterval() 方法 —— 菜鸟教程](http://www.runoob.com/jsref/met-win-setinterval.html)
- :book: [关于 setTimeout —— 掘金](https://juejin.im/post/5aa4c47af265da239866e236)
- :book: [你不知道的 Javascript：有趣的 setTimeout —— 掘金](https://juejin.im/post/5a77f8ce5188257a6d635d76)
- :book: [原来你是这样的 setTimeout —— 掘金](https://juejin.im/entry/5861ebf01b69e6006ce61d38)
- :book: [setTimeout() 和 setInterval() 本质区别在哪里？ —— SegmentFault](https://segmentfault.com/q/1010000005989491)
- book: [window.requestAnimationFrame —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/API/Window/requestAnimationFrame)
- :book: [requestAnimationFrame 知多少？ —— 博客园](http://www.cnblogs.com/onepixel/p/7078617.html)
- :book: [CSS3 动画那么强，requestAnimationFrame 还有毛线用？ —— 张鑫旭](https://www.zhangxinxu.com/wordpress/2013/09/css3-animation-requestanimationframe-tween-%e5%8a%a8%e7%94%bb%e7%ae%97%e6%b3%95/)
- :book: [「JavaScript 定时器」setInterval、setTimeout 和 requestAnimationFrame 浅析 —— SegmentFault](https://segmentfault.com/a/1190000014661035)
- :book: [翻译：setInterval 与 requestAnimationFrame 的时间间隔测试 —— SegmentFault](https://segmentfault.com/a/1190000000386368)
- :book: [阿里前端面试题：requestAnimationFrame 实现类似 setInterval 的计时器 —— SegmentFault](https://segmentfault.com/q/1010000013909430)

### 视频

- :tv: [setTimeout 和 setInterval —— 优酷](http://v.youku.com/v_show/id_XNTA4OTQ0NzA0.html)

**[:arrow_up: 返回目录](#目录)**

---

## 19. 继承, 多态和代码复用

### 文章

- :book: [JS 面向对象编程之：封装、继承、多态 —— 博客园](https://www.cnblogs.com/Leo_wl/p/5734794.html)
- :book: [Javascript 的继承与多态 —— 简书](https://www.jianshu.com/p/5cb692658704)
- :book: [js:面向对象编程，带你认识封装、继承和多态 —— 掘金](https://juejin.im/post/59396c96fe88c2006afc2707)
- :book: [JavaScript 中的“多继承” —— 掘金](https://zhuanlan.zhihu.com/p/34693209)
- :book: [代码复用模式 —— github](https://github.com/TooBug/javascript.patterns/blob/master/chapter6.markdown)
- :book: [深入理解 JavaScript：代码复用模式(推荐篇) —— 汤姆大叔](http://www.cnblogs.com/TomXu/archive/2012/04/24/2438050.html)
- :book: [深入理解 JavaScript：代码复用模式(避免篇) —— 汤姆大叔](https://www.cnblogs.com/TomXu/archive/2012/04/23/2438005.html)

**[:arrow_up: 返回目录](#目录)**

---

## 20. 按位操作符, 类数组对象和类型化数组

### 文章

- :book: [按位操作符 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/Bitwise_Operators)
- :book: [类数组对象 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Typed_arrays)
- :book: [类型化数组 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/ArrayBuffer)
- :book: [JavaScript ArrayBuffer 浅析 —— 博客园](https://www.cnblogs.com/gradolabs/p/4762134.html)

**[:arrow_up: 返回目录](#目录)**

---

## 21. DOM 树和渲染过程

### 文章

- :book: [如何创建一个 DOM 树 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/API/Document_Object_Model/How_to_create_a_DOM_tree)
- :book: [HTML DOM 节点 —— W3school](http://www.w3school.com.cn/htmldom/dom_nodes.asp)
- :book: [DOM 概述 —— 阮一峰](http://javascript.ruanyifeng.com/dom/node.html)
- :book: [《JavaScript 闯关记》之 DOM（上）—— 掘金](https://juejin.im/post/583cbbfa61ff4b006ccc41fe)
- :book: [《JavaScript 闯关记》之 DOM（下）—— 掘金](https://juejin.im/post/583cbc4961ff4b006ccc44fb)
- :book: [掌握 DOM 操作 —— 掘金](https://juejin.im/entry/58314efd8ac2470061bb30fd)
- :book: [操作 DOM —— 廖雪峰](https://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000/001434500494451273e6b3dec9d411d9ba841dee8caec45000)
- :book: [原来 CSS 与 JS 是这样阻塞 DOM 解析和渲染的 —— 掘金](https://juejin.im/post/59c60691518825396f4f71a1)

### 视频

- :tv: [DOM 探索之基础详解篇 —— 慕课网](https://www.imooc.com/learn/488)
- :tv: [DOM 事件探秘 —— 慕课网](https://www.imooc.com/learn/138)
- :tv: [jQuery 基础(二)DOM 篇 —— 慕课网](https://www.imooc.com/learn/530)
- :tv: [JS 操作 DOM 对象属性和方法 —— 爱奇艺](http://www.iqiyi.com/w_19rr19s08l.html)

**[:arrow_up: 返回目录](#目录)**

---

## 22. new 与构造函数, instanceof 与实例

### 文章

- :book: [构造函数与 new 命令 —— 阮一峰](http://javascript.ruanyifeng.com/oop/basic.html)
- :book: [Javascript 面向对象编程（二）：构造函数的继承 —— 阮一峰](http://www.ruanyifeng.com/blog/2010/05/object-oriented_javascript_inheritance.html)
- :book: [完整原型链详细图解(构造函数、原型、实例化对象) —— CSDN](https://blog.csdn.net/SpicyBoiledFish/article/details/71123162)
- :book: [JavaScript 中构造函数与 new 操作符的实例详解 —— PHP 中文网](http://www.php.cn/js-tutorial-376246.html)
- :book: [构造函数、实例、原型、原型链之间的关系 —— CSDN](https://blog.csdn.net/yin_991/article/details/80954453)
- :book: [深入理解 JS—instanceof 和原型链 —— CSDN](https://blog.csdn.net/cecilia620/article/details/71158048)
- :book: [前端基础进阶（九）：详解面向对象、构造函数、原型与原型链 —— 简书](https://www.jianshu.com/p/15ac7393bc1f)
- :book: [js 用 new 实例化对象与直接调用的 this 的区别 —— 简书](https://www.jianshu.com/p/60ffc4831bff)
- :book: [JavaScript 并非所有的东西都是对象 —— justjavac](http://justjavac.com/javascript/2012/12/22/javascript-values-not-everything-is-an-object.html)
- :book: [JavaScript instanceof 运算符深入剖析 —— IBM](https://www.ibm.com/developerworks/cn/web/1306_jiangjj_jsinstanceof/)

### 视频

- :tv: [改良版的构造函数 —— 乐视](http://www.le.com/ptv/vplay/27766889.html)

**[:arrow_up: 返回目录](#目录)**

---

## 23. 原型继承与原型链

### 文章

- :book: [继承与原型链 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)
- :book: [构造函数、原型与原型链 —— github](https://github.com/bigdots/blog/issues/1)
- :book: [原型及原型链 —— github(1269 Star)](https://github.com/stone0090/javascript-lessons/tree/master/2.5-Prototype)
- :book: [理清 javascript 中的面向对象(一) 原型继承 —— SegmentFault](https://segmentfault.com/a/1190000004282206)
- :book: [JavaScript：继承和原型链(译) —— justjavac](http://justjavac.com/2015/12/09/inheritance-and-the-prototype-chain.html)
- :book: [三张图搞懂 JavaScript 的原型对象与原型链 —— 博客园](http://www.cnblogs.com/shuiyi/p/5305435.html)
- :book: [一张图让你搞懂 JavaScript 的继承与原型链 —— CSDN](https://blog.csdn.net/the__apollo/article/details/76774698)
- :book: [JS 高级--原型链(一看就懂，但 18 岁以下请绕道) —— CSDN](https://blog.csdn.net/xiaotao_css/article/details/72782416)
- :book: [原型继承 —— 廖雪峰](https://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000/0014344997013405abfb7f0e1904a04ba6898a384b1e925000)
- :book: [JS 原型链与继承别再被问倒了 —— 掘金](https://juejin.im/post/58f94c9bb123db411953691b)
- :book: [征服 JavaScript 面试系列：类继承和原型继承的区别 —— 掘金](https://juejin.im/entry/5885db221b69e600592253e7)
- :book: [JavaScript 深入之从原型到原型链 —— 冴羽](https://github.com/mqyqingfeng/Blog/issues/2)
- :book: [深入理解 JavaScript 原型与闭包 —— 王福朋](https://www.cnblogs.com/wangfupeng1988/p/3977924.html)

### 视频

- :tv: [JS 高级-07-原型链继承 —— 乐视](http://www.le.com/ptv/vplay/27552753.html)
- :tv: [JS 原型对象和原型链简介 —— 腾讯视频](https://v.qq.com/x/page/b0511nwa7d3.html)

**[:arrow_up: 返回目录](#目录)**

---

## 24. Object.create 和 Object.assign

### 文章

- :book: [Object.create —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/create)
- :book: [Object.assign —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
- :book: [Object.create vs Object.assign —— 慕课网手记](https://www.imooc.com/article/17591)
- :book: [JS 中的 Object.assign()、Object.create()、Object.defineProperty() —— CSDN](https://blog.csdn.net/DeepLies/article/details/52915143)
- :book: [es6 中 object.create()和 object.assign() —— 风信子博客](http://www.onlyfordream.cn/2018/03/19/es6%E4%B8%ADobject-create%E5%92%8Cobject-assign/)
- :book: [Object-Assign-Deep —— github](https://github.com/saikojosh/Object-Assign-Deep)

**[:arrow_up: 返回目录](#目录)**

---

## 25. 工厂函数和类

### 文章

- :book: [类 —— MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Classes)
- :book: [类和实例 —— 廖雪峰](https://www.liaoxuefeng.com/wiki/001374738125095c955c1e6d8bb493182103fac9270762a000/00138682004077376d2d7f8cc8a4e2c9982f92788588322000)
- :book: [Javascript 定义类（class）的三种方法 —— 阮一峰](http://www.ruanyifeng.com/blog/2012/07/three_ways_to_define_a_javascript_class.html)
- :book: [【译】ES6 的工厂函数 —— 掘金](https://juejin.im/post/59c8c8756fb9a00a681ae5bd)
- :book: [JavaScript 创建对象之单例、工厂、构造函数模式 —— 掘金](https://juejin.im/entry/587992c961ff4b0065edf1ff)

**[:arrow_up: 返回目录](#目录)**

---

## 26. 设计模式

### 文章

- :book: [JavaScript 设计模式 —— 掘金](https://juejin.im/post/59df4f74f265da430f311909)
- :book: [学用 JavaScript 设计模式 —— 极客学院](http://wiki.jikexueyuan.com/project/javascript-design-patterns/)
- :book: [[面试专题]JS 设计模式 —— SegmentFault](https://segmentfault.com/a/1190000010914032)
- :book: [JavaScript Patterns 中译本 —— github](https://github.com/lxj/javascript.patterns)

### 视频

- :tv: [HTML5 课程大纲 2-11JS 设计模式](https://tv.sohu.com/v/dXMvMjQwNzYwNzQ4Lzg5NzM2MDA3LnNodG1s.html)

**[:arrow_up: 返回目录](#目录)**

---

## 27. Memoization

### 文章

- :book: [JavaScript Memoization —— 司徒正美](https://www.cnblogs.com/rubylouvre/archive/2009/08/06/1540678.html)
- :book: [memoization 提升递归效率 —— 博客园](https://www.cnblogs.com/yingshuizy/p/4517102.html)
- :book: [如何提升 JavaScript 的递归效率 —— 51CTO](http://developer.51cto.com/art/201010/231513.htm)
- :book: [JavaScript 高级技巧 Memoization —— SegmentFaut](https://segmentfault.com/a/1190000016703106)

**[:arrow_up: 返回目录](#目录)**

---

## 28. 纯函数, 函数副作用和状态变化

### 文章

- :book: [纯函数(Pure Function) —— React.js 小书](http://huziketang.mangojuice.top/books/react/lesson32)
- :book: [JavaScript Functional Programming：纯函数 —— 宁皓网](https://ninghao.net/blog/4634)
- :book: [js 函数的副作用分析 —— 脚本之家](https://www.jb51.net/article/28079.htm)
- :book: [如何使用纯函数式 JavaScript 处理脏副作用 —— 掘金](https://juejin.im/post/5b82bdb351882542e241ed32?utm_medium=hao.caibaojian.com&utm_source=hao.caibaojian.com)
- :book: [原生 JavaScript 实现 state 状态管理系统 —— 博客园](http://www.cnblogs.com/zhangycun/p/9403335.html)
- :book: [JavaScript 函数式编程 —— @BuptStEve](https://github.com/BuptStEve/blog/issues/10)

**[:arrow_up: 返回目录](#目录)**

---

## 29. 耗性能操作和时间复杂度

### 文章

- :book: [时间复杂度 O(log n) 意味着什么？ —— 掘金](https://juejin.im/entry/593f56528d6d810058a355f4)
- :book: [算法的时间复杂度和空间复杂度 —— 掘金](https://juejin.im/entry/5a49f7d36fb9a0450a67b269)
- :book: [算法（一）时间复杂度 —— 掘金](https://juejin.im/post/58d15f1044d90400691834d4)
- :book: [Big O Search Algorithms in JavaScript —— Bradley Braithwaite](http://www.bradoncode.com/blog/2012/04/big-o-algorithm-examples-in-javascript.html)
- :book: [Time Complexity Analysis in JavaScript — Jennifer Bland](https://www.jenniferbland.com/time-complexity-analysis-in-javascript/)

**[:arrow_up: 返回目录](#目录)**

---

## 30. JavaScript 引擎

### 文章

- :book: [javascript 引擎 —— 百度百科](https://baike.baidu.com/item/javascript引擎/5356108)
- :book: [V8(JavaScript 引擎) —— 百度百科](https://baike.baidu.com/item/V8/6178125)
- :book: [图解搞懂 JavaScript 引擎 Event Loop —— 掘金](https://juejin.im/post/5a6309f76fb9a01cab2858b1)3
- :book: [V8 JavaScript 引擎：高性能的 ES2015+ —— justjavac](https://segmentfault.com/a/1190000010819020)
- :book: [10 分钟理解 JS 引擎的执行机制 —— SegmentFaut](https://segmentfault.com/a/1190000012806637)
- :book: [V8 javascript 引擎 —— 博客园](https://www.cnblogs.com/weirdoQi/p/6609811.html)

**[:arrow_up: 返回目录](#目录)**

---

## 31. 二进制, 十六进制, 十进制, 科学记数法

### 文章

- :book: [二、八、十、十六进制转换(图解篇) —— 博客园](http://www.cnblogs.com/gaizai/p/4233780.html)
- :book: [JavaScript 读写二进制数据 —— 掘金](https://juejin.im/post/5b93dadaf265da0a857a58a3)

### 视频

- :tv: [二进制、十进制、十六进制互相转化很难吗？ —— 百度视频](http://baishi.baidu.com/watch/7873060963471478456.html)

**[:arrow_up: 返回目录](#目录)**

---

## 32. 偏函数, 柯里化, Compose 和 Pipe

### 文章

- :book: [Javascript 函数式编程之偏函数 —— CSDN](https://blog.csdn.net/qq_42129063/article/details/81874314)
- :book: [JavaScript 专题之偏函数 —— SegmentFault](https://segmentfault.com/a/1190000010686144)
- :book: [柯里化和偏函数有什么区别？ —— SegmentFault](https://segmentfault.com/q/1010000008626058)
- :book: [Javascript 偏函数与柯里化 —— CSDN](https://blog.csdn.net/neweastsun/article/details/75947785)
- :book: [柯里化(curry) —— JS 函数式编程指南](https://llh911001.gitbooks.io/mostly-adequate-guide-chinese/content/ch4.html)
- :book: [代码组合(compose) —— JS 函数式编程指南](https://llh911001.gitbooks.io/mostly-adequate-guide-chinese/content/ch5.html)
- :book: [关于 javascript 函数式编程中 compose 的实现 —— SegmentFault](https://segmentfault.com/a/1190000008394749)
- :book: [实现 compose 的五种思路 —— SegmentFault](https://segmentfault.com/a/1190000011447164)
- :book: [JavaScript 函数式编程之函数组合函数 compose 和 pipe 的实现 —— SegmentFault](https://segmentfault.com/a/1190000015102804)
- :book: [JavaScript 轻量级函数式编程-第 4 章:组合函数 ——掘金](https://juejin.im/post/59a62f3d6fb9a0248363fd9d#comment)
- :book: [JavaScript 函数式编程（二） —— @BuptStEve](https://github.com/BuptStEve/blog/issues/11)

**[:arrow_up: 返回目录](#目录)**

---

## 33. 代码整洁之道

### 文章

- :book: [[译] JavaScript 代码整洁之道 —— 边城](https://www.zcfy.cc/article/clean-code-javascript-readme-md-at-master-ryanmcdermott-clean-code-javascript-github-2273.html)
- :book: [Javascript 编程风格 —— 阮一峰](http://www.ruanyifeng.com/blog/2012/04/javascript_programming_style.html)
- :book: [重构 - 代码整洁之道 —— 掘金](https://juejin.im/post/5a5b2a5c6fb9a01cbc6e59f9)
- :book: [让你的代码更简短，更整洁，更易读的 ES6 小技巧 —— 掘金](https://juejin.im/post/5a7d71836fb9a063435ecf51)
- :book: [Web 前端：11 个让你代码整洁的原则 —— 伯乐在线](http://blog.jobbole.com/23617/)
- :book: [Clean Code concepts adapted for JavaScript —— ryanmcdermott](https://github.com/ryanmcdermott/clean-code-javascript)

<br>

**[:arrow_up: 返回目录](#目录)**

---
