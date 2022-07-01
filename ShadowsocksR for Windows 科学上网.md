## ShadowsocksR for Windows 科学上网

#### 下载ShadowSocksR

>ShadowsocksR（简称SSR）  
>https://github.com/shadowsocksr/shadowsocksr-csharp （项目已删除）  
>最后windows版本ShadowsocksR-4.7.0-win.7z（已发现问题：PAC更新失效）  
>备份下载  
>https://github.com/shadowsocksr-backup/shadowsocksr-csharp/releases
>
>ShadowSocksR-RM （仅修复PAC更新链接，更新为ShadowsocksR-4.7.0.1-win.7z）  
>https://github.com/shadowsocksr-rm/shadowsocksr-csharp/releases
>
>ShadowSocksR项目停止后，一个较受欢迎的分支ShadowSocksRR（简称SSRR）  
>https://github.com/shadowsocksrr/shadowsocksr-csharp/releases
>
>ShadowsocksR for Windows （HMBSbige）  
>https://github.com/HMBSbige/ShadowsocksR-Windows/releases
	
#### 运行ShadowSocksR

>解压后，直接运行ShadowsocksR-dotnet2.0或exeShadowsocksR-dotnet4.0.exe  
>如果运行时提示错误，请先安装Microsoft .NET Framework 4  
>https://download.microsoft.com/download/9/5/A/95A9616B-7A37-4AF6-BC36-D6EA96C8DAAE/dotNetFx40_Full_x86_x64.exe
	
#### SSR服务器订阅

>右键任务栏通知区域的纸飞机 - 服务器订阅 - SSR服务器订阅设置 - Add - 在“网址”框中粘贴下面地址  
>https://raw.githubusercontent.com/AmazingDM/sub/master/ssrshare.com （ 来自 [SSR小工具](https://www.ssrtool.com) ,网站被墙）  
>把“自动更新”勾上 - 确认  
>右键任务栏通知区域的纸飞机 - 服务器订阅 - 更新SSR服务器订阅（不通过代理）  
>等SSR服务器订阅更新完成（后，可以把ShadowSocksR自带的那个没有用的服务器删掉 ）  
>右键任务栏通知区域的纸飞机 - 服务器 - WWW.SSRTOOL.COM - 选择一个国外的服务器  
>www.google.com 测试

#### 软件设置

>系统代理模式 - PAC模式  
>PAC - 更新PAC为GFWList  
>系统代理模式 - 全局模式  
>代理规则 - 绕过局域网和大陆  
>服务器订阅 - SSR服务器订阅设置 - 自动更新（勾选）  
>服务器负载均衡（如果前面打了勾，把勾去掉）  
>选项设置 - 切换服务器前断开所有连接（勾选） #SSRR v4.9.1更新  
>端口设置（默认）  
	
#### 小技巧

- 快速选择服务器节点  
`鼠标滚轮单击任务栏通知区域的纸飞机，可以直接打开“服务器 - 服务器连接统计”`
	
- 同wifi的移动设备通过pc端ssr实现http代理  
`pc端ssr设置：选项设置\本地代理\（勾选）允许来自局域网的连接\本地端口“1080”`  
`移动端无线局域网设置：wifi信息\http代理（配置代理）\手动\服务器“pc端所连wifi的ipv4地址”\端口“1080”`

#### 免费节点（临时应急）

https://github.com/Alvin9999/new-pac/wiki/ss免费账号  免费SS/SSR账号/节点列表（长期更新）

https://lncn.org/  每周一晚和周五凌晨更新。一键复制所有节点 - 批量导入SSR://链接

https://free-ss.site/  优先选择V/T/U/M为10↑/10↑/10↑/10↑的节点

#### 免费机场推荐

[GetfreeCloud](https://portal.getfree.cloud/auth/register?code=fxaq  "需每天签到领流量")  邀请码`fxaq`

#### 付费机场推荐

[ADSL.Cloud](https://portal.adsl.cloud/auth/register?code=kxL1  "低至2元每月")  邀请码`kxL1`


#### VPS 服务商（支持支付宝）

[VULTR](https://www.vultr.com/)

[BandwagonHost](https://bandwagonhost.com/)

[CloudCone](https://cloudcone.com/)

[Host1Plus](https://www.heficed.com/)

#### 深入学习

[ShadowsocksR @ 维基百科](https://zh.wikipedia.org/wiki/Shadowsocks#ShadowsocksR)

[ShadowsocksR 客户端 小白使用教程](https://doubibackup.com/jeptq9ir-2.html)

[逗比根据地](https://doubibackup.com/)

[SSR中文网](https://ssr.tools/)

[翻墙党论坛](https://fanqiangdang.com/)
