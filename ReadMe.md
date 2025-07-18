# 【我的装机笔记】

## 一、安装前的准备

#### 硬件：U盘、网络、备用电脑  
#### 软件：系统、PE、镜像刻录工具、解压缩工具、激活工具、运行库、驱动

##### 系统 下载
- MSDN,我告诉你 https://msdn.itellyou.cn/
- HelloWindows https://hellowindows.cn/
- 远景Windows论坛* https://bbs.pcbeta.com/

##### PE 下载
- IT天空优启通 https://www.itsk.com/
- 微PE（原：通用PE）* https://www.wepe.com.cn/
- 金狐系统维护盘 http://www.jinhu.me/
> 拓展：[FirPE](https://firpe.cn/)  
> 拓展：[杏雨梨云启动维护系统](https://www.xyboot.com/)  
> 拓展：[无忧启动论坛](http://bbs.wuyou.net/forum.php)  

##### 镜像刻录工具 下载
- Rufus https://rufus.ie/zh/
- UltraISO软碟通* https://cn.ezbsystems.com/ultraiso/download.htm  
> UltraISO软碟通 简体中文版 注册信息  

| 注册名  | 注册码 |
| :--- | :--- |
| Guanjiu | A06C-83A7-701D-6CFC |
| 累累 | 4EE9-A156-B015-A70E |
| 李明 | 509F-BA54-BBA6-73C5 |
| 王涛 | 7C81-1689-4046-626F |

##### 解压缩&文件校验工具 下载
- 7-zip* https://www.7-zip.org/
- WinRAR https://www.rarlab.com/
- Hash https://keir.net/hash.html
- HashCheck Shell Extension 插件* https://code.kliu.org/hashcheck/

##### 运行库 下载
- 微软常用运行库合集-果壳剥壳 https://www.ghxi.com/yxkhj.html
- 微软.NET运行库合集-果壳剥壳 https://www.ghxi.com/nethj.html
- 微软常用运行库合集-Dreamcast http://dreamcast2.ysepan.com/
- VisualCppRedist AIO* https://github.com/abbodi1406/vcredist
- Microsoft .NET Framework 修复工具 https://support.microsoft.com/zh-cn/topic/microsoft-net-framework-修复工具可用-942a01e3-5b8b-7abb-c166-c34a2f4b612a
- DirectX修复工具 https://blog.csdn.net/VBcom/article/details/6962388
- Adobe Flash Player https://www.flash.cn/
- Clean Flash Player https://github.com/darktohka/clean-flash-builds
- Java Development Kit* https://www.oracle.com/java/technologies/downloads/
> 拓展：[《Windows常用运行库（VC++、DirectX、.NET）》](https://blog.csdn.net/cbing2002/article/details/121263687)  
> 拓展：[《windows 10 配置Java 环境变量》](https://www.jianshu.com/p/9fc41ea941aa)

#### 激活工具 下载
- 知彼而知己HEU_KMS_Activator https://github.com/zbezj/HEU_KMS_Activator
- Microsoft Activation Scripts (MAS)* https://github.com/massgravel/Microsoft-Activation-Scripts

#### 驱动 下载
- 对应硬件官网的技术支持服务下载中心
- 联想驱动管理 https://newsupport.lenovo.com.cn/driveDownloads_index.html
- 360驱动大师 https://dm.weishi.360.cn/home.html
- IT天空万能驱动 https://www.itsk.com/
- 驱动总裁* https://www.sysceo.com/dc

## 二、制作PE启动盘

#### PE 下载
- 微PE https://www.wepe.com.cn/
> 拓展：[无忧启动论坛](http://bbs.wuyou.net/forum.php)  

#### PE 制作（提前准备的U盘、PE、镜像刻录工具UltraISO）
> 拓展：[《微pe工具箱+软碟通 制作 U盘启动盘》](https://blog.csdn.net/yong53jun/article/details/118408973)  
> 拓展：[《ultraiso制作u盘启动盘教程图文详解纯净-U盘启动教程》](https://blog.csdn.net/qufuxiaozi/article/details/80124887)  
> 拓展：[《Windows 重装系统-U盘启动盘制作及启动》](https://blog.csdn.net/m0_55483902/article/details/123496575)

#### U盘启动进PE
> 拓展：[《如何用U盘启动电脑(系统U盘使用最重要的步骤)》](https://zhuanlan.zhihu.com/p/81344150)

## 三、进WindowsPE，部署安装系统

#### 快速分区：[DiskGenius](https://www.diskgenius.com/)（原PartitionGuru）

###### 分区表类型选择
- Windows7 及以下，MBR格式，Legacy启动模式
- Windows8 及以上，GUID（GPT）格式，UEFI启动模式
> 拓展：[《BIOS中的UEFI和Legacy启动模式》](https://blog.csdn.net/z15732621736/article/details/49048779)  
> 拓展：[《硬盘分区表格式GUID和MBR知识普及》](https://blog.csdn.net/z15732621736/article/details/49046367)

###### 4K对齐
- [勾选] 对齐分区到此扇区数的整数倍：[固态硬盘选4096扇区/机械硬盘2048扇区]
> 拓展：[《分区4K对齐那些事，你想知道的都在这里》](https://diskgenius.cn/exp/about-4k-alignment.php)

#### 系统安装：[WinNTSetup](https://msfn.org/board/topic/149612-winntsetup)

###### 选择包含Windows安装文件的文件夹
- 选 X:\sources\install.wim

###### 选择引导驱动器 （右侧三盏灯，绿灯、黄灯均为正常，若亮红灯说明选择引导驱动器磁盘选择错误）
- 选 C盘 或 引导盘

###### 安装磁盘的位置
- 选 C盘

###### 开始安装
- 引导扇区 [使用bootsect.exe 更新引导代码] [ALL]
- 关机：[勾选]安装成功后自动重新启动计算机

## 四、进入Windows系统，激活优化系统并安装必要程序

#### 开启Administrator账户
> 拓展：[《Win10怎么开启Administrator超级管理员账户》](https://answers.microsoft.com/zh-hans/windows/forum/all/win10%E6%80%8E%E4%B9%88%E5%BC%80%E5%90%AFadministr/b7576403-c6dc-4fe1-b55a-3803f8fae320)

#### 激活系统（工具看“安装前的准备”）
> 拓展：[《如何激活Windows10》](https://answers.microsoft.com/zh-hans/windows/forum/all/%e5%a6%82%e4%bd%95%e6%bf%80%e6%b4%bbwindows10/ccd2dae7-76f6-49ea-89bc-0b02d2244514)

#### 安装运行库（工具看“安装前的准备”）

#### 安装驱动（工具看“安装前的准备”）

## 五、Windows装机软件精选

#### 解压缩&文件校验工具
- 7-zip* https://www.7-zip.org/
- WinRAR https://www.rarlab.com/
- Hash https://keir.net/hash.html
- HashCheck Shell Extension 插件 https://code.kliu.org/hashcheck/

#### [科学上网工具](https://github.com/vinswu/notes/blob/master/Agent.md)
- XX-Net https://github.com/XX-net/XX-Net
- Shadowsocks https://github.com/shadowsocks/shadowsocks-windows
- ShadowsocksR https://github.com/HMBSbige/ShadowsocksR-Windows
- v2rayN* https://github.com/2dust/v2rayN
- Clash for Windows https://github.com/Z-Siqi/Clash-for-Windows_Chinese
- Clash Verge https://github.com/clash-verge-rev/clash-verge-rev

#### 浏览器
- Mozilla Firefox https://www.mozilla.org/zh-CN/firefox/browsers/
- Tor Browser[H] https://www.torproject.org/zh-CN/download/
- Google Chrome*[H] https://www.google.com/chrome/
- Microsoft Edge https://www.microsoft.com/zh-cn/edge

#### 输入法
- 小狼毫输入法 https://rime.im/
- 紫光华宇拼音输入法 https://pinyin.thunisoft.com/
- 搜狗输入法 https://shurufa.sogou.com/
- 百度输入法 https://shurufa.baidu.com/
- 讯飞输入法* https://srf.xunfei.cn/

#### 系统维护辅助工具
- 360杀毒 https://sd.360.cn/
- 360安全卫士 https://weishi.360.cn/ *建议下载使用极速版*
- 火绒安全* https://www.huorong.cn/
- 火绒应用商店* https://www.huorong.cn/app_store.html
- 腾讯电脑管家 https://guanjia.qq.com/
- 微软电脑管家 https://pcmanager.microsoft.com/
- 图吧工具箱 https://www.tbtool.cn/
- Dism++ https://github.com/Chuyu-Team/Dism-Multi-language/releases *系统优化*
- WPD* https://wpd.app/ *系统优化*
- CCleaner https://www.ccleaner.com/zh-cn *垃圾清理*
- Geek Uninstaller https://geekuninstaller.com/ *软件卸载*


#### 下载&网盘工具
- Gopeed https://github.com/GopeedLab/gopeed
- eMule(电骡) http://emule-project.net
- BitComet(比特彗星) https://www.bitcomet.com/cn
- 迅雷 https://www.xunlei.com/
- 百度网盘 https://pan.baidu.com/
- 阿里云盘 https://www.aliyundrive.com/
- 夸克网盘 https://pan.quark.cn/
- 坚果云 https://www.jianguoyun.com/
- Internet Download Manager https://www.internetdownloadmanager.com/

#### 聊天工具
- Telegram*[H] https://telegram.org/
> 简体中文语言包 https://t.me/setlanguage/zh-hans-raw
- QQ https://im.qq.com/
- TIM* https://office.qq.com/
- 微信* https://weixin.qq.com/

#### OA办公自动化
- 企业微信 https://work.weixin.qq.com/
- 钉钉 https://www.dingtalk.com/
- 飞书 https://www.feishu.cn/

#### 办公基础套件
- Microsoft Office* / Project* / Visio* https://www.office.com/
> 安装 [Office Tool Plus](https://otp.landian.vip/zh-cn/) | [LKY Office Tools](https://github.com/OdysseusYuan/LKY_OfficeTools)  
> 激活 [Ohook](https://github.com/asdcorp/ohook)  
> 插件 [OfficePLUS*](https://www.officeplus.cn/addin/OPCN/)  
> 插件 [OfficeAI](https://www.office-ai.cn/)  
> [常用办公字体](https://vinswu.lanzoue.com/b0e50lpde "密码:1024")  
- Adobe Acrobat* https://www.adobe.com/
> 更新 [Acrobat Enterprise Release Notes](https://www.adobe.com/devnet-docs/acrobatetk/tools/ReleaseNotesDC/index.html)  
> 破解 [@vposy](https://weibo.com/vposy "2023年8月11日起暂停更新") | [@m0nkrus](http://www.monkrus.ws)  
> 插件 [WebPShop](https://helpx.adobe.com/cn/photoshop/kb/support-webp-image-format.html "在Photoshop中使用WebP文件")  
- WPS Office* https://www.wps.cn/
- WPS PDF https://www.wpspdf.cn/
- FreeOffice https://www.freeoffice.com/
- FreePDF https://www.getfreepdf.com/
- 数科OFD https://www.ofd.cn/

#### 办公增强工具
- 万彩办公大师 http://www.wofficebox.com/
- NotepadNext* https://github.com/dail8859/NotepadNext *替代记事本*
- Qalculate! https://github.com/Qalculate/libqalculate *替代计算器*
- DeepL https://github.com/DeepLcom/deepl-python *翻译*
- Stickies https://www.zhornsoftware.co.uk/stickies/ *桌面便签提醒*
> [Classic Apps](https://win7games.com/)

#### 笔记清单/思维导图
- 日历清单*（原：桌面日历） https://www.xdiarys.com/
- OneNote https://www.onenote.com/
- Notion https://www.notion.so/zh-cn
- Effie* https://www.effie.co/
- Xmind* https://www.xmind.cn/

#### 电子书阅读器
- calibre https://calibre-ebook.com
- Koodo Reader* https://www.koodoreader.com/
- Sumatra PDF https://www.sumatrapdfreader.org/free-pdf-reader

#### 看图
- ImageGlass https://imageglass.org/
- IrfanView* https://www.irfanview.com/
- XnView Shell Extension 插件 https://www.xnview.com/en/xnshell/ *右键图片预览、格式转换、调整大小、等*
- FastPreview 插件* https://github.com/nmaier/fastpreview *右键图片预览*

#### 截图/gif动图录屏
- QQ截图*
- ScreenCapture https://github.com/xland/ScreenCapture
- ShareX https://getsharex.com/
- Snipaste* https://www.snipaste.com/
- 小旺AI截图 https://www.xiaowang.com/
- ScreenToGif https://www.screentogif.com/
- FastStone Capture https://www.faststone.org/

#### 修图
- Adobe Photoshop* https://www.adobe.com/
- GIMP https://www.gimp.org/

#### 听音乐
- VLC https://www.videolan.org/vlc/
- AIMP* https://www.aimp.ru/
- foobar2000 https://www.foobar2000.org/

#### 音乐编辑
- Mp3tag https://www.mp3tag.de/ *音乐标签编辑*
- Exact Audio Copy https://exactaudiocopy.de/ *音轨抓取*
- Medieval CUE Splitter http://www.medieval.it/ *音轨切割*
- Sound Organizer https://www.sonystyle.com.cn/minisite/cross/app/sound_organizer.htm

#### 看视频
- VLC https://www.videolan.org/vlc/
- Potplayer* https://potplayer.daum.net/
- Emby https://emby.media/

#### 视频录制
- QQ截图-屏幕录制
- Captura https://github.com/MathewSachin/Captura
- OBS https://obsproject.com/zh-cn
- oCam* https://ohsoft.net/
> 注册 [@大眼仔~旭](https://www.dayanzai.me/ocam.html)

#### 视频编辑
- Adobe Premiere Pro* https://www.adobe.com/
- Kdenlive https://kdenlive.org/
- Shotcut https://www.shotcut.org/
- 剪映 https://www.capcut.cn/
- 格式工厂 http://www.pcgeshi.com/index.html

#### 个性化
- 必应壁纸 https://www.microsoft.com/zh-cn/bing/bing-wallpaper
- 微软桌面壁纸 https://lockscreen.microsoft.com/
- Fliqlo https://fliqlo.com/ *时钟屏保*
- FlipIt* https://github.com/phaselden/FlipIt/releases *时钟屏保*
- f.lux https://justgetflux.com/ *护眼*
- noMeiryoUI https://github.com/Tatsu-syo/noMeiryoUI/releases *Windows系统字体修改*

#### 小工具
- ContextMenuManager https://github.com/BluePointLilac/ContextMenuManager *右键菜单管理*
- MyComputerManager https://github.com/1357310795/MyComputerManager *此电脑内快捷方式管理*
- PdfInvoiceMerge https://github.com/hetaoos/PdfInvoiceMerge *PDF发票合并*
- 增值税电子发票阅读器 https://inv-veri.chinatax.gov.cn/xgxz.html
- 全国资格考试网报平台证件照片审核处理系统 http://www.cpta.com.cn/tooldown.html

## 外链
| [不忘初心系统博客](https://www.pc528.net/)
| [宋永志博客](http://www.songyongzhi.com/)
| [小众软件](https://www.appinn.com/)
| [异次元软件世界](https://www.iplaysoft.com/)
| [sysin](https://sysin.org/)
| [zd423](https://www.423down.com/)
