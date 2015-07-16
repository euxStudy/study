# 本周任务
1. 编码规范了解

    我们来简单接触一些团队的编码规范，这不但能够规范我们的代码，而且可以让代码更加美观

    - 腾讯Alloyteam (http://alloyteam.github.io/CodeGuide/)
    - 百度EFE (https://github.com/ecomfe/spec)
    
    我们可以在以后的学习中尝试使用这些团队的编码规范去要求自己，向更加专业化的道路迈进

2. js基础（一）
    - 闭包
    - 事件
    - DOM
    - BOM

# 期望达成
1. 规范你的代码，至少你的代码要足够美观
2. 了解闭包，了解IIFE(立即执行函数表达式)
3. 了解函数中this的特点
4. 了解ie/其他浏览器的事件绑定、移除，知道什么是事件委派
5. 了解DOM的相关操作，能够简单实现jquery的选择器$()
6. 能够利用BOM进行浏览器的判定(userAgent)
7. 能够使用正则表达式进行简单的匹配
8. 自行查阅书籍学习可能用到的js函数方法

# 参考学习资料
- [阮一峰的网络日志-学习Javascript闭包(Closure)](http://www.ruanyifeng.com/blog/2009/08/learning_javascript_closures.html)
- [鸟哥：Javascript作用域原理](http://www.laruence.com/2009/05/28/863.html)
- [Javascript中this关键字详解](http://www.cnblogs.com/justany/archive/2012/11/01/the_keyword_this_in_javascript.html)
- [IIFE - 苏青 - ITeye技术网站](http://suqing.iteye.com/blog/1981591/)
- 《JavaScript高级程序设计》(eux群共享)事件、DOM、BOM部分
- [正则表达式30分钟入门教程](http://www.jb51.net/tools/zhengze.html)

# 本周作业
1. 写一份有关闭包和this的总结笔记
2. 构造能兼容所有浏览器的事件绑定/事件移除/取消默认事件的函数(请不要复制粘贴，手抄一遍也没有关系)
3. 构造能实现简单id/class/tag选取的$()方法
    ```javascript
    // 实现一个简单的Query
    function $(selector) {
        
    }
    
    // 可以通过id获取DOM对象，通过#标示，例如
    $("#adom"); // 返回id为adom的DOM对象
    
    // 可以通过tagName获取DOM对象，例如
    $("a"); // 返回第一个<a>对象
    
    // 可以通过样式名称获取DOM对象，例如
    $(".classa"); // 返回第一个样式定义包含classa的对象
    ```
    - Use only "getElementById"/"getElementsByTagName", methods like "getElementsByClassName"/"querySelectorAll" are not allowed.
    - Pay attention to the request "return the first element".
4. 知道如何使用userAgent进行浏览器的判定，自行学习了解其他BOM相关知识
   
    Write a funciton able to distinguish all kinds of browsers in PC.
5. 利用正则表达式进行表单验证

    Write a form checked by regular expression.

# Advance request
You can decide whether to do any of these exercises or not.

1. Write a full-screen-scroll plugin. Every time you scroll up/down with your mouse the window will move the distance which is its height.
2. Complete the following functions with regular expression or other native javascriipt methods:
  - trim()
  
    Remove the blank at the beginning or the end of an expression.
  - animate(element, attr, value)
  
    We all know "animate" method in jquery is very strong. However, when it comes to some attributes in CSS3, it doesn't work either. Let's create a function with "setTimeout" to manage animation in CSS3 attributes. Here we shall try only 1-2 attributes such as "rotate"/"scale". It is not complex at all, just try it.
3. Learn by yourself about Object in javascript and write a summary not shorter than 80 lines.
