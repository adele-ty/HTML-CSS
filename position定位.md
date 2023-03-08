# static
static是position的默认值。元素使用正常的布局行为，即元素在文档常规流中当前的布局位置，元素与元素之间不产生重叠。此时 top, right, bottom, left 和 z-index 属性无效。
# relative
定位基点是元素的默认位置（即static时的位置）。元素先放置在未添加定位时的位置，再在不改变页面布局的前提下调整元素位置，原来在正常文档流中的位置会继续占有。position:relative 对 table-*-group, table-row, table-column, table-cell, table-caption 元素无效。搭配top、bottom、left、right指定偏移的方向和距离。
# absolute
定位基点是非static定位的祖先元素。元素会被移出正常文档流，且不占有在正常文档流中的位置，周边元素不受影响。绝对定位的元素可以设置外边距（margins），且不会与其他边距合并。搭配top、bottom、left、right指定偏移的方向和距离。
# fixed
定位基点是浏览器窗口。元素会被移出正常文档流，且不占有在正常文档流中的位置，会创建新的层叠上下文。元素的位置在屏幕滚动时不会改变。
# sticky
定位基点是它的最近滚动祖先。该值总是创建一个新的层叠上下文。sticky生效的前提是，必须基于 top、right、bottom 和 left 的值进行偏移，偏移值不会影响任何其他元素的位置，不能省略，否则等同于relative定位，不产生"动态固定"的效果。原因浏览器把偏移值当作sticky的生效门槛。  
它的具体规则是，当页面滚动，父元素开始脱离视口时（即部分不可见），视口与sticky元素的距离小于偏移值就会达到生效门槛，relative定位自动切换为fixed定位；等到父元素完全脱离视口时（即完全不可见），fixed定位自动切换回relative定位。

注意：  
* 绝对定位的盒子无法通过margin: 0 auto; 设置水平居中，原因绝对定位的盒子脱标了。
* 行内元素添加绝对或固定定位，可以直接设置宽度和高度。块级元素添加绝对或固定定位，如果不给宽度或高度，默认大小是内容的大小。  
* 脱离标准流的元素不会引起外边距塌陷的问题。

参考文档[MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/position)  
参考文档[阮一峰-CSS定位详解](https://www.ruanyifeng.com/blog/2019/11/css-position.html)
