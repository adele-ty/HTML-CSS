# vertical-align
用于设置一个元素的垂直对齐方式，但只针对行内元素或行内块元素以及表格单元格元素（table-cell）有效。  
图片底部默认空白缝隙问题：原因是行内块元素会和文字的基线对齐。  
解决方案：  
* 给图片添加vertical-align: middle|top|bottom等；  
* 将图片转换为块级元素display: block;
# text-align
定义行内内容（例如文字）如何相对它的块父元素对齐。text-align 并不控制块元素自己的对齐，只控制它的行内内容的对齐。对块级元素和table-cell元素有效。