# 本周任务 #
1. 面向对象相关知识
2. 复习canvas相关知识

# 期望达成 #
1. 了解对象的创建方式(工厂模式、构造函数模式、原型模式)
2. 知道什么是字面量，知道原型的动态性，知道什么是原型对象什么是实例
3. 知道什么是继承，了解原型链相关知识
4. 能够使用面向对象的方法操作canvas

# 参考资料 #

  自行阅读《javascript高级程序设计》第6章

# 本周作业 #
1. 构建一个虚拟的家庭，帮助理解继承和原型的动态性
  - 父亲和母亲是两个原型对象
  - 女儿和儿子是继承了父亲或母亲部分外貌特征和能力的对象实例(假设如果父亲会武术，儿子一出生也会)
  - 设想某一天父亲学会新技能，儿子/女儿并不能立即get
  - 某一天母亲烫了卷发，儿子/女儿发型特征并没有变化
  - 构造符合上述约束条件的对象和实例
  - 在此基础上构造更多特征以充分理解相关概念

  下面是一个简单的例子：
  ```javascript
  function Father() {
	   this.eye = 'blue',
	   this.nose = 'big'
  }
  Father.prototype = {
     constructor: Father,
	   kongfu: function() {
	     alert('I have ever learnt it from Bruce Lee!');
	   }
  }

  function Son(eye) {
	   Father.call(this, eye);
     this.nose = 'small';
  }
  Son.prototype = new Father();
  Son.prototype.constructor = Son;

  var son = new Son();
  son.kongfu(); // alert('I have ever learnt it from Bruce Lee!');

  Father.prototype.eye = 'black';
  console.log(son.eye); // blue
  ```
2. 使用面向对象的方法重写你的"屌丝追女神"游戏(没写过，那从头开始吧~)
