


工具箱
Nmap
	[Nmap使用教程图文教程（超详细） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/585377081)
	[Nmap入门到高级【第三章】 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/618942575#:~:text=XMAS%E6%89%AB%E6%8F%8F%E6%98%AF%E4%B8%80%E7%A7%8D%E4%B8%8D%E5%B8%B8%E7%94%A8%E7%9A%84TCP%E6%89%AB%E6%8F%8F%E7%B1%BB%E5%9E%8B%EF%BC%8C%E4%B8%BB%E8%A6%81%E7%94%A8%E4%BA%8E%E6%8E%A2%E6%B5%8B%E7%9B%AE%E6%A0%87%E4%B8%BB%E6%9C%BA%E4%B8%8A%E7%9A%84%E4%B8%80%E4%BA%9B%E7%89%B9%E6%AE%8A%E6%9C%8D%E5%8A%A1%E5%92%8C%E5%BA%94%E7%94%A8%E7%A8%8B%E5%BA%8F%E7%9A%84%E5%AD%98%E5%9C%A8%E5%92%8C%E9%85%8D%E7%BD%AE%E3%80%82,XMAS%E6%89%AB%E6%8F%8F%E5%90%91%E7%9B%AE%E6%A0%87%E4%B8%BB%E6%9C%BA%E5%8F%91%E9%80%81%E4%B8%80%E4%B8%AAFIN%E3%80%81URG%E3%80%81PSH%E6%A0%87%E5%BF%97%E4%BD%8D%E9%83%BD%E8%A2%AB%E8%AE%BE%E7%BD%AE%E4%B8%BA1%E7%9A%84%E5%8C%85%EF%BC%8C%E5%A6%82%E6%9E%9C%E7%9B%AE%E6%A0%87%E4%B8%BB%E6%9C%BA%E7%9A%84%E7%AB%AF%E5%8F%A3%E5%A4%84%E4%BA%8E%E5%BC%80%E6%94%BE%E7%8A%B6%E6%80%81%EF%BC%8C%E5%88%99%E4%BC%9A%E8%BF%94%E5%9B%9E%E4%B8%80%E4%B8%AARST%E5%8C%85%EF%BC%8C%E8%A1%A8%E6%98%8E%E8%AF%A5%E7%AB%AF%E5%8F%A3%E5%A4%84%E4%BA%8E%E5%85%B3%E9%97%AD%E7%8A%B6%E6%80%81%E3%80%82)
	[【精选】kali初学——nmap扫描_kali nmap扫描端口命令_萌伶的博客-CSDN博客](https://blog.csdn.net/weixin_49998039/article/details/125242779)
	常用
		扫描网段
		nmap -sP 192.168.31.*
		扫描主机
		nmap 【host ip】
		扫描端口
		nmap 【host ip】-p 80
		版本识别
		nmap 192.168.31.180 -p 80 -O
		扫描结果导出为文件
		nmap 192.168.31.180 -p 80 -oN result.txt
		nmap 192.168.31.180 -p 80 -oX result.xml
	扫描结果，常见端口
		[常用端口号及攻击方向汇总_常见端口及攻击方向-CSDN博客](https://blog.csdn.net/weixin_42320142/article/details/102679143)
	
Metasploit
	SSH爆破
	[Metasploit对目标主机SSH爆破_metasploit端口攻击-CSDN博客](https://blog.csdn.net/weixin_39934520/article/details/108042194)

msfconsole（MSF终端）（irb交互式终端）
	https://docs.metasploit.com/

教程
	[tiancode/learn-hacking: 开始学习Kali Linux 各种破解教程 渗透测试 逆向工程 HackThisSite挑战问题解答 (github.com)](https://github.com/tiancode/learn-hacking)

拓展语言
	python脚本


[[攻击流程]]

![[Pasted image 20231219191630.png]]