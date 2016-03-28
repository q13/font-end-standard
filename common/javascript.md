# Basics
参考Google的[JavaScript Style Guide](http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)，以下是需要特别注意的几点。

## 特别的
- 遵循ES3语法[规范](http://www.ecma-international.org/publications/files/ECMA-ST-ARCH/ECMA-262,%203rd%20edition,%20December%201999.pdf), 对ES2015[规范](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-262.pdf)引入的新内容保留使用，当前约定可使用的ES2015新语法特性参照[Babel](https://babeljs.io/)支持的polyfill实现；

- 变量要经过`var`关键字声明，不能直接使用；

- 变量、函数名、属性名采用驼峰性命名方式，首字母小写，作为构造函数的函数名首字母大写；

```javascript
/* Not recommended */
var var_name = 1;
var funName = function () {
  this.prop = 1;
};
//or
function funName() {
  this.prop = 1;
}
var inst = new funName();

/* Recommended */
var varName = 1;  //驼峰式命名
var FunName = function () { //构造函数变量名首字母大写
  this.prop = 1;
};
//or
function FunName() {    //构造函数名首字母大写
  this.prop = 1;
}
var inst = new FunName();
```

- 每条语句后不要丢失`;`，函数声明后不需要追加`;`；

```javascript
/* Not recommended */
var varName = 1

var funName = function () {
}

function funName() {
};

/* Recommended */
var varName = 1;

var funName = function(){
};

function funName() {
}
```

- 使用JSDoc文档规范，参考[介绍](http://usejsdoc.org/)

```javascript
/* Recommended */
/**
 * Class making something fun and easy.
 * @param {string} arg1 An argument that makes this more interesting.
 * @param {Array.<number>} arg2 List of numbers to be processed.
 * @constructor
 * @extends {goog.Disposable}
 */
project.MyClass = function(arg1, arg2) {
  // ...
};

```

## 附录
- ES3规范下的保留字和关键词，参考[这里](http://www.w3schools.com/js/js_reserved.asp)

