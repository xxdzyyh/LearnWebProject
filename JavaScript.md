## JavaScript

JavaScript  用来指明网页的行为。

JavaScript 是 Web 的编程语言。

所有现代的 HTML 页面都使用 JavaScript。



[TOC]

### 使用javaScript

* 直接写在 `<script></script>`中间，脚本可被放置在 HTML 页面的 <body> 和 <head> 部分中。

  ```
  <!DOCTYPE html>
  <html>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <head>
  	<title>点击按钮弹出alert</title>
  </head>
  <body>
  <h3>点击弹出</h3>
  <button type="button" onclick="myButtonClicked()"> 点我 </button>
  <script type="text/javascript">	
  function myButtonClicked() {
  	alert("点我干什么？？？")
  }
  </script>
  </body>
  </html>
  ```

* 外部 js 文件

  ```
  // alert.html
  <!DOCTYPE html>
  <html>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <head>
    <title>点击按钮弹出alert</title>
  </head>
  <body>
  <h3>点击弹出</h3>
  <button type="button" onclick="myButtonClicked()"> 点我 </button>
  <script type="text/javascript" src="alert.js"></script>
  </body>
  </html>
  
  // alert.js
  function myButtonClicked() {
  	alert("点我干什么？？？")
  }
  
  ```

JavaScript 没有任何打印或者输出的函数。

### JavaScript 显示数据

JavaScript 可以通过不同的方式来输出数据：

- 使用 **window.alert()** 弹出警告框。
- 使用 **document.write()** 方法将内容写到 HTML 文档中。
- 使用 **innerHTML** 写入到 HTML 元素。
- 使用 **console.log()** 写入到浏览器的控制台。

> 请使用 document.write() 仅仅向文档输出写内容。 如果在文档已完成加载后执行 document.write，整个 HTML 页面将被覆盖。


```
<!DOCTYPE html>
<html>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
<body>
<h1>我的第一个 Web 页面</h1>
<p id="demo">我的第一个段落</p>
<script>
document.getElementById("demo").innerHTML = "段落已修改。";
</script>
</body>
</html>
```

### JavaScript 对象

```
var person = {firstName:"John",lastName:"Doe",id:5566}
// 重新定义变量，变量的值不会丢失
var person
console.log(person)
// {firstName:"John",lastName:"Doe",id:5566}

// 声明变量类型
var name = new String;
```

### Undefined 和 Null

Undefined 这个值表示变量不含有值。

可以通过将变量的值设置为 null 来清空变量。