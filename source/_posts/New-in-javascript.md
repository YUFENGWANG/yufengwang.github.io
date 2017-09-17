---
title: New in javascript
date: 2016-11-21 10:15:06
tags: JS
---
## 语法
{% codeblock %}
new constructor[([arguments])]
{% endcodeblock %}
注：[]表示参数可选。

当 new Foo(...) 执行时，发生了下面三件事：
1. 创建了一个新对象，继承自Foo.prototype.
2. 调用Foo函数，this绑定到新创建的对象。
3. 如果构造函数内部没有显式返回一个对象的话，则返回这个新创建的对象，

