### 来五毛钱的CSS
# 块级标签与行内标签
<br>**块级标签：**不能与其他标签并排，独占一行
		div p form h1 hr ul ol 
<br>**行内标签：**可以与其他行内标签并排, 共享一行，不能设置宽高，只能由内容撑起
		span label img a
<br>**特殊：**
		p, 文本级标签，只能是文本内容，不能放其他标签 

# display	
`inline`   行级元素<br>
`block`    块级元素，必须遵循盒子模型<br>
`inline-block` 行内块级元素 , 如input button 行内元素排列，又可设置块的大小<br>
`flex`     弹性布局


### flex

	1. flex-direction 设置排列方向
		row  | row-reverse | column | column-reverse
		
	2. flex-wrap 换行
		nowrap | wrap  | wrap-reverse
		
	3. flex-flow 是direction与wrap的简写形式 row nowrap
		
	4. justify-content 主轴上的对齐方式
	
	5. align-items   交叉轴的对齐方式
		
	6. flex 宽度grows，shink，basis...

# 细节点
inline-block: 标签之间会有间隙，导致的原因是换行符，消除的方式是在父级标签上设置font-size：0<br>
float: left,right; 浮动元素脱离文档流会导致父元素【高度属性】 坍塌 处理如下
```
	.parent-div:after{
		clear:both;
		display: block;
		content:'';
	}
```

设为 Flex 布局以后，子元素的float、clear和vertical-align属性将失效


	
	