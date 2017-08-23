### 2_HTML

> 准备工作：[下载Atom编辑器](https://atom.io/)

> 可以选择安装在Windows下或者虚拟机下，建议两边都安装上，
> 因为有时需要在不同的平台下进行开发

#### 2.0 调试HTML

打开文本编辑器后，我们可以通过新建HTML文件并且把写好的HTML文件在浏览器中打开
来查看HTML文件的效果。

有关文本编辑器，有很多实用的功能这里列举一些，还有很多供大家探索：

Atom快捷键：

如`shift+方向键`进行不需移动鼠标的选择，`ctrl+方向键`进行跨单词移动，
`ctrl+点击`进行多点编辑，`ctrl+/`快速注释，`ctrl+[`快速缩进等等

鉴于网上教程没找到合适的，可以根据file->settings
->keybindings ->search "editor" 查看全部快捷键

#### 2.1 HTML
HTML 相关教程：
http://www.w3school.com.cn/html/html_jianjie.asp

关注重点：
1. HTML文本格式化标签有哪些

2. 空标签

4. HTML 注释

5. HTML CSS

6. HTML 链接

7. HTML 图像

8. HTML 表格

9. HTML 块

10. HTML 类

11. HTML 布局（留到之后学习CSS的时候看）

12. HTML 头部

13. HTML 实体（字符实体）

14. HTML 表单（包括表单元素/输入类型/输入属性）


随堂问题：

1. 所有HTML元素都有开始标签和结束标签。错，空元素没有结束标签。

2. 在HTML中，可以使用`<img>`&emsp;标记向网页中插入GIF动画文件。

3. 请列举一个可以嵌套别的HTML元素的HTML元素——body元素

4. HTML对大小写是否敏感？ 否

5. `<a href="http://www.w3school.com.cn">This is a link</a>`这里href代表的意思是

6. `<hr/>` 标签在 HTML 页面中作用是：创建水平线。

7. HTML如何添加注释？

8. HTML如何查看源代码？

9. “改变所有 HTML 元素的样式的通用方法”的是哪个HTML属性？

10. `<del>`和`<ins>`分别代表什么？

练习题：

1.如果在catalog.htm中包含如下代码，则该HTML文档IE浏览器中打开后，用户单击此链接将(&emsp;&emsp;)。     

`<A HREF="#novel">小说</a>`

A. 使页面跳转到同一文件夹下名为“novel.html”的HTML文档

B. 使页面跳转到同一文件夹下名为“小说.html”的HTML文档

C. 使页面跳转到catalog.htm包含名为“novel”的锚记处

D. 使页面跳转到同一文件夹下名为“小说.html”的HTML文档中名为“novel”的锚记处<br/>

<br/>

2.分析下面的HTML代码片段，则选项中的说法正确的是（&emsp;&emsp;）。
```html
<table border="10">
  <tr> <td colspan=2 align="center">姓名</td></tr>
  <tr> <td rowspan=2 align="center">成绩</td><td align="center">语文</td></tr>
  <tr><td align="center">数学</td></tr>
<table>
```
A. 该表格共有2行3列  B. 该表格的宽度为10  C. “姓名”单元个跨2列

<br/>

3.以下说法正确的是（&emsp;&emsp;）

A. `<P>`标签必须以`</P>`标签结束

B. `<BR>`标签必须以`</BR>`标签结束

C. `<TITLE>`标签应该以`</TITLE>`标签结束

<br/>

4.以下说法正确的是（&emsp;&emsp;）。  

A. `<A>`标签是页面链接标签，只能用来链接到其他页面  

B. `<A>`标签是页面链接标签，只能用来链接到本页面的其他位置

C. `<A>`标签的src属性用于指定要链接的地址

D. `<A>`标签的href属性用于指定要链接的地址

<br/>

5.在HTML中，（&emsp;&emsp;）标签用于在网页中创建表单。

A. `<INPUT>`

B. `<SELECT>`

C. `<TABLE>`

D. `<FORM>`

<br>

6.阅读以下代码段，则可知（&emsp;&emsp;）。

```html
<INPUT type="text" name="textfield">  
<INPUT type="radio" name="radio" value="女">  
<INPUT type="checkbox" name="checkbox" value="checkbox">
<INPUT type="file" name="file">  
```
A. 上面代码表示的表单元素类型分别是：文本框、单选按钮、复选框、文件域

B. 上面代码表示的表单元素类型分别是：文本框、复选框、单选按钮、文件域

C. 上面代码表示的表单元素类型分别是：密码框、多选按钮、复选框、文件域

D. 上面代码表示的表单元素类型分别是：文本框、单选按钮、下拉列表框、文件域

<br>

7.在插入图片标签中，对插入的图片进行文字说明使用的属性是（）。  

A. name

B. id

C. src

D. alt

<br>

8.对于`<FORM  action=″URL″ method=*>`标签，其中*代表GET或（）。  

A. SET

B. PUT  

C. POST  

D. INPUT

<br>

9.HTML文件中，下面（）标签中包含了网页的全部内容。  

A. `<Center...</center>`  

B. `<pre...</pre>`  

C. `<Body...</Body> `

D. `<Br...</Br>`

<br>

10.超级链接元素A有很多属性，其中用来指明越级链接所指向的URL的属性是（）。  

A. href

B. herf

C. target

D. link
