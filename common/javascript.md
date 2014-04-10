# Basics
参考Google的[JavaScript Style Guide](http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)，以下是需要特别注意的几点。

## 特别的
- 变量要经过`var`关键字声明，不能直接使用；

- 变量、函数名、属性名采用驼峰性命名方式，首字母小写，作为构造函数的函数名首字母大写；

```javascript
/* Not recommended */
var var_name=1;
var funName=function(){
    this.prop=1;
};
function funName(){
    this.prop=1;
}

/* Recommended */
var varName=1;  //驼峰式命名
var FunName=function(){ //构造函数变量名首字母大写
    this.prop=1;
};
function Function(){    //构造函数名首字母大写
    this.prop=1;
}
```

- 每条js语句后不要丢失`;`，函数声明后不需要追加`;`

```javascript
/* Not recommended */
var varName=1

var funName=function(){
}

function funName(){
};

/* Recommended */
var varName=1;

var funName=function(){
};

function funName(){
}
```


