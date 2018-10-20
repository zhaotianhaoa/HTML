# CSS基本用法

### 1.CSS基本语法
* 选择器{属性：值; 属性：值}
* 1.HTML自有的标签选择器
```css
标签名{属性：值}
```
* 2.自定义CLASS样式选择器
```css
.自定义样式{属性：值}
```
* 3.定义事件发生属性的语法
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
    
### 2.CSS选择器分组
* 逗号隔开的意思是是每一个选择器都有身体里面的属性
```css
h1,h2,h3,h4,h5,h6 {
  color: green;
  }
```

### 3.选择器派生，也就是爷爷父亲孙子
* 派生选择器之间用空格隔开
```css
body .mycss h1{
    color:#ffffff
} 
```
### 4.id选择器
* 开头用#代表id选择器
```css
#red {color:red;}
```
### 5.id选择器和派生选择器组合
```css
#sidebar p {
	font-style: italic;
	text-align: right;
	margin-top: 0.5em;
	}
```
