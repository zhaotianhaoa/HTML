# HTML的基础知识总结：
* 备注：这个工程总结了所有HTML的基本知识

# HTML所有标签的英文中文对照表
## 1.```<HTML>```  -根标签
  * HTML - Hyper Text Markup Language:超级文本标记语言
  * HTML是网页语言的根元素,树形结构的最顶端。

## 2.```<head>``` -头部标签
  * 包含所有的文档元数据```<meta>```，包括脚本（JS）或样式表(CSS)的链接或内容。
  
## 3.```<title>```-标题标签
  * 文档的标题，将显示在浏览器的标题栏或标签页上。该元素只能包含文本，包含的标签不会被解释。
  
## 4.```<body>``` -身体标签
  * 代表 HTML 文档的内容。在网页中只能有一个 ```<body>``` 元素。
  
## 5.```<link>``` -链接标签
  * 用于链接外部CSS（层叠样式表）, 例如链接index.css
```html
  <link href="./index.css" rel="stylesheet">
```

## 6.```<style>```-样式标签
  * 用于链接内部CSS（层叠样式表）， 例如：
```html
  <style type="text/css">
  body {
    color:red;
  }
  </style>
```

