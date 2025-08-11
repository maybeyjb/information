
# app

隐私合规、app使用过程中的权限是否是通过用户授权得到。

1、逆向

2、渗透

 分析动态抓包、静态反编译：

  演示、对比抓包和反编译的区别。自动提取一些地址，资产。

![image-20250308232535457](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451883.png)

#### 静态：

app.py工具：![image-20250309140356876](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451884.png)

提取到的信息：

![image-20250309140904173](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451885.png)

apkleaks.py:

![image-20250309141013379](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451886.png)

会将结果放到txt文件中，里面有一些apikey、key或者域名的信息。

####  动态调试：



![image-20250308232557078](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451887.png)

mobsf工具，测试软件app的。

直接run.bat然后在上传目标apk文件。

![image-20250309144042536](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451889.png)

上传看分析结果：

![image-20250309144248716](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451890.png)

分apk里的一些功能，资产，隐私合规等。

也支持hook，动态调试等功能

![image-20250309145424798](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451891.png)

  使用逍遥模拟器可以用mobsf进行动态调试。证书测试、绕过证书校验（就可以抓包了）等方面。

但是这个动态调试不太方便，所以后期会介绍一些其他工具，面具这类。

hook绕过限制抓包，调试。

会自动获取模拟器上的app文件、点击即可进行动态调试。

![image-20250309145751130](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451892.png)

具体后续绕过ssl协议、证书之类的后面app课程细讲。主要还是逆向方面的知识。

![image-20250309180840833](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451893.png)

  apk app获取：

通过app的公司、进行小蓝本查旗下的其他app产品。开发者查找

![image-20250309150856471](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451894.png)

ios的反编译较难，不开源。鸿蒙也是。就安卓好弄点。

  其他工具，不推荐，先用手工测试收集app的信息。
