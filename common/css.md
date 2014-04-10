# Basics
采用Google的[HTML/CSS Style Guide](http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml)，以下是需要特别注意的几点。

## 特别的
- 不允许出现包含大写字母的css选择符

```css
/* Not recommended */
.clsSelector {

}
```
```css
/* Recommended */
.cls-selector {

}
```

- `{`应该在css选择符后，中间用空格隔开（可选），采用多行书写方式，`}`不能和`{`处于同一行

```css
/* Not recommended */
.cls-selector
{ font-size: 13px; color: red; }
```
```css
/* Recommended */
.cls-selector {
    font-size: 13px;
    color: red;
}
```
