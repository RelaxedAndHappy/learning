1. flex 即弹性布局， 行内元素也可以使用flex布局
  
   注意： 设置flex布局以后， 子元素的float，clear和vertical-align属性将失效;

2. flex有6个个属性
   
    flex-direction:  及项目的排列方向
       它有4个值： row(默认值), 主轴的水平方法，起点在左端；
       				row-reverse：主轴的水平方法，起点在右端;
       				column: 主轴为垂直方向， 起点在上沿
       				column-revers: 主轴为垂直方法，起点在下沿

    flex-wrap:  项目在一条线（又成轴线）上，如果轴线排不下，如何换行;
    	它有3个值： nowrap(默认值)，不换行；
    				wrap，换行，第一行在上方;
    				wrap-reverse；换行第一个在下方;

    flex-flow: 是flex-direction和flex-wrap属性的简写形式,默认值是row nowrap

    justify-content定义了项目在主轴的对齐方式;
         它有5个值： 
         	      flex-start(默认值) 左对齐；
         	      flex-end：右对齐;
         	      center: 居中；
         	      space-between: 两端对齐，项目之间的间隔都相等;
         	      space-around: 每个项目两侧的间隔相等，所以项目之间的间隔比项目与边框的间隔大一倍;

    align-itmes 定义项目交叉轴如何对齐，交叉其实就是上下方向；
    	它有5个值： flex-start： 交叉轴起点对齐，沿上边缘对齐
    				flex-end： 交叉轴终点对齐，下边缘对齐
    				center: 交叉点居中对齐， 可以理解为垂直居中
    				baseline： 项目的第一行文字的基线对齐;
    				stretch: （默认值）， 如果项目未设置高度或者设为auto,将占满整个容器的高度;

    align-content: 定义多根轴线对齐方式; 如何只有一根不起作用;
    	它有6个值 ： flex-start : 与交叉轴的起点对齐；
    				 flex-end： 与交叉轴的终点对齐;
    				 center: 与交叉轴的中点对齐;
    				 space-between:与交叉轴两端对齐，轴线之间的间隔平均分布;
    				 space-around: 每根轴线两侧的间隔都是相等，所以轴线之间的间隔比轴线的边框间隔大一倍;
    				 stretch(默认值): 轴线沾满整个交叉轴

3. 项目上的属性。
     
     order 定义项目的排列顺序，数值越小，排列越靠前，默认是0；
     flex-grow: 定义项目的放大比例，默认值0 。即如何存在剩余空间，也不放大;
				如果flex-grow属性都为1， 则他们将等分剩余的空间, 如果一个项目的flex-grow属性为2 其他项目都是为1，则前者占据的空间比其他想多一倍;

	flex-shrink:  定义项目缩小比例，默认值1， 如果空间不足，该项目将缩小;
	           如何改flex-shrink属性都为1，当空间不足时，都等比例缩小，如何一个项目的flex-shrink属性为0，其他项目都为1，则空间不足，前者不缩小；

	flex-basis：定义了分配在多余空间之前，项目占据的主轴空间，默认是auto 即项目本来的大小；

	align-self： 允许单个项目有与其他项目不一样的对齐方式，可覆盖align-items属性，默认值为auto,表示继承父元素align-items属性，如何没有父元素，则等同于stretch；
