#Slides效果的焦点图
 一款基于slidesjs的左右滑动焦点图插件，带文字标题，也可带文章内容，条状/圆点索引按钮，左右切换，结构简单，调用方便！
可以根据自己的需要在只修改css的的基础上改变界面风格，配合不同主题，完成不同的定制。
####官方地址：http://www.slidesjs.com

##兼容性

* ie6+
* Chrome 8+

##样例：
* [小图单页](http://192.168.14.97:8080/acc/lxj/focus/focus1/)
* [中图双页](http://192.168.14.97:8080/acc/lxj/focus/focus2/)
* [大图单页]( http://192.168.14.97:8080/acc/lxj/focus/focus3/)

##方法和API
###1、方法
     slides();
```javascript
$('#slides').slides({
    			preload: true,
				preloadImage: 'images/loading.gif',
				play: 5000,
				pause: 2500,
				hoverPause: true,
				animationStart: function(current){
					
					if (window.console && console.log) {
						// example return of current slide number
						console.log('animationStart on slide: ', current);
					};
				},
				animationComplete: function(current){
					
					if (window.console && console.log) {
						// example return of current slide number
						console.log('animationComplete on slide: ', current);
					};
				},
				slidesLoaded: function() {
					
				}
			});
```
###2、API
    无
     
###3、参数说明
     preload: true, //是否预加载（是）
     preloadImage: 'images/loading.gif',//加载时的展示图片路径
     play: 5000,//焦点图播发时间（5000ms）
     pause: 2500,//两次滑动暂停时间（2500ms）
     hoverPause: true,//悬浮暂停（是）


##更新日志
* 2015年11月8日第一次更新

##下载地址






