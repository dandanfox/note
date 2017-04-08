- 样式
	- 背景 backgorund
	- 文本
		- text-indent
		- text-align
		- word-spacing
		- letter-spacing
		- text-transform
		- text-decoration
		- white-space
		- direction
			- ltr
			- rtl
	- 字体	
		- font-style
		- font-variant
		- font-weight
		- font-size
		- font-family
	- 列表 (ul，ol)	
		- list-style-image
		- list-style-position
		- list-style-type
		- list-style (前三个合在一起的缩写形式)
	- 表格 (基础而有用的一个东西)
		- border-collapse
		- border-spacing
		- caption-side
		- empty-cells
		- table-layout
	- 轮廓
		- outline-color
		- outline-style
		- outline-width
- 盒模型
	- element(height,width)
	- padding
	- border
	- margin
		- 外边距合并，当两个垂直外边距相遇时，它们将形成一个外边距，合并后的边距等于两个中较大的那个
- 定位
	- position
		- static
		- relative
		- absolute
		- fixed
	- top
		- auto
		- %
		- length
	- right
	- bottom
	- left
	- overflow
		- visible(default) 内容会超出element区域
		- hidden 内容被截取，超出不显示，并且不现实滚动条
		- scroll 内容不截取，始终显示滚动条
		- auto	内容不截取，自动判断是否显示滚动条
	- clip
		- rect(0px,60px,200px,0px) 截取一个区域
	- vertical-align
	- z-index
- 高级
	- 对齐
		1. 中间对齐 width:70%;marign:auto;
		2. 左对齐
			- postion:absolute;left:0;
			- float:left;
	

display vs visibility
visibility种的hidden，依旧会占据空间，一般不太需要
visibility （不常用，使用场景不太常用）
	- visible (default)
	- hidden 
	- collapse

1.font:	

	- font-style:
		- normal
		- italic
		- oblique
	- font-variant
		- normal
		- small-caps
	- font-weight 
		- normal
		- bold
		- bolder
		- lighter
		- num (100-900) 400=normal 700=bold
	- font-size/line-height
		- 14px/1
	- font-family
	

2.outline, border
outline 使用场景比border更少
	
	- outline-width
		- thin		
		- medium
		- thick  (加粗)
	- outline-style
		- none	(default)
		- dotted
		- dashed
		- solid
		- double	
		- ... 
	- outline-color

3.box-sizing

	- box-sizing
		- content-box 内容的宽高是确定的，border另算
		- border-box  内容的宽高不确定，hiehgt-border=内容高度
	 
4.white-space

	- white-space
		- normal 浏览器忽略空白
		- pre	浏览器保留空白，类型html标签pre
		- nowrap	 忽略空白，文本不会换行直到遇到br标签为止（nomarl+wrap）
		- pre-wrap 保留空白，并能换行（组合pre+wrap）
		- pre-line 合并空白序列，换行

5.vertical-align 
	设置元素的垂直对齐方式
	
	- vertial align
		- baseline (default)
		- sub	(文本下标)
		- super	(文本上标)
		- top	(把元素的顶端与行中最高元素的顶端对齐)
		- text-top (把元素的顶端与父元素字体的顶端对齐)
		- middle		(把此元素放置在父元素的中部。)
		- bottom	(把元素的顶端与行中最低的元素的顶端对齐)
		- text-bottom(把元素的底端与父元素字体的底端对齐)
		- length
		- %

6.text-transform

		- text-transform
			- none
			- capitalize 首字母大写
			- uppercase
			- lowercase
			
7.appearance 使得div想button，icon，window等
	
8.border-callpase 专门为table设置的一个属性
	
		- border-collapse
			- separate (default)
			- collapse (忽略border-spacing和empty-cells)
			
9.text-rending 字体渲染

-webkit-font-something 字体抗锯齿

-moz-font-something	字体抗锯齿

10.animation
	
	- animation
		- animation-name	（动画名称@keyframe）
		- animation-duration (动画持续时间)
		- animation-timing-function(动画快慢)
		- animation-delay
		- animation-iteration-count
		- animation-direction
	
	- animation-duration 动画一个周期的时间(秒或毫秒)
		- 0 (default)
		- num (2s,3s)
	- animation-timing-function （infinite 是永久循环）
		- linear	从头到尾一样
		- ease（default）从低速开始，加快，结束前变慢
		- ease-in 以低速开始
		- ease-out 以低速结束
		- ease-in-out 以低速开始和结束
		- cubic-bezier(n,n,n,n)
	- animation-delay (-2s立即开始，跳过前2s的动画，2s等待2s然后开始动画) 
		- 0 (default)
		- num(2s,-2s)
	- animation-iteration-count
		- 1	(default)
		- n
		- infinite (无限)
	- animation-direction
		- normal
		- alternate
	  
	- @keyframes animationname{keyframes-selector{css-styles;}}
		- animatinoname
		- keyframes-selector 
			- 0-100%
			- from 0%
			- to 100%
		- css-styles
	
11.border-radius
	
	- border-top-left-radius
	- border-top-right-radius
	- border-bottom-left-radius
	- border-bottom-right-radius
	
12	list-style 

	- list-style-type 虽然属性有很多，不过一般都不用了，都是用none
	- list-style-position
		- outside
		- inside
	- list-style-image
		- url(...)

13 float css1
	
	- none
	- left
	- right

14 transform 2D,3D的转换
	
	- 2D方法
	- transform-origin: x-axis y-axis;
		- translate() translate(50px,100px) 2d方向x,y移动
		- rotate()	rotate(30deg) y轴夹角
		- scale() scale(2,3)x长度2倍,y方向长度3倍
		- skew() skew(20deg,30deg) 翻转，
		- matrix() 矩阵，transform-origin 等的综合应用，很复杂
	
	- 3D
	- transform-origin: x-axis y-axis z-axis;
	
15 filter 滤镜

16.transition
	
	- transiation-property	(css property)
	- transition-duration
	- transation-timing-function
	- transition-delay
		
17.display

		- block 前后都带有换行符
		- inline	 前后都没有换行符
		- inline-block 
		- list-item 列表显示
		- run-in
		- table	table前后带有换行
		- inline-table
		- table-row-group tbody
		- table-head-group thead
		- table-footer-group tfoot
		- table-row tr
		- table-column-group colgroup
		- table-column col
		- table-cell td,th
		- table-caption caption
		
18.clear
	
		- clear
			- left 左侧不允许浮动元素
			- right 右侧不允许浮动元素
			- both  两侧不允许浮动元素
			- none(default)

19.max-width
		
		- max-width
			- none(default)
			- lenth
			- % (定义基于包含它的块级对象的百分比最大宽度)

20.background
		
		- css 2
			- background-color
				- transparent(default 透明的)
			- background-position
				- top left
				- top center
				- top right
				- center left
				- center center
				- center right
				- bottom left
				- bottom center
				- bottom right
				- x% y%
				- xpos ypos
			- background-repeat
				- repeat (default)
				- repeat-x
				- repeat-y
				- no-repeat		
			- background-clip 属性规定背景的绘制区域
				- border-box (default)
				- padding-box
				- content-box
			- background-attachment 
				- scroll (default)
				- fixed 当页面的其余部分滚动时，背景图像不会移动。
			- background-image
				- none (default)
		- css 3
			- background-size						
				- length (100px 200px,200px)
				- percentage (100% 100%,50%)
				- cover
				- contain
			- background-origin 规定 background-position 属性相对于什么位置来定位
				- border-box (default)
				- padding-box			
				- content-box

21.box-shadow: h-shadow v-shadow blur spread color inset;

		- box-shadow
			- h-shadow
			- v-shadow
			- blur (可选)
			- spread (可选)
			- color (可选)
			- inset	(可选)
			 
22.text-decoration
	
		- none 
		- underline
		- overline
		- line-througn
		- blink

23.text-overflow
	
		- clip
		- ellipsis (= '...')
		- '.....'(任意字符串替换被截断的字符串)

	


	 