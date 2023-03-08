弹性框布局模型 (flexbox) 是专为一维内容设计的布局模型。它擅长获取一组大小不同的项目，并为这些项目返回最佳布局。 
 
父项属性：  
* flex-direction：决定主轴方向。当我们设置该值为row，那么侧轴方向就是column。
* justify-content：设置子项沿主轴的分布方式。
* align-items：设置每一行子项沿侧轴的分布方式。
* align-content：将所有子项视为一个组，设置该组沿侧轴的分布方式。  

子项属性：  
* align-self：更改特定子项沿侧轴的分布方式。
* flex-basis：指定了 flex 元素在主轴方向上的初始大小。flex-basis 比width或者height具有更高的优先级。
* flex-grow：指定子项如何划分剩余空间。默认值为0，不划分剩余空间。
* flex-shrink：指定子项在空间不足时按多大的比例缩小。默认值为1，值为0时不缩放。

注意：当父盒子设为flex布局后，子元素的float、clear和vertical-align属性将失效，子元素中的元素会自动垂直居中。

查阅右侧链接[了解详细信息](https://www.joshwcomeau.com/css/interactive-guide-to-flexbox/)
查阅右侧链接[了解详细信息](https://web.dev/learn/css/flexbox/)