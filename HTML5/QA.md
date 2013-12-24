#Q&A#


##Q：千牛H5插件怎么开发，给个DEMO看看什么样的
>
	千牛上那么多已经开发好的插件，任何一个都能起到“看看什么样”的作用，如果您准备开发千牛插件，都先不装一下千牛，这个也实在说不过去吧。
	实在要看demo的话，其实我们的JSSDK文档就是一个插件，地址是：http://jindoucloud.aliapp.com/bridge/index.html

##Q: 如何在千牛上开发一个H5应用
>
	先抛开H5，其实很多时候就是被这两个字绕进去了。开发web程序会么？大家肯定都会说：那个熟，就是做Web开发出身的。那你肯定也能马上就理解所谓的：开发H5插件。其实说白了，就是开发了一个web程序，适配了移动页面，然后把web程序的地址给千牛，用户点击你们程序图标的时候，会跳到你们web地址上。就这么简单。
	上面这段明白了之后，咱再来说H5，所谓的H5，就是javascript多了几个API，让原来可能JS做不了的事情，现在能做了。在手机上目前支持没有PC好，所以看起来比用起来爽。
	
	
##Q: 千牛上开发H5应用有什么特别
>
	特别就在于，在千牛上开发H5，我们提供了一个JSSDK，通过JSSDK，你可以和native代码打交道，完成更简单的身份校验，数据调用，已经javascript做不到的事情。JSSDK的地址是：
	http://jindoucloud.aliapp.com/bridge/index.html

##Q: JSSDK为什么我点了没反应
>
	哥们，又在PC浏览器里点了吧，JSSDK既然是和native打交道的，自然必须跑在千牛的环境里，你在chrome里点击，有啥用呢？
	
##Q：千牛里的那个日历组件好好看的，能开放给我们用么？
>
	千牛的确开放了一些组件，但是这些组件都是和业务相关的，目前没有任何和UI相关的组件，近期也不太会做UI视觉上的组件开放。觉得好看，麻烦自己写一个，想偷懒，其实有很多开源的。
	顺便说一下：千牛里的日历组件用的是native默认的，其实通过HTML5 设置input type就可以呼出来，请问再提需求之前，是否有自己努力找过解决办法呢？有没有去了解过呢？
	
##Q：为什么一定要求所有的JS和CSS后面带版本号
>
	因为移动端本身流量就是资源，一个好的插件一定是动用了各种各样的缓存（其实PC上浏览器的缓存也挺重的）。当然你也可以不加缓存，但是用户量大起来了之后，要多少机器才能抗？
	所有，目前来说加版本号是最稳妥的办法，你要实在不愿意加，或者你想试试其他办法，我也逼不了你，但是请保证不因为缓存问题出故障，除了故障请问故障买单。
	如何做一个稳妥的缓存：文档地址https://github.com/emersonli/qianniu-wiki/blob/master/HTML5/offline_update.md
	
##Q: 在千牛上开发H5插件如何debug
>
	目前提供了一个js debug方案，操作起来确实稍微有点繁琐，请理解，目前业务压力的情况下，用户体验确实不好，请先包容下，等空下来，我们会简化proxy的步骤。
	对了，目前只有IOS提供此套方案，android并不支持。
	https://github.com/emersonli/qianniu-wiki/blob/master/HTML5/jsbrige_debug.md
	

