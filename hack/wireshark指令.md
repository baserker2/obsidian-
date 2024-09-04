指令基础
[Wireshark 基本语法-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1442007)

**1.过滤IP，如来源IP或者目标IP等于某个IP**
ip.src eq 192.168.28.1 or ip.dst eq 192.168.28.1
或者
ip.addr eq 192.168.1.107 // 都能显示来源IP和目标IP

**2.过滤端口**
	tcp.port eq 80 // 不管端口是来源的还是目标的都显示
	tcp.port == 80
	tcp.port eq 2722
	tcp.port eq 80 or udp.port eq 80
	tcp.dstport == 80 // 只显tcp协议的目标端口80
	tcp.srcport == 80 // 只显tcp协议的来源端口80
	udp.port eq 15000
	过滤端口范围
	tcp.port >= 1 and tcp.port <= 80

**3.过滤协议**

**4.过滤指定字符**

**5.http模式过滤**
	http.request.method == “GET”
	http.request.method == “POST”
	http.request.uri == “/img/logo-edu.gif”
	http contains “GET”
	http contains “HTTP/1.”
	例：过滤GET请求
	http contains "GET"
	// GET包
	http.request.method == “GET” && http contains “Host: “
	http.request.method == “GET” && http contains “User-Agent: “
	// POST包
	http.request.method == “POST” && http contains “Host: “
	http.request.method == “POST” && http contains “User-Agent: “
	// 响应包
	http contains “HTTP/1.1 200 OK” && http contains “Content-Type: “
	http contains “HTTP/1.0 200 OK” && http contains “Content-Type: “
	一定包含如下
	Content-Type:

[使用wireshark过滤/查找协议里面的特定内容_wireshark过滤报文内容-CSDN博客](https://blog.csdn.net/Fems_123_/article/details/118188389?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522170022561116800182768170%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=170022561116800182768170&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-118188389-null-null.142^v96^pc_search_result_base1&utm_term=%E4%BD%BF%E7%94%A8wireshark%E8%BF%87%E6%BB%A4%2F%E6%9F%A5%E6%89%BE%E5%8D%8F%E8%AE%AE%E9%87%8C%E9%9D%A2%E7%9A%84%E7%89%B9%E5%AE%9A%E5%86%85%E5%AE%B9&spm=1018.2226.3001.4187)】

