# BFC: block formatting context(块级格式化上下文)
> w3c中关于[bfc](http://www.w3.org/TR/CSS2/visuren.html#block-formatting)的解释

阅读的两篇关于bfc解释的[bolg1](http://kayosite.com/block-formatting-contexts-in-detail.html)、[blog2](http://www.html-js.com/article/1866)  
## 触发条件 
> MDN中关于[bfc的触发条件](https://developer.mozilla.org/zh-CN/docs/Web/Guide/CSS/Block_formatting_context)

* 根元素或其它包含它的元素
* 浮动 (元素的 float 不为 none)
* 绝对定位元素 (元素的 position 为 absolute 或 fixed)
* 行内块 inline-blocks (元素的 display: inline-block)
* 表格单元格 (元素的 display: table-cell，HTML表格单元格默认属性)
* 表格标题 (元素的 display: table-caption, HTML表格标题默认属性)
* overflow 的值不为 visible的元素
* 弹性盒子 flex boxes (元素的 display: flex 或 inline-flex)

## 影响

* 阻止外边距折叠
* 可以包含浮动的元素(清浮动)
* 可以阻止元素被浮动元素覆盖(用于布局)