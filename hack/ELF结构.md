 __x86_get_pc_thunk_bx
 连接动态加载库
[ELF文件详解—初步认识-CSDN博客](https://blog.csdn.net/daide2012/article/details/73065204)

[从零解析ELF目标文件(附源码) - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/544198038)

[elf_inject/ELF文件详解.pdf at master · zn-cn/elf_inject (github.com)](https://github.com/zn-cn/elf_inject/blob/master/ELF%E6%96%87%E4%BB%B6%E8%AF%A6%E8%A7%A3.pdf)
[深入分析ELF文件结构及其载入过程_-fpie-CSDN博客](https://blog.csdn.net/weixin_46222091/article/details/108645592#:~:text=ELF%E6%96%87%E4%BB%B6%E7%94%B14%E9%83%A8%E5%88%86%E7%BB%84%E6%88%90%EF%BC%8C%E5%88%86%E5%88%AB%E6%98%AFELF%E5%A4%B4%EF%BC%88ELF%20header%EF%BC%89%E3%80%81%E7%A8%8B%E5%BA%8F%E5%A4%B4%E8%A1%A8%EF%BC%88Program%20header,table%EF%BC%89%E3%80%81%E8%8A%82%EF%BC%88Section%EF%BC%89%E5%92%8C%E8%8A%82%E5%A4%B4%E8%A1%A8%EF%BC%88Section%20header%20table%EF%BC%89%E3%80%82%20%E5%AE%9E%E9%99%85%E4%B8%8A%EF%BC%8C%E4%B8%80%E4%B8%AA%E6%96%87%E4%BB%B6%E4%B8%AD%E4%B8%8D%E4%B8%80%E5%AE%9A%E5%8C%85%E5%90%AB%E5%85%A8%E9%83%A8%E5%86%85%E5%AE%B9%EF%BC%8C%E8%80%8C%E4%B8%94%E5%AE%83%E4%BB%AC%E7%9A%84%E4%BD%8D%E7%BD%AE%E4%B9%9F%E6%9C%AA%E5%BF%85%E5%A6%82%E5%90%8C%E6%89%80%E7%A4%BA%E8%BF%99%E6%A0%B7%E5%AE%89%E6%8E%92%EF%BC%8C%E5%8F%AA%E6%9C%89ELF%E5%A4%B4%E7%9A%84%E4%BD%8D%E7%BD%AE%E6%98%AF%E5%9B%BA%E5%AE%9A%E7%9A%84%EF%BC%8C%E5%85%B6%E4%BD%99%E5%90%84%E9%83%A8%E5%88%86%E7%9A%84%E4%BD%8D%E7%BD%AE%E3%80%81%E5%A4%A7%E5%B0%8F%E7%AD%89%E4%BF%A1%E6%81%AF%E7%94%B1ELF%E5%A4%B4%E4%B8%AD%E7%9A%84%E5%90%84%E9%A1%B9%E5%80%BC%E6%9D%A5%E5%86%B3%E5%AE%9A%E3%80%82)

--GOT和PLT（ELF格式下结构）
[technovelty.org/linux/plt-and-got-the-key-to-code-sharing-and-dynamic-libraries.html](https://www.technovelty.org/linux/plt-and-got-the-key-to-code-sharing-and-dynamic-libraries.html)

[elf_inject/ELF文件详解.md at master · zn-cn/elf_inject (github.com)](https://github.com/zn-cn/elf_inject/blob/master/ELF%E6%96%87%E4%BB%B6%E8%AF%A6%E8%A7%A3.md)

https://ir0nstone.gitbook.io/notes/types/stack/aslr/plt_and_got
(更详细的网站)


ELF文件接结构
![[Pasted image 20231203200323.png]]
读写权限见chmod 777 文件读写权限（RWX）
![[Pasted image 20231203201446.png]]
段与节
![[Pasted image 20231203202414.png]]