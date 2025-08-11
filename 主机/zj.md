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

<img width="1367" height="841" alt="image" src="https://github.com/user-attachments/assets/07d1ee3a-eed6-42fb-b2a8-bca388adc4e1" />


无影

<img width="1367" height="567" alt="image" src="https://github.com/user-attachments/assets/1914c1ad-72c4-43eb-8fae-9dc97d38da9b" />


C段全端口：

<img width="1367" height="839" alt="image" src="https://github.com/user-attachments/assets/96adf472-3e66-4fee-bd95-9e4c047b0ce3" />


namp  支持换协议进行扫描端口：

<img width="1367" height="889" alt="image" src="https://github.com/user-attachments/assets/f637d3dc-67b0-482f-8bed-81837b1d902f" />


 防火墙拦截：换协议扫描，尝试。namp支持多种协议

协议是有多种的，所以是几率性绕过

![image-20250304170303782](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451803.png)

 内网拦截、通讯不到：让其外联，利用漏洞。比如ssrf，让其自己访问自己，进行探针。

  安全服务防火墙

就比如碰到了启明星辰的汉马防火墙，就用漏洞库打，测试。或者厂商的默认密码等：

<img width="1367" height="800" alt="image" src="https://github.com/user-attachments/assets/9e999f0c-295f-4cd1-8415-b98dec4b1fb2" />


![image-20250304173007953](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451805.png)

