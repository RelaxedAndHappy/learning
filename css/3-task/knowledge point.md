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

