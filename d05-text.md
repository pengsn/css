### 来五毛钱的CSS

## 文本
`word-spacing` 单词之间的间隔

`letter-spacing` 字符之间的间隔

`text-decoration` 文本下划线

`text-indent` 首行文本缩进


## wrap 换行
  `word-wrap` break-word 强制换行
  
  `overflow-wrap` break-word 强制换行
   
   `white-space`


## align 位置
  `text-align`  行内元素水平位置
  `vertical-align`  行内元素垂直位置
  `line-height `  行内元素所占行高

1. 行内元素水平居中
	text-algin: center;
	
2. 行内元素垂直居中
	父元素设置line-height=height;
	vertical-align=middle;
	
3. 块级元素水平居中
	margin: 0 auto;
	
4. 块级元素垂直居中
	
	根据需要选择position的方式
	
	```
		.mydiv{
			width: 100px;
			height: 100px;
			position: fixed;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
		}
	```
	
	jquery
	
	```
		$(window).resize(function(){
		 
		    $(".myblock").css({
		 
		        position: "absolute",
		 
		        left: ($(window).width() - $(".myblock").outerWidth())/2,
		 
		        top: ($(window).height() - $(".myblock").outerHeight())/2     });        
		 
		});	
	```
