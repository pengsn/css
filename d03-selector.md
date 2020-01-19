### 来五毛钱的CSS

##	选择器 

1. `specificity` 计算规则 
	- 行内样式    1 0 0 0 
	- id选择器    0 1 0 0
	- 类选择器    0 0 1 0
	- 元素选择器  0 0 0 1
	
	按以上规则计算优先级： 
	1. !important 级别最高  行内样式级别其次
	2. 按以上规则，内联样式  > id选择器样式 > 类选择器样式 > 元素选择器样式
	3. 多样式组合， 不进位增加，数值越大，级别越高； 所谓不进位即 11个[类选择器]也抵不过一个[id]
	4. 级别相同，后出现的覆盖先出现的
	
2. `选择器`
	- 普通选择器
	
		标签|描述
		-|-
		*|选择所有元素
		#id|id选择器
		.class|class选择器
		el|标签元素选择器
		el,el2| 多个元素公用一个样式分组
		el el2 | 所有后代
		el>el2 | 第一代后代
		el+el2 | 平级往后的一个兄弟元素
		el~el2 | 平级往后所有的兄弟元素
	
	- 属性选择器

		标签|描述
		-|-
		[att]| 包含某个属性
		[att='v'] |属性等于某个值
		[att~='v'] |属性包含 单词v
		[att、='v'] |属性以v-开头
		[att^='v'] |属性以v开头
		[att$='v'] |属性以v结尾
		[att*='v'] |属性包含字符串v

   - 伪类选择器

		标签|描述
		-|-
		:link| 未被访问的链接
		:visited|访问过的链接
		:active|正在被访问的链接
		:hover| 鼠标悬浮的链接
		:foucs| 拥有焦点的链接
		:lang(language)|拥有某个属性的节点
		-|-
		:first-of-type|选择某个类型元素的第一个
		:last-of-type|选择某个类型元素的最后一个
		:only-of-type|选择某个类型元素是父级下同类型独子的一个
		:nth-of-type(n)|选择某个类型元素的正数第n个
		:nth-last-type(n)|选择某个类型元素的倒数第n个
		-|-
		:first-child|第一个子元素
		:last-child|最后一个子元素
		:only-child|选择某个类型元素是父级下独子的一个
		:nth-child(n)|选择某个类型元素是父级下同类型的第n个
		:nth-last-child(n)|选择某个类型元素是父级下同类型的倒数第n个
		-|-
		:root|文档根节点
		:empty|空节点
		:target|活动节点
		:enabled|启用的节点
		:disabled|disabled的节点
		:checked|checked的节点
		:not(e)|排除某个节点
		:read-only|只读元素的节点
		:required|匹配必填项的节点
		:valid| 匹配合法的节点
		:invalid| 匹配非法的节点

   - 伪元素选择器
		
		标签|描述
		-|-
		::before|元素之前添加内容
		::after|元素之后添加内容
		::first-letter|首字母
		::first-line|首行
		::selection|处理选中的文本 如颜色，鼠标
		
		
		