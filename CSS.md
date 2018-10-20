# CSS基本用法

### 1.CSS语法
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
例如鼠标悬浮事件：
```css
a:hover{font-size:x-large}
```
* 其他的类似的事件还有:
1. a:link{color:#fff}  未访问时的状态（鼠标点击前显示的状态）
2. a:hover{color:#fff}  鼠标悬停时的状态
3. a:visited{color:#fff}  已访问过的状态（鼠标点击后的状态）
4. a:active{color:#fff}  鼠标点击时的状态
5. a:focus{color:#fff}  点击后鼠标移开保持鼠标点击时的状态（只有在<a href="#"></a>时标签中有效）

    
### 2.CSS
