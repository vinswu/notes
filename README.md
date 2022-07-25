# 【我的快速装机笔记】

## 安装前的准备

#### 硬件：U盘、网络、备用电脑  
#### 软件：系统、PE、镜像刻录工具UltraISO、解压缩工具7-zip、激活工具、运行库、驱动

##### 系统 下载
- MSDN,我告诉你 https://msdn.itellyou.cn/ 
- 远景Windows论坛 https://bbs.pcbeta.com/

##### PE 下载
- IT天空-优启通 http://www.usbzl.com/
- 微PE https://www.wepe.com.cn/
- 金狐系统维护盘 http://www.jinhu.me/
- 杏雨梨云启动维护系统 https://www.xyboot.com/  
> 拓展：[无忧启动论坛](http://bbs.wuyou.net/forum.php)

##### 镜像刻录工具 下载
- UltraISO软碟通 https://cn.ezbsystems.com/ultraiso/download.htm  
> 简体中文版 注册信息  

| 注册名  | 注册码 |
| :--- | :--- |
| Guanjiu | A06C-83A7-701D-6CFC |
| 累累 | 4EE9-A156-B015-A70E |
| 李明 | 509F-BA54-BBA6-73C5 |
| 王涛 | 7C81-1689-4046-626F |

##### 解压缩工具 下载
- 7-zip https://www.7-zip.org/

##### 运行库 下载
- 微软常用运行库合集_果壳剥壳 https://www.ghxi.com/yxkhj.html
- 微软.NET运行库合集_果壳剥壳 https://www.ghxi.com/nethj.html
- 微软常用运行库合集_Dreamcast http://dreamcast2.ysepan.com/
- VisualCppRedist AIO https://github.com/abbodi1406/vcredist
- DirectX修复工具增强版 https://blog.csdn.net/vbcom/article/details/7245186
> 拓展：[《Windows常用运行库（VC++、DirectX、.NET）》](https://blog.csdn.net/cbing2002/article/details/121263687)

#### 激活工具 下载
- 知彼而知己HEU_KMS_Activator https://github.com/zbezj/HEU_KMS_Activator
- ZD423Down_Microsoft_Activation_Tools https://pan.lanzou.com/b0f1t9l0b

#### 驱动 下载
- 对应硬件官方服务支持下载中心
- IT天空-万能驱动 http://www.wandrv.com/
- 360驱动大师 http://www.drivergenius.com/
- 驱动精灵 http://www.drivergenius.com/

## 制作PE启动盘

#### PE 下载
- IT天空-优启通 http://www.usbzl.com/
- 微PE https://www.wepe.com.cn/
> 拓展：[无忧启动论坛](http://bbs.wuyou.net/forum.php)  

#### PE 制作（提前准备的U盘、PE、镜像刻录工具UltraISO）
> 拓展：[《微pe工具箱+软碟通 制作 U盘启动盘》](https://blog.csdn.net/yong53jun/article/details/118408973)  
> 拓展：[《ultraiso制作u盘启动盘教程图文详解纯净-U盘启动教程》](https://blog.csdn.net/qufuxiaozi/article/details/80124887)
> 拓展：[《Windows 重装系统-U盘启动盘制作及启动》](https://blog.csdn.net/m0_55483902/article/details/123496575)

#### U盘启动进PE
> 拓展：[《如何用U盘启动电脑(系统U盘使用最重要的步骤)》](https://zhuanlan.zhihu.com/p/81344150)

## 进PE后开始安装部署

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

## 进Windows系统完成安装

#### 开启Administrator账户
> 拓展：[《Win10如何启用Administrator账户》](https://blog.csdn.net/r875330957/article/details/79775494)  
> 拓展：[《Win10开启Administrator账户》](https://zhuanlan.zhihu.com/p/362058979)

#### 激活系统（提前准备的激活工具）
- 知彼而知己HEU_KMS_Activator https://github.com/zbezj/HEU_KMS_Activator
- ZD423Down_Microsoft_Activation_Tools https://pan.lanzou.com/b0f1t9l0b

#### 安装运行库（提前准备的微软常用运行库合集）
- 微软常用运行库合集_果壳剥壳 https://www.ghxi.com/yxkhj.html
- 微软.NET运行库合集_果壳剥壳 https://www.ghxi.com/nethj.html
- 微软常用运行库合集_Dreamcast http://dreamcast2.ysepan.com/
- VisualCppRedist AIO https://github.com/abbodi1406/vcredist
- DirectX修复工具增强版 https://blog.csdn.net/vbcom/article/details/7245186
> 拓展：[《Windows常用运行库（VC++、DirectX、.NET）》](https://blog.csdn.net/cbing2002/article/details/121263687)

#### 安装驱动（提前准备的驱动）
- 对应硬件官方服务支持下载中心
- IT天空-万能驱动 http://www.wandrv.com/
- 360驱动大师 http://www.drivergenius.com/
- 驱动精灵 http://www.drivergenius.com/

## 我的 Windows Apps

#### 科学上网工具
- ShadowsocksR https://github.com/HMBSbige/ShadowsocksR-Windows/releases
- Clash https://github.com/Fndroid/clash_for_windows_pkg/releases
> 加餐：[《SS/SSR免费账号/节点（长期更新）》](https://github.com/Alvin9999/new-pac/wiki/ss免费账号)

#### 浏览器
- Google Chrome https://www.google.com/chrome/

#### 输入法
- 讯飞输入法 https://srf.xunfei.cn/

#### 系统优化维护
- 腾讯电脑管家 https://guanjia.qq.com/
- WPD https://wpd.app/
- Geek Uninstaller https://geekuninstaller.com/

#### 腾讯聊天套件
- TIM https://office.qq.com
- 微信 https://weixin.qq.com/
- 腾讯会议 https://meeting.tencent.com/

#### 常用办公软件
- 企业微信 https://work.weixin.qq.com/
- 钉钉 https://www.dingtalk.com/
- 飞书 https://www.feishu.cn/

#### 文案处理
- Microsoft Office https://www.office.com/
> [Office Tool Plus](https://otp.landian.vip/zh-cn/)
- Adobe Acrobat / Adobe Photoshop .. https://www.adobe.com/cn/
> [vposy_Adobe全家桶](https://weibo.com/vposy)
- Xmind https://www.xmind.cn/


#### 看图
- FastStone Image Viewer https://www.faststone.org/FSViewerDetail.htm
- XnView Shell Extension https://www.xnview.com/en/xnshell/

#### 截图/录屏
- Snipaste https://www.snipaste.com/
- ScreenToGif https://github.com/NickeManarin/ScreenToGif

#### 听音乐
- AIMP https://www.aimp.ru/
- Listen 1 音乐播放器 https://listen1.github.io/listen1/

#### 看视频
- Potplayer https://potplayer.daum.net/

#### 个性化
- 桌面日历 https://chs.desktopcal.com/chs/
- 必应壁纸 https://www.microsoft.com/zh-cn/bing/bing-wallpaper
- f.lux https://justgetflux.com/
- FlipIt https://github.com/phaselden/FlipIt/releases
