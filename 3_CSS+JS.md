### 3_CSS+JS

#### 3.1 何为CSS?

CSS，(**C**ascading **S**tyle **S**heets)，即层叠样式表，定义如何显示 HTML 元素，就像 HTML 的字体标签和颜色属性所起的作用那样。**它的目的是为了解决内容与表现分离的问题。** 样式通常保存在外部的 .css 文件中。
通过仅仅编辑一个简单的 CSS 文档，外部样式表使你有能力同时改变站点中所有页面的布局和外观。

由于允许同时控制多重页面的样式和布局，CSS 可以称得上 WEB 设计领域的一个突破。作为网站开发者，你能够为每个 HTML 元素定义样式，并将之应用
于你希望的任意多的页面中。如需进行全局的更新，只需简单地改变样式，然后网站中的所有元素均会自动地更新。

#### 3.2 CSS教程
[教程地址](http://www.w3school.com.cn/css/css_jianjie.asp)

学习重点：
1. 外部样式表，内部样式表，内联样式分别是什么?

2. 如何创建CSS

2. 如果多个矛盾的样式指向同一个元素，会发生什么情况?如果有样式，会是什么样的样式?([CSS优先级](http://www.cnblogs.com/xugang/archive/2010/09/24/1833760.html))

3. 怎么把元素设为红色?

4. 如果希望`<p>`和`<h1>`是一个颜色的话，我该怎么做?

5. 希望`<h2>`的子元素变色，我该怎么做?

6. HTML文档中，同一个 id 能出现几次? 同一个 class 又能出现几次?

7. id选择器的标识是?class选择器的标识是?

8. `<img class='2nd' />`是合法的标签么?

4. 如何用CSS进行定位? **(选学)**

4. CSS语句`p.important {color:red;}`是什么意思?

5. 如何给一个元素添加两个以上的class?如何选择这些不止一个类的元素?

6. 后代选择器和子元素选择器的区别是什么?

7. 如何选择`任何元素的第一个子元素的 p 元素`?

8. `:hover`是什么意思?

#### 3.3 CSS3教程
惊不惊喜，意不意外?学了那么多CSS以后竟然还没学完。

[教程地址](http://www.w3school.com.cn/css3/)

学习重点——CSS 3动画效果:

##### 什么是 CSS3 中的动画？

动画是使元素从一种样式逐渐变化为另一种样式的效果。
您可以改变任意多的样式任意多的次数。
请用百分比来规定变化发生的时间，或用关键词 "from" 和 "to"，等同于 0% 和 100%。
0% 是动画的开始，100% 是动画的完成。
为了得到最佳的浏览器支持，您应该始终定义 0% 和 100% 选择器。

1. `规定动画完成一个周期所花费的时间`的属性是什么?

2. `-webkit-` `-moz-`这些标记有什么用途?

3. 请动手实践

#### 3.4 JS教程

JavaScript 是一种轻量级的编程语言。
JavaScript 是可插入 HTML 页面的 **编程代码**。
JavaScript 插入 HTML 页面后，可由所有的现代浏览器执行。
JavaScript 很容易学习。在网站编程中，
HTML 控制内容，CSS控制表现，JS控制逻辑。

然而，JS的书写困难导致在现代编程中使用JS是一件十分困难的事情，程序员们选取更加简单的方式书写JS是必然趋势。因此下面我们不讲接JS，而是讲解JS衍生出的JQuery，它极大地简化了JS。

[教程地址](http://www.w3school.com.cn/jquery/index.asp)

学习重点:

1. jQuery是一个JS库

2. 如何引入JQuery库?

3. 我想要隐藏被点击的元素，应该怎么做?

4. JQuery选择器如何工作?

5. 文档就绪函数有何作用?

6. JQ如何改变 HTML 元素的 CSS 属性？

7. JQ实现元素一个接一个淡入出现应该怎么做?

8. 阅读`JQuery效果`

9. JQ如何所选元素的文本内容？如何获取所选元素的内容？如何获得链接中 href 属性的值？

10. JQ如何在被选元素的结尾插入内容？

11. `after` `before`方法有何作用？

12. JQ如何删除元素?

13. Jquery CSS 操作

14. JQuery 遍历

#### 测试题
1.观察下面的代码,要是想实现CSS 3 从无到有的渐变效果的话，
图中横线处应该填写________
```css
@-webkit-keyframes fadeIn /* Safari 和 Chrome */
{
  0% {
  /*初始状态 不透明度为0*/
  }
  50% {
  /*中间状态*/
  }
  100% {
  ________ /*结尾状态*/
  }
}
```

2.下列关于选择器描述错误的是?

A. 后代选择器(li a)

B. 子选择器(li > a)

C. 伪类选择器(a:hover)

D. 相邻选择器（h1 + p）

<br/>

3.CSS是什么的缩写？（ ）

A. Colorful Style Sheets

B. Cascading Style Sheets

C. Creative Style Sheets

D. Computer Style Sheets

<br/>

4.访问外部样式表的正确的HTML代码是（ ）

A. `<style src="mystyle.css" />`

B. `<link rel="stylesheet" type="text/css" href="mystyle.css">`

C. `<stylesheet>mystyle.css</stylesheet />`

D. `<usecss file="mystyle.css" />`

<br/>

5.哪个是正确的CSS语法？（ ）

A. `{body;color:black}`

B. `body:color=black`

C. `{body:color=black(body}`

D. `body {color: black}`

<br/>

6.哪个HTML标签定义内部的样式表？（  ）

A. `<style>`

B. `<css>`

C. `<script>`

D. `<cssStyle>`

<br/>

7.下面哪一个是用来追加到指定元素的末尾的？

A、insertAfter() 

B、append() 

**C、appendTo()**

D、after() 

<br/>

8.在一个表单里，想要找到指定元素的第一个元素用_________实现，那么第二个元素用_________实现。 
考点：jquery的选择器 （first,eq(1)）

<br/>

9.为每一个指定元素的指定事件（像click）绑定一个事件处理器函数，下面哪个是用来实现该功能的？

A、trigger (type) 

B、bind(type)

C、one(type) 

D、bind 

<br/>

10.在jquery中指定一个类，如果存在就执行删除功能，如果不存在就执行添加功能，下面哪一个是可以直接完成该功能的？

A、removeClass() 

B、deleteClass() 

C、toggleClass() 

D、addClass() 
