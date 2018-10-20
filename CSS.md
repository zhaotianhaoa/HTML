# CSS基本用法

### CSS基本语法
* 选择器{属性：值; 属性：值}
* HTML自有的标签选择器
```css
标签名{属性：值}
```
* 自定义CLASS样式选择器
```css
.自定义样式{属性：值}
```
* 定义事件发生属性的语法
```css
选择器：事件{属性：值}
```
* 例如鼠标悬浮事件：
```css
a:hover{font-size:x-large}
```
* 其他的类似的事件还有:
```css
a:link{color:#fff}  未访问时的状态（鼠标点击前显示的状态）
a:hover{color:#fff}  鼠标悬停时的状态
a:visited{color:#fff}  已访问过的状态（鼠标点击后的状态）
a:active{color:#fff}  鼠标点击时的状态
a:focus{color:#fff}  点击后鼠标移开保持鼠标点击时的状态（只有在<a href="#"></a>时标签中有效）
```
    
### CSS选择器分组
* 逗号隔开的意思是是每一个选择器都有身体里面的属性
```css
h1,h2,h3,h4,h5,h6 {
  color: green;
  }
```

### 选择器派生，也就是爷爷父亲孙子
* 派生选择器之间用空格隔开
```css
body .mycss h1{
    color:#ffffff
} 
```
### id选择器
* 开头用#代表id选择器
```css
#red {color:red;}
```
### id选择器和派生选择器组合
```css
#sidebar p {
	font-style: italic;
	text-align: right;
	margin-top: 0.5em;
	}
```
### CSS属性选择器
* 下面的例子为带有 title 属性的所有元素设置样式：
```css
[title]
{
color:red;
}

input[type="text"]
{
  width:150px;
  display:block;
  margin-bottom:10px;
  background-color:yellow;
  font-family: Verdana, Arial;
}

input[type="button"]
{
  width:120px;
  margin-left:35px;
  display:block;
  font-family: Verdana, Arial;
}
```

# CSS的盒子模型
    * http://www.w3school.com.cn/css/css_boxmodel.asp
```css
h1{margin:10px 0.25em 2ex 20%;}
h1{padding:10px 0.25em 2ex 20%;}
上 右 下 左 ，先是上然后四个值顺时针转一圈
````
# CSS定位 position属性
  * 绝对定位 position: absolute 相对于网页页面的左上角来定位的
  * 相对定位 position: relative 相对于某一个网页元素定位的
  * 浮动定位 float：left,right,center,inherit(继承父亲的float),none(不浮动)
    http://www.w3school.com.cn/css/css_positioning.asp
##### position 属性值的含义：
* static
元素框正常生成。块级元素生成一个矩形框，作为文档流的一部分，行内元素则会创建一个或多个行框，置于其父元素中。
* relative
元素框偏移某个距离。元素仍保持其未定位前的形状，它原本所占的空间仍保留。
* absolute
元素框从文档流完全删除，并相对于其包含块定位。包含块可能是文档中的另一个元素或者是初始包含块。元素原先在正常文档流中所占的空间会关闭，就好像元素原来不存在一样。元素定位后生成一个块级框，而不论原来它在正常流中生成何种类型的框。
* fixed
元素框的表现类似于将 position 设置为 absolute，不过其包含块是视窗本身。
