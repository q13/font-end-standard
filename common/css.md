# Basics
采用Google的[HTML/CSS Style Guide](http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml)，以下是需要特别注意的几点。

## 特别的
- ### 不允许出现包含大写字母的css选择符

```css
/* Not recommended */
.clsSelector {
    font-size: 13px;
    color: red;
}
```
```css
/* Recommended */
.cls-selector {
    font-size: 13px;
    color: red;
}
```

- `{`应该在css选择符后，中间用空格隔开（可选），采用多行书写方式，`}`不能和`{`处于同一行

```css
/* Not recommended */
.cls-selector1, .cls-selector2
{ font-size: 13px; color: red; }
```
```css
/* Recommended */
.cls-selector1,
.cls-selector2 {
    font-size: 13px;
    color: red;
}
```

- 每条css声明后用`;`结尾

/* Not recommended */
.cls-selector {
    font-size: 13px;
    color: red
}
```
```css
/* Recommended */
.cls-selector {
    font-size: 13px;
    color: red;
}
```

- 忽略`0`后面的单位

/* Not recommended */
.cls-selector {
    font-size: 0px;
    color: red;
}
```
```css
/* Recommended */
.cls-selector {
    font-size: 0;
    color: red;
}
```

- 对于一些css3的声明，一般不需要写私有前缀，留给预编译工具去解决这个问题

/* Not recommended */
.cls-selector {
    -moz-border-radius: 4px;
    -webkit-border-radius: 4px;
    border-radius: 4px;
}
```
```css
/* Recommended */
.cls-selector {
    border-radius: 4px;
}
```
