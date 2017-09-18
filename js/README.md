# js相关

## js的特点

- 弱类型:`var a=1; a='124'`
- 解释执行，脚本语言
- 宿主环境一般是浏览器，现在也可以运行在服务器端（node），得益于js引擎的发展
- 特有的原型链
- JavaScript 中的变量是没有类型的，只有值才有

## 基本语法

JavaScript是EMCAScript标准的一种实现，是一种解释性的动态语言，在js里数据类型是动态的，意味着可以在运行时改变变量的数据类型，变量的数据类型也只有在运行时才能决定。

也因为可以动态改变变量的类型，所以也容易出现一些不可预知的错误，导致代码可维护性降低。所以在编码的过程中应该尽量避免。

### 基本数据类型
首先，在JavaScript里，一切皆对象。typeof运算符能识别以下6种数据类型：

- 值类型：
    + `typeof 1`:number
    + `typeof ''`:string
    + `typeof true`:boolean
    + `typeof function f(){}`:function
    + `typeof undefined`:undefined
- 引用类型
    + object

其他的Array，null，正则表达式都是object类型

但是，ECMAScript标准定义了7种数据类型（ES56种，ES6新增了Symble类型）：
- null
- undefined
- number
- string
- boolean
- object
- symbol

#### null

- 变量定义未初始化则为null
- `null === null // true`
- `null === false // true`
- `Object.toString.call(null) === '[Object Null]'`
- `typeof null === 'object'`这是JavaScript实现的一个bug

#### undefined
- 变量不存在则为undefined
- `undefined === false // true`
- undefined可以被重新定义，undefined = 1；
- `Object.toString.call(undefined) === '[Object Undefined]'`

#### Object 对象

js里的其他对象都继承自object对象，object对象是其他一切对象的祖先，任何一个对象沿着原型链往上找，最终找到的是object对象，object对象的原型对象是null.

Object对象的一些方法：

- `Object.keys`
- `Object.values`
- `Object.assign(es6)`
- `Object.defineProperty`
- `Object.defineProperties`
- `Object.toString`

### 语句和表达式

和其他语言类型，js里也有语句和表达式，包括：
- 变量定义
- 赋值语句
- 条件判断语句
- 循环语句
- 函数表达式
- 逻辑表达式
- 立即执行表达式

### 函数

在js里函数是一等公民，意味着：
- 1.函数也是对象，可以作为变量
- 2.函数可以作为函数的参数，也可以作为返回值
- 3.可以在函数内部定义函数，形成闭包

### 作用域链

作用域链其实就是当前语句执行的上下文环境中能访问到的变量所组成的链，在ES6之前js里只有全局作用域和函数作用域，没有块级作用域。
在访问某个变量的时候，先在当前函数的作用域中查找，如果找不到，则在函数的调用栈里找，如果找不到，则继续递归，直到到达全局作用域，如果在全局作用域也找不到这个变量，则返回undefined

- 可以用立即执行表达式模拟块级作用域
- with语句可以改变变量查找的上下文，降低效率
- 编码时，应尽量避免在作用域链上多级查找变量，缓存多次用到的全局变量

#### 作用域链，执行环境，函数对象，活动对象是什么？

### 原型链

### 声明提升

## 宿主环境

即JS的执行环境，主要是浏览器和nodejs
### 浏览器

#### 几大引擎

#### BOM对象

#### DOM

### nodejs

## 周边扩展

### coffeescript

### typescript

### ES6，7，8

## 相关工具

### eslint

### uglifyjs

## 相关书籍

## 框架和库

### 库

#### jQuery

#### loadsh

#### underscore

#### requirejs

#### seajs

### 框架

#### backbone

#### emberjs

#### vue

#### moon

#### react

#### anu

#### angularjs



