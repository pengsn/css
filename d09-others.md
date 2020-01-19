### 来五毛钱的CSS

### 一些CSS样式的特殊的妙用
1. 伪元素的使用
	如表格隔行变色
		nth-child(even) :th-child(odd) :th-child(2n)
	
2. inline-block 元素之间有间隙
		父元素添加样式：font-size=0px
	
3. input元素默认选中有轮廓
		outline: none;
		
4. box-sizing: border-box; 让div宽度=内外边距+边框+内容宽度

5. table tr之间有空隙 border-collapse:collapse;