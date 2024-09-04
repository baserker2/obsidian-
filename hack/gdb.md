dbg overflow2
b 断点
ni 下一步
r 运行
c 继续运行
disassemble 反汇编
p 打印
x/100x &buf 打印内存
x/100xb &buf 打印内存，word=2byte ，byte=8bit
info reg 查看寄存器
b 0x+地址
x/10x $ebp 打印寄存器
cyclic 200 创建循环随机字符串
cyclic -l 查找溢出点距离
[很经典的GDB调试命令，包括查看变量，查看内存-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1036960)
[GDB调试查看内存数据_gdb 查看内存-CSDN博客](https://blog.csdn.net/u014470361/article/details/102230583)

linux下反汇编objdump
	objdump -d -M intel ./woof | grep getshell
	objdump -d
	-M intel指定架构
	 ./woof  指定对象
	 | grep getshell
	[objdump命令详解-CSDN博客](https://blog.csdn.net/qq_41683305/article/details/105375214)
	objdump -S overflow2
	查看硬盘中程序节解构

vmmap（mmap：虚拟内存）查看内存映射 vmmap stack
[GDB 调试--新手笔记1_gdb vmmap-CSDN博客](https://blog.csdn.net/weixin_44442852/article/details/102062368)
	GEF
	xinfo 查看地址页信息 
		xinfo $pc
		xinfo $sp
	telescope (显微镜)命令观察当前栈，或者pc位置的代码信息。
	dps $pc li
	pattern create 40 创建垃圾字符
	pattern search $esp 找返回地址
	pi 调用python语句

切换gdb工具
	vim ~/.gdbinit
	一般来说，peda 用来做逆向破解是最方便的  
	gef 用来 debug 最好  （windbg同族指令）
	gdbinit 相对于上面两个来说显示信息比较少，喜欢简单版的可以试试
	[PWN中的gdb调试, pwndbg,peda,gef 切换使用的方法；_pwn gef-CSDN博客](https://blog.csdn.net/weixin_45556441/article/details/115536426)
	[gdb exhanced features(GEF)工具的使用 - 寻梦99 - 博客园 (cnblogs.com)](https://www.cnblogs.com/liulianzhen99/articles/17824258.html)

gef教程
	[Advanced exploitation with GDB-GEF: GEF 101 - Solving pwnable.tw/start - YouTube](https://www.youtube.com/watch?v=KWG7prhH-ks)