



gcc编译指令
[gcc简介和命令行参数说明_gcc -t_KuoGavin的博客-CSDN博客](https://blog.csdn.net/yueguangmuyu/article/details/116703618)
指令是对计算机发出的命令，而伪指令则是对编译器发出的命令

C程序的编译过程：源代码 `->` 编译 `->` 汇编 `->` 链接 `->` 可执行文件 `->` 装载 `->` 执行

![[Pasted image 20231130233535.png]]
-E：==预编译==后停下来，生成后缀为 .i 的预编译文件
	gcc -E test.c -o test.i
	生成的还是文本文件，吧#中头文件展开了，在源程序中添加__attribute__等魔术字符，删除注释
	添加行号和文件名标识
	
-S：==编译==后停下来，生成后缀为 .s 的汇编源文件
	gcc -S test.c -o test.s
	内部为汇编伪代码，格式类似PE文件

-c：==**汇编**==后停下来，生成后缀为 .o 的目标文件
	gcc -c test.c -o test.o
	对照指令表生成机器指令

-o：将生成的目标文件==链接==成可执行文件
	gcc test.o - o test

【1】程序员的自我修养【62】
【2】实操[[dll注入]]中手动链接dll
*你好* ctrl+i
**你好** ctrl+b
==你好== ctrl+h
>你好 建立引用
[Obsidian中，最常用的14个Markdown语法（建议收藏） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/526494299?utm_oi=569633560235941888#:~:text=%E5%AD%97%E4%BD%93%E5%8A%A0%E7%B2%97%EF%BC%9A%2A%2A%E9%9C%80%E8%A6%81%E5%8A%A0%E7%B2%97%E7%9A%84%E6%96%87%E5%AD%97%2A%2A%20%E5%BF%AB%E6%8D%B7%E9%94%AE%20cmd%2Bb%20%E5%AD%97%E4%BD%93%E5%8F%98%E6%96%9C%EF%BC%9A%2A%E9%9C%80%E8%A6%81%E6%96%9C%E4%BD%93%E7%9A%84%E6%96%87%E5%AD%97%2A%20%E5%BF%AB%E6%8D%B7%E9%94%AE%20cmd%2Bi,%E8%8D%A7%E5%85%89%E6%95%88%E6%9E%9C%EF%BC%9A%3D%3D%E8%8D%A7%E5%85%89%E6%95%88%E6%9E%9C%E6%96%87%E5%AD%97%3D%3D%20%E5%BF%AB%E6%8D%B7%E9%94%AE%20cmd%2Bh%20%E5%BB%BA%E7%AB%8B%E5%BC%95%E7%94%A8%EF%BC%9A%E8%BE%93%E5%85%A5%E5%90%91%E5%8F%B3%E7%9A%84%E5%B0%96%E6%8B%AC%E5%8F%B7%20%3E%20%E7%84%B6%E5%90%8E%E8%BE%93%E5%85%A5%E6%96%87%E5%AD%97)



-shared 生成共享目标文件，即dll
gcc --share print.c -o print.dll
链接程序与动态库
gcc test.c print.dll -o test













保护机制
	Canary嗅探，cookie
	ASLR
	NX 将数据页标识为不可执行，防止溢出攻击
	地址分页
	PIE（linux）

ASLR与PIE的区别


关闭保护指令
[PWN入门系列（四）：栈终结篇 - bonelee - 博客园 (cnblogs.com)](https://www.cnblogs.com/bonelee/p/13789378.html)
[gcc安全编译选项详解（NX(DEP)、RELRO、PIE(ASLR)、CANARY、FORTIFY）_gcc pie-CSDN博客](https://blog.csdn.net/tabactivity/article/details/126660974)

gcc -g -fno-stack-protector -z execstack -no-pie -z norelro  -m32   overflow.c  -o  overflow2 
	gcc -g  调试符号
	-fno-stack-protector   - 栈溢出保护CANARY
	-z execstack   -NX
	-no-pie         -PIE
	-z norelro    -RELRO- 设置符号重定向表格为只读
	-m32   overflow.c  -o  overflow2 
	-Wall 编译时回弹警告信息
	
checksec overflow2 

gcc -Wall -g -fno-stack-protector -z execstack -no-pie -z norelro  -m32   overflow.c  -o  overflow2 

gcc -g   -m32   overflow.c  -o  overflow2 
[聊聊Linux动态链接中的PLT和GOT（１）——何谓PLT与GOT_plt got-CSDN博客](https://blog.csdn.net/linyt/article/details/51635768)

[GCC 参数详解 | 菜鸟教程 (runoob.com)](https://www.runoob.com/w3cnote/gcc-parameter-detail.html)

[CPU的实模式和保护模式(一) - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/42309472)
	[「学习笔记」对实模式/保护模式的三种访问内存机制的理解 - 幼麟 - 博客园 (cnblogs.com)](https://www.cnblogs.com/bEngi1/p/12173719.html)
	[操作系统篇-分段机制与GDT|LDT - 卫卐 - 博客园 (cnblogs.com)](https://www.cnblogs.com/chenwb89/p/operating_system_003.html#commentform)
