第一步：获取画图框对象

第二步：获取当前画图框的上下文——理解成对当前画图框的一套工具

第三步：引用上下文的一系列画图工具，一步一步的执行画图



moveTo(x,y)：设置起点方法
lineTo(x,y)：画线方法
lineCap：线头属性
lineWidth：线宽度
strokeStyle：线属性，rgb等

beginPath()：重新开始新的线段绘制
closePath()：关闭路径，连接到起点

fillStyle：填充属性
fill()：填充fillStyle

fillRect(x,y,width,height)：直接填充一个矩形

arc(centerX,centerY,radius,startAngle,endAngle)：画圆弧

stroke()：显示画的结果
