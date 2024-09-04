 操作步骤 
- 设置pc为代理服务器
- 使用脚本清洗数据
- 手机**配置证书**和设置代理
app爬取
- https://juejin.cn/post/6972740110274002975
- 小程序爬取
- https://blog.csdn.net/HeyShHeyou/article/details/90452656
注意
https加密，需要证书，root手机
通过Charles抓取Android的Https链接数据

app抓包[面试官问我会不会APP抓包,我.. (qq.com)](https://mp.weixin.qq.com/s/4hQplDJ4xrV30ZkwE78QVQ)

appium
[启动appium服务的2种方法(python脚本&cmd窗口)_终端启动appium-CSDN博客](https://blog.csdn.net/wuyoudeyuer/article/details/107038096)

adb
[ADB安装及使用详解（非常详细）从零基础入门到精通，看完这一篇就够了-CSDN博客](https://blog.csdn.net/Python_0011/article/details/132040387)

[appium远程连手机调控 - 幸福来之不易 - 博客园 (cnblogs.com)](https://www.cnblogs.com/st998/p/13868183.html)











## 抓包
工具
 - Fiddler
 - Charles

app端devtool开启
[WankkoRee/WebViewPP: Enable WebView debugging and add vConsole in it. Support WebView, TBS X5, UC U4, Crosswalk(XWalk), XWeb. 启用 WebView 调试并添加 vConsole，支持 WebView、TBS X5、UC U4、Crosswalk(XWalk)、XWeb。 (github.com)](https://github.com/WankkoRee/WebViewPP)

wechat历史版本
[Releases · tom-snow/wechat-windows-versions (github.com)](https://github.com/tom-snow/wechat-windows-versions/releases)

wechat cdp
- 官网表示不支持websocket调试，是没实现还是怎么的
	- 了解chroium二开的架构，看看是被关闭了还是怎么的
	[Devtools架构浅析写此文章的起源是我目前正在做的一个开源项目miniblink（欢迎访问miniblink.net - 掘金 (juejin.cn)](https://juejin.cn/post/6844903565429833736)
	[Chrome DevTools Frontend 运行原理浅析 | 匠心博客 (zhaomenghuan.js.org)](https://zhaomenghuan.js.org/blog/chrome-devtools-frontend-analysis-of-principle.html
	![[Pasted image 20240818113050.png]]
	- 收集xweb信息，开源闭源
	- 启动行参数能不能打开？？通过启动行参数逆向了解项目结构
		 [chrome内核浏览器在PE下无声的一种解决办法 - PE讨论区 - 无忧启动论坛 - Powered by Discuz! (wuyou.net)](http://bbs.wuyou.net/forum.php?mod=viewthread&tid=421403)
		[Chromium Mojo & IPC | 柯幽 (keyou.github.io)](https://keyou.github.io/blog/2020/01/03/Chromium-Mojo&IPC/)
	- 逆向功底再练练，看看wechatwin.dll的关键字里还有没有其他关键字
	- 微信官方devtools
	[下载 / 稳定版更新日志 (qq.com)](https://developers.weixin.qq.com/miniprogram/dev/devtools/stable.html#_1-06-2407110-Windows-64-%E3%80%81-Windows-32-%E3%80%81-macOS-x64-%E3%80%81-macOS-ARM64)


