#web网站

域名:

1、备案信息  

<img width="1365" height="350" alt="image" src="https://github.com/user-attachments/assets/5b1ec76c-cf85-4c72-a615-f5656ac759f6" />


2、企业产权  app，小程序等。     小蓝本、爱妻查、企查查等

查到网站的企业，就可以查看其下的其他域名或者网站、app资产等：

<img width="1366" height="666" alt="image" src="https://github.com/user-attachments/assets/691d8cf7-90dd-4bad-9d0b-56fb40b6c5f8" />


<img width="1367" height="543" alt="image" src="https://github.com/user-attachments/assets/e090d811-34cb-4122-8d87-e7720a7d39ea" />


3、域名相关性

![image-20250304122055897](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451809.png)

### whois

​	whois信息。联系人，联系邮箱等信息。

![image-20250304181406887](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451810.png)

子域名：

autohome.com.cn 	autohome.com	autohome.cn  就这种

通过查域名是否被使用来查找子域名。

![image-20250304182338655](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451811.png)s

还可以爆破域名。

![image-20250304183405160](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451812.png)

1、DNS数据

​	以DNS解析历史记录查询域名资产	

2、证书查询

以SSL证书解析查询域名资产

3、网络空间 

多网络空间综合型获取的记录

4、威胁情报

各类接口的集成的记录

5、枚举解析

结果主要以字典决定

https://github.com/knownsec/ksubdomain 子域名。

https://github.com/shmilylty/OneForAll

ksubdomain ：	

有时候会有误报，因为域名解析，比如说*.xiaodi8.com 的dns解析，这时候就会出现 * 会当作域名解析，所以就需要看一些有意义的前缀 ，比如a.xiaodi8.com  b.xiaodi8.com这种可能就是误报。

ksubdomain.exe -d  autohome.com.cn

![image-20250304205158001](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451813.png)

6、JS提取子域名

比如说未授权一些接口。


# web指纹

指纹识别，看是不是开源的cms，使用什么语言（比如看尾缀.php），什么框架组件。

可能就算是开源，有源码也是加密的，比如通达OA。

判断数据库类型：端口扫描、或者组合判断：lnmp---linux+nginx+mysql+php          

wamp---------windows+apache+mysql+php 

![image-20250306121638142](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451814.png)

cdn怎么识别厂商：

就ping后在百度上查。

就根据ping后的域名，或者ip分布是哪家厂商的：

![image-20250306224837894](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451815.png)



指纹识别：在线网站识别、推荐云悉，但是要邀请码。

![image-20250306225309408](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451816.png)

#### 工具

 工具指纹识别 、主要有价值的就是看是什么cms的（不过大厂都是自己开发的，可能旁站是用开源的cms）

ehole_windows

![image-20250306225641668](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451817.png)

hfinger

![image-20250306225737115](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451818.png)

wappalyzer插件：

![image-20250306225807664](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451820.png)



 使用图标识别cms

查看网站前端源码，找到icon图标、保存

![image-20250306230530901](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451821.png)

使用刚才保存的网页图标进行搜索：

![image-20250306230846459](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451822.png)

就搜到了图标ico的结果，就是使用这个网站同一个图标的各个网站：

![image-20250306230937941](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451823.png)

当然如果这个公司将图标改了，那么就会搜不到或者识别不到。

  工具识别waf种类---------云waf

类似碰到这种情况就是被waf拦截了：

![image-20250306231240224](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451824.png)

identYwaf.py 

![image-20250306231734999](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451825.png)

wafw00f![image-20250306232754443](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451826.png)

#### 蜜罐识别

 蜜罐产品   一般在红蓝对抗，hw，演练中常见。现实或者实战少。	原理就是调试数据包

![image-20250306233922235](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451827.png)



 kuake有工具检测蜜罐。需要加ip地址。特征：端口多也有规律性（比如说端口是连续开放着），也不一定，有些单服务也可能只开一个。

![image-20250306183158526](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451828.png)

quake.exe：

![image-20250306234610521](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451829.png)

![image-20250306234748089](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451830.png)

 	若依里面有shiro框架，就你懂这个cms，你就了解它用的什么组件框架。或者不知道但是知道cms，那么也可以查这种cms用的什么框架之类的。

![image-20250306235307014](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451831.png)

# 源码获取

已知指纹后，就可以找到对应的源码框架。

![image-20250306210416832](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451832.png)

 工具测试是否存在git源码泄露，并下载解析。然后找里面的配置文件等。

IDEA比如说打开会自动产生一个.idea文件，就是保存你当前的状态，备份的，就是记住你上次对文件更改的操作，方便下次你打开还原到上次的状态。那么git源码泄露就是这个原理。

![image-20250307213455651](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451833.png)

跑出来的源码在工具脚本下的目录中

![image-20250307214019182](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451834.png)

 svn泄露，还是用工具扫。

原因是源码开发或者备份的时候忘记删了。

![image-20250307214701715](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451835.png)

DS_Store泄漏：

ds_store_exp.py

![image-20250307214742981](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451836.png)

composer.json-未知指纹识别获取源码途径--------- php的，就和python里面的pip、java里面的maven这类库一样

![image-20250307215527019](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451837.png)

  备份为zip文件：

还是工具可以直接扫的。

 webpack打包器，只能看到前端的泄露。

#### 平台搜索

借助资源平台去搜索（GitHub  gitee   oschina）、搜也是搜一些有特点，特征性比较强的文件。

![image-20250307221321527](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451838.png)

就比如这种有特征的文件，然后对应着找到了zblog的源码地方：

![image-20250307221017879](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451839.png)



hc  sese方面的。

![image-20250307221512897](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451840.png)

![image-20250307221632381](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451841.png)

#js信息收集

![image-20250307133805604](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451842.png)

#### 人工分析

  演示

![image-20250307134135198](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451843.png)

src=

![image-20250307222147616](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451844.png)

![image-20250307223021944](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451845.png)



#### 项目工具

从js中可以提取到有价值的信息：

  ffuf模糊测试



jsfinder-----有点落后。

linkfinder-------也不太行。

urlfinder--------jsfinder升级版。还不错、爬虫的原理

![image-20250307223554851](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451846.png)

  burpapifinder-较推荐 	apifinder

![image-20250307230749783](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451847.png)

findsoming

![image-20250307223048231](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451848.png)

 在线更新字典[Assetnote Wordlists](https://wordlists.assetnote.io/)	

fuzz模糊测试（fuff工具较快）、跑js路径有点像目录

![image-20250307231851998](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451849.png)

#### webpack

 webpack：用工具测试

![image-20250307232246106](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451850.png)

jjjjjjjjjjjjjs_windows_amd64_v2.4.0:

![image-20250307232809383](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451851.png)

PackerFuzzer.py

![image-20250307233221931](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451852.png)

下载出来可能是加密的。

案例
