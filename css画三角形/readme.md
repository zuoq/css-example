> 闲来无事，总结下用css画三角形的方法，我最早接触的一种方法是利用boeder属性画三角形，小面介绍一下其原理：

来看下正常的盒模型下的样式渲染效果：
``` css
    .border-with-con {
	width: 100px;
	height: 100px;
	margin: 0 auto;
	border-top: 40px solid #66ff66;
	border-left: 40px solid #0000cc;
	border-right: 40px solid #996600;
	border-bottom: 40px solid #333333;
}
```
其效果图如下：

![正常和模型下border显示](http://pic.yupoo.com/izqcool/G7QEWpNb/medish.jpg)
---

只有border而宽高为0时:
``` css
    .border {
	width: 0;
	height: 0;
	margin: 0 auto;
	border-top: 40px solid #66ff66;
	border-left: 40px solid #0000cc;
	border-right: 40px solid #996600;
	border-bottom: 40px solid #333333;
}

![只有border强宽下显示效果](http://pic.yupoo.com/izqcool/G7QF2JYn/medish.jpg)
---

可见border在秀安然的时候采用的是平分的方式，即相邻border之间各占一半，利用这个特性我们只需要控制border的显示与否以及设置border的大小，就可以画出各种三角形,例如：

![示例1](http://pic.yupoo.com/izqcool/G7QEWDPK/medish.jpg)
---

![示例2](http://pic.yupoo.com/izqcool/G7QEWMLC/medish.jpg)
---

![示例3](http://pic.yupoo.com/izqcool/G7QEWQd1/medish.jpg)
---





