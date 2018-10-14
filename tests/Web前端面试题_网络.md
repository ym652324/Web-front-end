1. url->页面加载完成的整个流程  
答：（1）dns寻址（将域名转化为IP地址）  
（2）HTTP请求连接，进行TCP三次握手  
（3）传送数据  
（4）断开连接，进行TCP四次挥手  
（5）浏览器解析HTML文件，加载图片、脚本等资源，构件DOM树  
（6）浏览器渲染页面  
2. get与post区别    
答：（1）get一般是从指定的资源请求数据；post一般是向指定的资源提交要被处理的数据  
（2）get发送的数据大小比较小，post发送的数据大小很大  
（3）get发送数据时，参数会显示到地址栏，不适合发送保密性数据  
（4）get在发送请求的时候只需要发送一次，而post需要发送两次，一次发送header，一次发送数据  
（5）get请求可被缓存，会保留在浏览器历史记录中，可被收藏为书签，post与之相反  
3. 介绍ajax，请求过程是怎样的  
答：ajax即异步的JavaScript和XML，可以在不重新刷新页面的情况下与服务器通信，交换数据，或更新页面。请求过程如下：  
> （1）创建XMLHTTPRequest对象
```
if(window.XMLHttpRequest){ // Mozilla, Safari, IE7+ ...
  httpRequest = new XMLHttpRequest();
}
else{ // IE 6 and older
  httpRequest = new ActiveXObject('Mirrosoft.XMLHTTP');
}
```
（2）设置响应函数
```
httpRequest.onreadystatechange = function(){
  // 操作
};
```
或者使用函数名，不用匿名函数
 ```
 httpRequest.onreadystatechange = ResponseFunction;
 ```
 （3）处理响应
 ```
 httpRequest.open('GET','URL',true);
 httpRequest.send();
 ```
 注：
 * open('method','URL',true)：method是GET、POST、HEAD等。需要大写。
 * 第三个参数用于设置请求是否是异步的。
