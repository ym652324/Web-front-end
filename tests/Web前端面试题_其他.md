1. 页面加载如何优化  
答：雅虎团队提出了七个优化方面。  
（1）页面内容：尽量减少HTTP请求次数；页面简洁元素尽量少；多个外部文件可以合并成一个文件，减少文件下载次数    
（2）JavaScript：脚本置于文件底部；实现封装抽象，减少重复代码；减少访问DOM元素，缓存已经访问过的元素   
（3）css：样式表置顶；合理运用选择器减少重复代码；用<link>标签代替@import  
（4）图片：使用css精灵；大屏大图小屏小图，不要用同一张图片压缩适应需求；不要使用空的图片src  
（5）cookie：能不使用cookie就不使用，一定要使用的话，cookie大小越小越好，有效时间越长越好  
（6）服务器端：使用内容分发网络CDN；更多使用get而不是post；使用Gzip压缩传输文件；  
（7）移动端：一次传送的内容大小尽量小，移动端缓存限制；把页面内容打包成复合文件，减少下载次数    
 <div align=center>  
  <img src="https://github.com/ym652324/Web-front-end/blob/master/image/%E9%A1%B5%E9%9D%A2%E4%BC%98%E5%8C%96.png" width = 80% >    
  </div>  
   <p align=center> 参考：http://www.cnblogs.com/developersupport/p/webpage-performance-best-practices.html  </p> 
   
2. 如何处理浏览器兼容性问题  
