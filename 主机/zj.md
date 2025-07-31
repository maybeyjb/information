#主机

操作系统识别：

1、Web大小写：网站路径大小写改动、

2、端口服务特征：ssh---- 22 ----- linux   	远程终端----3389----windows（rdp）

3、TTL值判断返回：ping 命令返回ttl值。

![image-20250304092954187](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451794.png)

## IP资产

归属地查询------比如上面的ping  xiaodi8得到的ip，然后查ip归属为香港阿里云。

归属云厂商 

IP反查机构

IP反查域名 

![image-20250304160849700](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451795.png)

IP-C段查询：112.11.123.1-255  这就是c段，因为有的大型公司会买一个段都是自己的资产。

这里可以转换成Web上，机构上，从而获取更多信息

### 端口扫描

 网络引擎

fofa有时间延迟，最新的网站是找不到。

![image-20250304161428097](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451797.png)

2、在线端口扫描：百度或google直接搜索在线端口扫描就会有一些网站，同理很多功能都可以直接搜索在线xxx；例如在线正则提取解析、在线编码转换等。

![image-20250304161653859](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451798.png)

#### 工具：

工具就是实时的，网络测绘是有延迟的：

 	nmap（有点慢）、masscan、fscan（内网常用探测，体积小）、yakit	无影

yakit：

![image-20250304162423058](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451799.png)

无影

![image-20250304163150491](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451800.png)

C段全端口：

![image-20250304163237513](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451801.png)

namp  支持换协议进行扫描端口：

![image-20250304163540110](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451802.png)

 防火墙拦截：换协议扫描，尝试。namp支持多种协议

协议是有多种的，所以是几率性绕过

![image-20250304170303782](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451803.png)

 内网拦截、通讯不到：让其外联，利用漏洞。比如ssrf，让其自己访问自己，进行探针。

  安全服务防火墙

就比如碰到了启明星辰的汉马防火墙，就用漏洞库打，测试。或者厂商的默认密码等：

![image-20250304172944239](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451804.png)

![image-20250304173007953](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451805.png)

