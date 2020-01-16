### 来五毛钱的CSS
# positoin
	
   static:  默认遵循文档流的移动，从上往下，从左至右; 块级元素占一行，行内元素往后移动
   
   fixed: 固定在浏览器中的位置 , 浏览器滚动条下来也不会动<br>
   ```
		position: fixed;
		top: 80%;
		left: 0;
		width: 100px;
		height: 100px;
		transform : tranlate( 0,-40%);
   ```
   absolute: 是相对于最近的且不是static定位的父元素来定位, 会随浏览器滚动而滚动<br>
   ```
   		position: absolute;
   		top: 80%;
   		left: 40%;
   		width: 100px;
   		height: 100px;
   		transform : tranlate(-20%,-40%);
		/**
		margin-top: -50px;
		margin-left: -50px;
		**/
   ```
   relative: 是相对于其原本的位置来定位的, 原本占用的位置依然会占据<br>
   ```
   		position: relative;
   		top: 80%;
   		left: 0;
   		width: 100px;
   		height: 100px;
   		transform : tranlate(0, -40%);
   ```
   Inherit: 继承父元素的position值<br>
   
   