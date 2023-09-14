# BFC特性  
1. 内部box会在垂直方向，一个接一个地放置。  
2. Box垂直方向的距离由margin决定，在一个BFC中，两个相邻的块级盒子的垂直外边距会产生折叠。  
3. 在BFC中，每一个盒子的左外边缘（margin-left）会触碰到容器的左边缘(border-left)（对于从右到左的格式来说，则触碰到右边缘）  
4. 形成了BFC的区域不会与float box重叠  
5. 计算BFC高度时，浮动元素也参与计算  
6. BFC就是页面上的一个隔离的独立容器，容器里面的子元素不会影响到外面的元素。反之也如此。

# 触发 BFC
只要元素满足下面任一条件即可触发 BFC 特性：  
- body 根元素  
- 浮动元素：float 除 none 以外的值  
- 绝对定位元素：position (absolute、fixed)  
- display 为 inline-block、table-cells  
- overflow 除了 visible 以外的值 (hidden、auto、scroll)  
- flex布局  
- grid布局

# 应用
1. 避免外边距折叠
2. 解决浮动元素造成的父元素高度塌陷问题  
3. 阻止元素被浮动元素覆盖

查看[10 分钟理解 BFC 原理](https://zhuanlan.zhihu.com/p/25321647)  
查看[介绍下BFC及其应用](https://github.com/Advanced-Frontend/Daily-Interview-Question/issues/59)
