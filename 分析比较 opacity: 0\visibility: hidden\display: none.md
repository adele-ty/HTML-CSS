# 是否占据空间和点击
- display: none (不占空间，不能点击)（场景，显示出原来这里不存在的结构）  
- visibility: hidden（占据空间，不能点击）（场景：显示不会导致页面结构发生变动，不会撑开）  
- opacity: 0（占据空间，可以点击）（场景：可以跟transition搭配）  
# 株连性
如果祖先元素遭遇某祸害，则其子孙孙无一例外也要遭殃  
- 若父节点元素应用了opacity:0和display:none，无论其子孙元素如何挣扎都不会再出现在大众视野；  
- 若父节点元素应用visibility:hidden，子孙元素应用visibility:visible，那么其就会毫无意外的显现出来。  
# 性能
display: none 会回流，性能开销较大
visibility: hidden 会重绘，性能损耗较少
opacity: 0 会重绘，性能损耗较少