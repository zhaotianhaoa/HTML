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
## 13.```<h1>~<h6>```-标题标签
  * Headline - 标题
  * 用于显示6层文字大小不同的标题
## 14.```<ol>```-有序列表标签
  * ol (order list) - 有序列表
  * li (list)       - 列表
  * 表示多个有序列表项，通常渲染为有带编号的列表。
  ```html
<ol start="1">
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ol>
  ```
## 15.```<ul>```-无序列表标签
  * unorder list 无序列表,显示小圆点
  ```html
<ul>
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ul>
  ```
## 16.```<img>```-图片标签
  * image - 图像
  ```html
<img src="my.jpeg">
  ```
## 17.```<video>```-视频标签
  * video - 视频
  * HTML5 新增特性
  ```html
<video src="foo.mp4">
  <track kind="subtitles" src="foo.en.vtt" srclang="en" label="English">
</video>
  ```
## 18.```<table>```-表格标签
  * table - 表格
  * tr(table row) - 表格行
  * td(table data)- 表格数据单元
  ```html
<table>
  <tr>
    <td>1</td>
    <td>2</td>
  </tr>
  <tr>
    <td>3</td>
    <td>4</td>
  </tr>
</table>
  ```
## 19.```<form>```-表单标签
  * form - 表单
  * 表示了文档中的一个区域，这个区域包含有交互控制元件，用来向web服务器提交信息。
  * input 输入
  * label 标签
  * type 类型
  * submit 提交
  ```html
<form action="">
  <label for="GET-name">Name:</label>
  <input id="GET-name" type="text" name="name">
  <input type="submit" value="Save">
</form>
  ```
## 20.```<input>```-输入标签
  * 能够输入的占位符
  * type属性有几种：button（按钮）radio（单选框）checkbox（多选框）file（文件上传）password（密码输入框）submit（提交按钮）text（单纯文字）
  ```html
<fieldset>
    <legend>Input</legend>
    <form>
        <div>
            <label for="display-name"> Name:
                <span class="warning">*(Allows only letters.)</span> 
            </label>
            <input type="text" id="display-name" name="ip-display"
                   pattern="[A-Za-z\s]+"
                   maxlength="5" minlength="2" value="Aa" required />
            <span></span>
        </div>
        <div>
            <label for="readonly-ip">ReadOnly:</label>
            <input type="text" id="readonly-ip" name="ip-readonly"
                   placeholder="I'm read only." readonly />
        </div>
        <div>
            <label for="disabled-ip">Disabled:</label>
            <input type="text" name="ip-disabled"
                   id="disabled-ip"
                   value="I am disabled"
                   disabled />
        </div>
        <div>
            <input type="submit" class="submit" value="Submit" />
        </div>
        
    </form>
</fieldset>

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
