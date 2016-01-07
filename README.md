#lesson1:material lesson
![Alt text](./tu.jpg)

- **normal photo:未加任何效果的设计风格**
- **material photo:根据谷歌material design文档做出的material设计风格**

>`需要打造material设计风格，需要把握三点点：微厚度、微阴影、通过阴影调节环境深度关系，结合代码来分析`

###顶部topbarCSS样式
```html 
.topbar{
	height: 35px;
	line-height: 35px;
	background: #aaa;
	margin-bottom:5px;
	box-shadow: 0px 1px 0px #bbb inset,0px 1px 2px rgba(0,0,0,.6);
	color:#fff;
}

```
`box-shadow营造了这一风格："0px 1px 0px #bbb inset"为顶部增添了一抹高光，厚度出来了
"0px 1px 2px rgba(0,0,0,.6)"增加底部阴影。微厚度、微阴影的效果出来了
这部分比较灵活，看个人审美意识和色彩感觉吧`
###图片CSS样式
```html
.ele{
	box-sizing:border-box;
	float: left;
	width: 80px;
	height: 80px;
	background: #fffeff;
	margin: 5px;
	padding: 3px;
	box-shadow: 0px 0px 1px #fff inset,0px 1px 2px rgba(0,0,0,.3);
	transition:all 0.2s ease-in 0.1s;
}

.ele:hover{
	box-shadow: 0px 0px 1px #fff inset,0px 3px 6px rgba(0,0,0,.4)
};

```
`当鼠标经过时，调节盒子的阴影属性来实现深度的变化`

![Alt text](./tu2.jpg)

`#PS实现material设计风格时，主要使用"内阴影和投影"图层样式属性`

![Alt text](./tu3.jpg)
![Alt text](./tu4.jpg)

