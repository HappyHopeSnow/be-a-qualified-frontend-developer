# 第3天：打通基本概念

> 《HTML5与CSS3基础教程》是一本很好的入门书籍，里面提到很多重要的基本概念和方法论。

## 传统的html学习方法

同学们，`<b>` 标签是用来对文字做加粗效果的，在编辑器里输入

    <b>我是粗体</b>

是不是看到文字加粗了呢？对的吧，那么下一个标签……

*如果第3天仅仅是这么收获，那就太 low 了。*

**注意：**这里不做所谓的好坏评论或者对比，这里只是回想一下第1天提到的学习基本原则。

> 要**说清楚它是什么，它不是什么，它和别的概念有什么异同**；然后就是**与它相关的方法论**，比如，**使用的时候需要注意什么，怎样使用是正确的，怎样使用是错误的，容易发生错误的地方是什么……**

## 浏览器是怎样工作的？
> 你写的 HTML/CSS/JS 究竟是怎么显示出来的？

想了解细节的朋友可以移步[这里](http://kb.cnblogs.com/page/129756/)。

下面是一个简化版本的回答：

- 答案因浏览器而异（凌乱~）
- 大致的过程如下：
   - 访问一个html页面；
   - 浏览器会根据 HTML规范 解析文本为 DOM 结构，该结构遵循 DOM 规范；
   - 这时会根据你定义的样式规则做 attach 操作；
   - 同样的，样式代码（CSS）也会根据 CSS规范 进行解析；
   - 浏览器根据 attach 的结果进行渲染，最后展示；
   - 你写入的 JS脚本 会由浏览器提供的 JS引擎 进行调用，操作 DOM接口 实现页面的各种效果。

## 基本概念
从上面的过程可以看出，需要了解的基本概念包括但不限于以下内容：

### DOM
> DOM= Document Object Model，文档对象模型，DOM可以以一种独立于平台和语言的方式访问和修改一个文档的内容和结构。
> DOM 可被 JavaScript 用来读取、改变 HTML、XHTML 以及 XML 文档。

- [W3 DOM规范](https://www.w3.org/TR/dom/)

### HTML
#### 历史
- HTML 2.0——1995年11月作为RFC 1866发布，在RFC 2854于2000年6月发布之后被宣布已经过时
- HTML 3.2——1997年1月14日，W3C推荐标准
- HTML 4.0——1997年12月18日，W3C推荐标准
- HTML 4.01（微小改进）——1999年12月24日，W3C推荐标准
- HTML 5——2014年10月28日，W3C推荐标准

> HTML4.01 是常见的版本。

#### 标准
- [W3 HTML4](https://www.w3.org/TR/html4/)标准
  - HEAD 与 BODY 是什么
  - 文本国际化
  - 段落、行、短语
  - 有序、无序列表
  - 表格
  - 链接
  - 对象、图像及小程序
  - 样式表：添加样式表、链接样式表、CSS
  - 对齐、字体样式、水平分割线
  - Frame
  - 表单：表单内的输入，文本字段、按钮、菜单等
  - 脚本
- [HTML5](https://www.w3.org/TR/html5/)标准
  - [HTML4与HTML5的区别](https://www.w3.org/TR/html5-diff/)：新标记，废弃的标记，标记的属性变更

### CSS
- [W3 CSS的所有标准](https://www.w3.org/standards/techs/css#w3c_all)

## 方法论
学习HTML有一个很关键的方法，叫做 **渐进增强（progressive enhancement)**。

维基百科上[这个词条](http://css-discuss.incutio.com/wiki/Progressive_Enhancement)的解释是：

- 对所有浏览器都能够显示内容；
- 所有浏览器都能够使用基本功能；
- 用极少的、[语义化标签](https://en.wikipedia.org/wiki/Semantic_HTML)，包含所有的内容；
- 通过 外部CSS 提供高级布局；
- 通过 外部链接JS 定义行为；
- 能够兼容用户浏览器的个性化配置。

总结一下：

> 不论结果展示是否有差异，关键是网站的内容是可访问的。
> 本质上，渐进增强背后的含义是共赢。

### 实际操作
实际操作过程中，

- 先用基础的标记定义网页的结构和内容;
- 根据需要通过 CSS 定义页面的展示；
   - 注意，这里可能会有不同浏览器兼容性的问题，可以通过 [CSS Filter](https://en.wikipedia.org/wiki/CSS_filter) 根据不同的浏览器对CSS进行过滤，以便于正确显示；
- 用 JS 操作 DOM API 达到需要的行为及效果。

### 好处
不但可以成功地实践 [将表现与内容分离](https://en.wikipedia.org/wiki/Separation_of_presentation_and_content) 这个设计原则，还可以更好地为网站做搜索引擎优化，即SEO。

### Demo
这里有一个在线展示 渐进增强 概念的示例：

- 示例：[http://slayeroffice.com/articles/wsag/](http://slayeroffice.com/articles/wsag/)

## 接下来的行动
操练书中的各种例子：[http://www.htmlcssvqs.com/8ed/examples/](http://www.htmlcssvqs.com/8ed/examples/)

这里的例子都理解了，html/CSS/JS的基础就OK了。


