1.padding 和 margin  一个是间距，一个是填充，都存在上下左右

  当margin 设置成为百分数的时候，其top,right,bottom,left的值都是参考父元素盒子的宽度计算，padding依然

3. rem单位，相对与根(html)元素大小

4. absolute 绝对定位：
    
    脱离文档流

    绝对定位有效时。浮动是无效

    不依赖的absoulute： 设置margin属性可以对位置精确调整；
						跟随性

	>选择器，只会选中当前元素中的子元素，

	例如:<h1>This is <strong>very</strong> <strong>very</strong> important.</h1>
		<h1>This is <em>really <strong>very</strong></em> important.</h1>
	
		h1 > strong {color: red}
		只会选中h1下的strong元素，而包裹在em下的strong元素不会被选择

   css3
      calc() 自动计算宽度

	display: table-cell; 指让标签以表格单元格的形式呈现，类似于td标签
			  与大小不固定的元素垂直居中
			  与两栏自适应布局
			  等高布局
			  详细地址：http://www.zhangxinxu.com/wordpress/2010/10/%E6%88%91%E6%89%80%E7%9F%A5%E9%81%93%E7%9A%84%E5%87%A0%E7%A7%8Ddisplaytable-cell%E7%9A%84%E5%BA%94%E7%94%A8/

	position: absolute; 
		在绝对定位下 ，可以设置top，left，right，bottom 自动拉伸元素，不用设置高度宽度；
	当尺寸限制，拉伸以及marigin:auto同时出现的时候，就会有绝对定位元素绝对居中的效果
		对于position为absolute和fixed的元素，同时设置left、right和width，即可由margin:auto水平居中；
同理，top、bottom、height即可设置垂直居中。

	css3: user-select: none | text | all | element
		默认值 text
		none 文本不能被选中，text 可以选择文本
		all 当所有内容作为一个整体时可以被选中，如果双击或者上下文点击子元素，那么被选中的部分将是以该子元素向上回溯的最高祖先元素
		element：可以选择文本，但选择范围受元素边界的约束
	

 隐形改变display类型: 
 		元素设置了position：absolute，或者float：left/right 时， 元素的display显示类型就会自动改变成display:inline-block，这样就是可以设置宽度，默认宽度沾满父元素


 		vertical-align: middle 设置垂直居中的位置， 把元素放在父元素的中部，如果是有图片，给图片定义此样式

 viewport 响应式
	width: 控制viewport的大小，可以指定一个值，如device-width为设备的宽度(单位为缩放为100%时的css的像素)
	height: 和width相对应，指定高度
	initial-scale: 初始缩放比例，也即当前页面第一次load的时候的缩放比例 位1.0表示按页面实际尺寸显示
	maximum-scale: 允许用户缩放到最大比例
	minimum-scale:允许用户缩放到最小的比例
	user-scalable:用户是否可以收到缩放;