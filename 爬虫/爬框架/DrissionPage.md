# DrissionPage
## 控制浏览器
 - ChromiumPage
## 收发数据包
- SessionPage
## 复合模式
- WebPage 
	- d模式，浏览器（ChromiumElement）
	- s模式，数据包（SessionElement）
	- page.change_mode() 切换模式

 ## 实战
 - 淘宝

 [python-DrissonPage实现手爬淘宝网_drissonphttps://blog.csdn.net/m0_74545383/article/details/135490099age官网-CSDN博客](https://blog.csdn.net/m0_74545383/article/details/135490099)

[(10 封私信 / 84 条消息) 程序员coding - 知乎 (zhihu.com)](https://www.zhihu.com/people/hou-sai-60)

[【GUI软件开发】小红书评论采集：自动采集1w多条，含二级评论！ - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/665509516)


├─ SessionPage
|     └─ SessionElement
|           └─ SessionElement
├─ ChrmoiumPage
|     ├─ ChromiumTab
|     |     └─ ChromiumElement
|     |     └─ SessionElement
|     ├─ ChromiumFrame
|     |     └─ ChromiumElement
|     |     └─ SessionElement
|     ├─ ChromiumElement
|     |     └─ ChromiumElement
|     |     └─ SessionElement
|     └─ ChromiumShadowElement
|           └─ ChromiumElement
|           └─ SessionElement
├─ WebPage
|     ├─ ChromiumTab
|     |     └─ ChromiumElement
|     |     └─ SessionElement
|     ├─ ChromiumFrame
|     |     └─ ChromiumElement
|     |     └─ SessionElement
|     ├─ ChromiumElement
|     |     └─ ChromiumElement
|     |     └─ SessionElement
|     ├─ ChromiumShadowElement
|     |     └─ ChromiumElement
|     |     └─ SessionElement
|     └─ SessionElement
|           └─ SessionElement
├─ SessionOptions
└─ ChrmoiumOptions
