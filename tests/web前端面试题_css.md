1. css盒子模型  
答：在网页中，元素所占据的位置由内而外由content、padding、border、margin四部分组成。盒子模型又分为标准盒子模型和IE盒子模型，标准盒子模型，设置的宽高仅仅是content的宽高；IE盒子模型设置的宽高是content+padding+border的总宽高。这两种盒子模型可以用css3属性box-sizing来设置，值为content-box则是标准盒子，值为border-box则是IE盒子。 
2. link与@import区别 
答：link是XHTML的标签，不仅仅可以用来引入css文件，还可以设置rel属性等，没有兼容性问题，而且是在页面加载的同时加载css文件的；@import是css2提出的，仅仅用于引入css文件，并且可能存在兼容性问题，是在页面加载完成之后加载css文件的  

 


