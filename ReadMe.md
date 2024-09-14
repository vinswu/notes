# 【装机笔记】

## 一、安装前的准备

#### 硬件：U盘、网络、备用电脑  
#### 软件：系统、PE、镜像刻录工具、解压缩工具、激活工具、运行库、驱动

##### 系统 下载
- MSDN,我告诉你 https://msdn.itellyou.cn/ 
- 远景Windows论坛* https://bbs.pcbeta.com/

##### PE 下载
- IT天空优启通 http://www.usbzl.com/
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
- HashCheck Shell Extension 插件 https://code.kliu.org/hashcheck/

##### 运行库 下载
- 微软常用运行库合集-果壳剥壳 https://www.ghxi.com/yxkhj.html
- 微软.NET运行库合集-果壳剥壳 https://www.ghxi.com/nethj.html
- 微软常用运行库合集-Dreamcast http://dreamcast2.ysepan.com/
- VisualCppRedist AIO* https://github.com/abbodi1406/vcredist
- Microsoft .NET Framework 修复工具 https://support.microsoft.com/zh-cn/topic/microsoft-net-framework-修复工具可用-942a01e3-5b8b-7abb-c166-c34a2f4b612a
- DirectX修复工具 https://blog.csdn.net/VBcom/article/details/6962388
> 拓展：[《Windows常用运行库（VC++、DirectX、.NET）》](https://blog.csdn.net/cbing2002/article/details/121263687)
- Java Development Kit https://www.oracle.com/java/technologies/downloads/

#### 激活工具 下载
- 知彼而知己HEU_KMS_Activator* https://github.com/zbezj/HEU_KMS_Activator
- KMS_VL_ALL_AIO https://github.com/abbodi1406/KMS_VL_ALL_AIO
- [Windows7 永久激活](https://vinswu.lanzouw.com/b0e1vhsuh "密码 1024")
- [Windows10 永久激活](https://vinswu.lanzouw.com/b0e4zgb0b "密码 1024")

#### 驱动 下载
- 对应硬件官网的技术支持服务下载中心
- 联想驱动管理 https://newsupport.lenovo.com.cn/driveDownloads_index.html
- 360驱动大师 https://dm.weishi.360.cn/home.html
- IT天空万能驱动 http://www.wandrv.com/
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

## 三、进PE后开始部署安装系统

#### 快速分区：DiskGenius（原PartitionGuru）

###### 分区表类型选择
- Windows7 及以下，MBR格式，Legacy启动模式
- Windows8 及以上，GUID（GPT）格式，UEFI启动模式
> 拓展：[《BIOS中的UEFI和Legacy启动模式》](https://blog.csdn.net/z15732621736/article/details/49048779)  
> 拓展：[《硬盘分区表格式GUID和MBR知识普及》](https://blog.csdn.net/z15732621736/article/details/49046367)

###### 4K对齐
- [勾选] 对齐分区到此扇区数的整数倍：[固态硬盘选4096扇区/机械硬盘2048扇区]
> 拓展：[《分区4K对齐那些事，你想知道的都在这里》](https://diskgenius.cn/exp/about-4k-alignment.php)

#### 系统安装：WinNTSetup

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
> 拓展：[《Win10如何启用Administrator账户》](https://blog.csdn.net/r875330957/article/details/79775494)  
> 拓展：[《Win10开启Administrator账户》](https://zhuanlan.zhihu.com/p/362058979)

#### 激活系统（工具看“安装前的准备”）

#### 安装运行库（工具看“安装前的准备”）

#### 安装驱动（工具看“安装前的准备”）

## 附：我的 Windows Apps

#### 解压缩&文件校验工具
- 7-zip* https://www.7-zip.org/
- WinRAR https://www.rarlab.com/
- 360压缩 https://yasuo.360.cn/
- Hash https://keir.net/hash.html
- HashCheck Shell Extension 插件 https://code.kliu.org/hashcheck/

#### 科学上网工具
- XX-Net https://github.com/XX-net/XX-Net
- ShadowsocksR https://github.com/HMBSbige/ShadowsocksR-Windows
- v2rayN https://github.com/2dust/v2rayN
- Clash Verge https://github.com/clash-verge-rev/clash-verge-rev
> 加餐：[《SS/SSR免费账号/节点（长期更新）》](https://github.com/Alvin9999/new-pac/wiki/ss免费账号)

#### 浏览器
- Mozilla Firefox https://www.mozilla.org/zh-CN/firefox/browsers/
- Google Chrome［H］* https://www.google.com/chrome/
- Microsoft Edge* https://www.microsoft.com/zh-cn/edge 

#### 输入法
- 紫光华宇拼音输入法 https://pinyin.thunisoft.com/
- 搜狗输入法 https://shurufa.sogou.com/
- 百度输入法 https://shurufa.baidu.com/
- 讯飞输入法* https://srf.xunfei.cn/

#### 系统维护辅助工具
- 360安全卫士 https://weishi.360.cn/ 
> [360安全卫士极速版](https://down.360safe.com/setupbeta_jisu.exe "点击下载")  
> [360安全卫士真的有那么不堪吗？](https://www.zhihu.com/question/333386410)  
- 腾讯电脑管家 https://guanjia.qq.com/
- 火绒安全* https://www.huorong.cn/
- 火绒应用商店* https://www.huorong.cn/app_store.html
- 联想电脑管家 https://guanjia.lenovo.com.cn/
- 联想应用商店 https://lestore.lenovo.com/
- 微软电脑管家 https://pcmanager.microsoft.com/
- Dism++ https://github.com/Chuyu-Team/Dism-Multi-language/releases *系统优化*
- WPD* https://wpd.app/ *系统优化*
- Geek Uninstaller* https://geekuninstaller.com/ *软件卸载*

#### 下载&网盘工具
- 迅雷 https://www.xunlei.com/
> [迅雷极速版_1.0.35.366](http://down.sandai.net/thunderspeed/ThunderSpeed1.0.35.366.exe "点击下载")
- 百度网盘* https://pan.baidu.com/
- 阿里云盘 https://www.aliyundrive.com/
- Internet Download Manager https://www.internetdownloadmanager.com/
> [重置IDM试用](https://github.com/malaohu/reset-idm-trial)

#### 聊天工具
- QQ/TIM* https://im.qq.com/
- 微信* https://weixin.qq.com/
- Telegram [H] https://telegram.org/

#### OA办公自动化
- 企业微信 https://work.weixin.qq.com/
- 钉钉 https://www.dingtalk.com/
- 飞书 https://www.feishu.cn/

#### 办公套件
- WPS https://www.wps.cn/
- Microsoft Office* / Project / Visio https://www.office.com/
> [Office Tool Plus](https://otp.landian.vip/zh-cn/)  
> [Mocreak](https://github.com/OdysseusYuan/Mocreak)  
> [LKY Office Tools](https://github.com/OdysseusYuan/LKY_OfficeTools)  
- Ohook https://github.com/asdcorp/ohook
- OfficePLUS 插件 https://www.officeplus.cn/addin/OPCN/
- Adobe Acrobat* / Photoshop / Premiere https://www.adobe.com/cn/
> [Adobe全家桶@vposy（暂停更新）](https://weibo.com/vposy)
- WebPShop 插件 https://helpx.adobe.com/cn/photoshop/kb/support-webp-image-format.html *在Photoshop中使用WebP文件*
- 万彩办公大师 http://www.wofficebox.com/
- NotepadNext https://github.com/dail8859/NotepadNext
- Qalculate! https://github.com/Qalculate/libqalculate
> [办公字体](https://vinswu.lanzoue.com/b0e50lpde "密码:1024")  

#### 笔记/思维导图
- OneNote 
- Effie* https://www.effie.co/
- Xmind https://www.xmind.cn/

#### 看图
- IrfanView* https://www.irfanview.com/
- FastStone Image Viewer [H] https://www.faststone.org/FSViewerDetail.htm
- XnView https://www.xnview.com/en/
- XnView Shell Extension 插件 https://www.xnview.com/en/xnshell/ *右键图片预览、格式转换、调整大小、等*
- FastPreview 插件* https://github.com/nmaier/fastpreview *右键图片预览*

#### 截图/gif动图录屏
- QQ截图*
- Snipaste* https://www.snipaste.com/
- ScreenToGif https://github.com/NickeManarin/ScreenToGif

#### 听音乐
- AIMP* https://www.aimp.ru/
- foobar2000 https://www.foobar2000.org/
- Listen 1 音乐播放器 https://listen1.github.io/listen1/

#### 音乐编辑
- Mp3tag https://www.mp3tag.de/ *音乐标签编辑*
- Exact Audio Copy https://exactaudiocopy.de/ *音轨抓取*
- Medieval CUE Splitter http://www.medieval.it/ *音轨切割*

#### 看视频
- VLC https://www.videolan.org/vlc/
- Potplayer* https://potplayer.daum.net/

#### 录视频
- QQ截图-屏幕录制
- OBS https://obsproject.com/zh-cn

#### 个性化
- 日历清单*（原：桌面日历） https://www.xdiarys.com/
- 必应壁纸 https://www.microsoft.com/zh-cn/bing/bing-wallpaper
- 微软桌面壁纸 https://lockscreen.microsoft.com/
- f.lux https://justgetflux.com/ *护眼*
- Fliqlo https://fliqlo.com/
- FlipIt* https://github.com/phaselden/FlipIt/releases *时钟屏保*
- noMeiryoUI https://github.com/Tatsu-syo/noMeiryoUI/releases *Windows系统字体修改*
