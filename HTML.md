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
<head>
  <link href="./index.css" rel="stylesheet">
</head>
```

## 6.```<style>```-样式标签
  * 用于链接内部CSS（层叠样式表）， 例如：
```html
<head>
   <style type="text/css">
   body 
   {
     color:red;
     font:宋体
   }
   </style>
</head>
```

## 7.```<meta>```-元数据标签
  * 表示那些不能由其它HTML元相关元素 (```<base>, <link>, <script>, <style>, <title>```) 之一表示的任何元数据信息.
  ```html
<head>
  <meta charset="utf-8">
</head>
  ```
## 8.```<base>```-URL基准标签
  * 指定用于一个文档中包含的所有相对URL的基本URL。一份中只能有一个
  ```html
<head>
  <base href="http://www.example.com/">
</head>
  ```
## 9.```<script>```-脚本标签
  * 用于嵌入或引用可执行脚本，属于元数据
  ```html
<head>
  <!-- HTML4 and (x)HTML -->
  <script type="text/javascript" src="javascript.js">

  <!-- HTML5 -->
  <script src="javascript.js"></script>
</head>
  ```
#显示数据和内容类的标签
## 10.```<p>```-段落标签
  * paragraph - 段落
  * 用于显示文字
  * 标签的 align 属性已被弃用，请不要使用。
  * 使用CSS margin属性去改变段落之间的间隙，不要在段落之间插入空的段落元素或者<br>元素。

## 11.```<a>```-地址标签
  * adress - 地址, 锚元素
  * ```<a>``` 元素  (或锚元素) 可以创建一个到其他网页、文件、同一页面内的位置、电子邮件地址或任何其他URL的超链接。
  * href(超链接地址)属性
#### i. 链接到外部网页某个地址
  ```html
<a href="http://www.mozilla.com/">
点我跳到链接地址
</a>
  ```
#### ii. 链接到本页面内的某个属性
  ```html
<a href="#属性">
点我跳到页面链接
</a>
  ```
## 12.```<hr>```-分割线hr标签
  * Horizontal Rule 水平分割规则
  * 显示一条水平分割线
  ```html
<p>This is the first paragraph of text. This is the first paragraph of text.
  This is the first paragraph of text. This is the first paragraph of text.</p>

<hr>

<p>This is second paragraph of text. This is second paragraph of text.
  This is second paragraph of text. This is second paragraph of text.</p>
  ```
## 13.``````-标签
  * 
  ```html
  ```
## 14.``````-标签
  * 
  ```html
  ```
## 15.``````-标签
  * 
  ```html
  ```
## 16.``````-标签
  * 
  ```html
  ```
## 17.``````-标签
  * 
  ```html
  ```
## 18.``````-标签
  * 
  ```html
  ```
## 19.``````-标签
  * 
  ```html
  ```
## 20.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```
## 7.``````-标签
  * 
  ```html
  ```

