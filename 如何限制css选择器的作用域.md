限制 CSS 选择器的作用域可以确保样式仅对特定范围内的元素起作用。以下是一些方法来实现这个目的：  
* 使用父元素
```c
<div class="limited-scope">
  <p>这段文本将受到限制作用域的影响。</p>
</div>
.limited-scope p {
  color: red;
}
```
在这个例子中，仅在类名为 limited-scope 的 &lt;div> 内的 &lt;p> 标签会被着色为红色。  
* 使用特定的类名
```c
<p class="limited-scope">这段文本将受到限制作用域的影响。</p>
.limited-scope {
  color: red;
}
```
在这个例子中，只有具有类名 limited-scope 的 &lt;p> 标签会被着色为红色。  
* 使用属性选择器
```c
<p data-limited-scope>这段文本将受到限制作用域的影响。</p>
p[data-limited-scope] {
  color: red;
}
```
在这个例子中，只有具有 data-limited-scope 属性的 &lt;p> 标签会被着色为红色。
