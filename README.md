# lz.js
html 使用 Jquery 懒加载 与 webp 整合优化

使用方法 
	
	引入jquery.lazyload.lz.js

例如：
		
	<img src="occupying270.png" data-original="4304485231505859.jpg" webp="true">
		
img标签增加webp 属性 控制是否使用webp模式
		 
	webp="true" ，该img路径使用webp格式模式，判断客户端是否兼容webp格式如果客户端兼容webp格式，该img路径使用data-original替换.jpg或.jpeg 为.webp路径，如果不兼容使用data-original设置的路径。
	
	webp="false" 或 webp属性未设置，该img路径使用data-original设置的路径。
	
图片懒加载使用方式参考jquery懒加载事例

	$("img").lazyload({   
		threshold : 200,  
	    effect: "fadeIn"  
  });
