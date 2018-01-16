# H5
这里整理了一些采用不同切割方法的例子：

## 一、网易常用换算方案
   要点：直接以iPhone6(750px为基准) 保证1rem=100px的换算,设定body的宽度为7.5rem; 结合脚本动态设置html的font-size大小
  		document.documentElement.style.fontSize = document.documentElement.clientWidth/7.5+"px";
   
   例子：index.html

## 二、通过CSS3的媒体查询设置不同设备像素比的样式
	例子：dpr.html

## 三、淘宝常用的适配方案 Flexible
	要点：
	    1、rem就是相对于根元素<html>的font-size来做计算；

	    2、lib-flexible是一个制作H5适配的开源库，可以点击这里下载相关文件，获取需要的JavaScript和CSS文件。

	    3、在head内引入script
	    <pre>
	    <script src="http://g.tbcdn.cn/mtb/lib-flexible/0.3.4/??flexible_css.js,flexible.js"></script>
		</pre>
	    4、1rem = 75px;

	例子：flex.html
	
	问题：对iPad支持力度不够 会默认当做Android来对待 dpr设置为1
