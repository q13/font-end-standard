# Basics
采用Google的[HTML/CSS Style Guide](http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml)，以下是需要特别注意的几点。
## DTD方式
采用html5的头声明方式 `<!DOCTYPE html>`，DTD声明前不能有任何输出。
> 参考 [Henri Sivonen整理的DTD分析](https://hsivonen.fi/doctype/)

## Meta标签
需要引入的几个标签：
- `<meta charset="utf-8">`；
- `<meta http-equiv="X-UA-Compatible" content="IE=edge">`；
- `<meta name="viewport" content="width=device-width, initial-scale=1">`。

请弄清各自含义再使用。
>参考 http://stackoverflow.com/questions/14611264/x-ua-compatible-content-ie-9-ie-8-ie-7-ie-edge

## 编写方式
- 标签名(Tag name)、属性名(Attribute name)、属性值(Attribute value)采用小写字母，多单词属性(名/值)用`-`（中划线）连接；
- 保证页面内`id`值唯一；
- 对于表单元素的`name`属性，其值采用小写字母，多单词用`_`（下划线）连接；
- button标签需要指定对应的`type`值，image标签需要指定对应的`alt`值；
- 用于控制间隔的空格字符用`&nbsp;`实体字符代替；
- 属性值(Attribute value)用`"`（双引号）引用方式，不允许出现`'`（单引号）引用；

# Template
以下为一个html模版示例：

```html
<!doctype html>
<html>
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <title></title>
        <meta name="description" content="">
        <meta name="viewport" content="width=device-width, initial-scale=1">

        <!-- Place favicon.ico and apple-touch-icon(s) in the root directory -->

        <link rel="stylesheet" href="#">
        <script src="#"></script>
    </head>
    <body>
        页面内容区
    </body>
</html>
```



