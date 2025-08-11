# 框架组件

识别框架

通达oa、致远oa 、泛微oa 、xxxcms

#### pythons

  框架py的django、插件识别

或者图标识别

![image-20250308165117344](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451865.png)s



![image-20250309125248372](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451866.png)





![image-20250308165107541](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451867.png)

像这些图标，就可能是某些团体或者公司用的flask的框架开发的：

![image-20250309125735308](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451868.png)



Tornado

![image-20250308165638244](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451869.png)

![image-20250309130829958](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451870.png)

![image-20250309130856077](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451871.png)



#### JavaScript

-开发框架 	Vue&Node.js

前端数据传输，美化的

![image-20250308165601544](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451872.png)

![image-20250309131042598](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451873.png)

Node.js

![image-20250308165700869](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451874.png)

![image-20250309131350571](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451875.png)





#### php

有时候有些图标可能是一个团队或者个人研发的。只是用到了thinkphp的图标

![image-20250308170040526](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451876.png)

 	ThinkPHP：

![image-20250308165934784](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451877.png)



  Laravel：

![image-20250308172812667](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451878.png)

![image-20250309132939915](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451879.png)



Yii:

![image-20250308172835917](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451880.png)

#### Java

框架组件

SpringBoot：

![image-20250309133111238](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451881.png)

这些都是有关联的，比如你的oa系统用到了shiro框架，那么shiro框架爆出来漏洞，oa就也会被影响到。上面主要还是识别框架的特征。

 nuclei  项目自带各个框架版本的Poc。

[【实用工具】nuclei 安全扫描工具修改模板默认保存位置_nuclei更新模板-CSDN博客](https://blog.csdn.net/weixin_54430466/article/details/145636178?ops_request_misc=%7B%22request%5Fid%22%3A%22650e9fac6695e983eeba0f4e8665f50c%22%2C%22scm%22%3A%2220140713.130102334.pc%5Fall.%22%7D&request_id=650e9fac6695e983eeba0f4e8665f50c&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_ecpm_v1~rank_v31_ecpm-1-145636178-null-null.142^v102^pc_search_result_base9&utm_term=nuclei库怎么换位置&spm=1018.2226.3001.4187)

他会将这里默认下载，后续需要改一下

![image-20250309134244992](https://cdn.jsdelivr.net/gh/maybeyjb/maybe/img/202506121451882.png)

这工具也可以扫，然后识别你的框架。



#app

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

  其他工具，但是迪宝不推荐，先用手工测试收集app的信息。
