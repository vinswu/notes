# 快速装机笔记

## 安装前准备

#### 硬件：U盘、网络、备用电脑  
#### 软件：系统、PE、虚拟光驱 UltraISO、解压软件 7-zip、激活工具、运行库、驱动

##### 系统 下载
- MSDN,我告诉你 https://msdn.itellyou.cn/ 
- 远景Windows论坛 https://bbs.pcbeta.com/

##### PE 下载
- IT天空-优启通 http://www.usbzl.com/
- 微PE https://www.wepe.com.cn/
- 金狐系统维护盘 http://www.jinhu.me/
- 杏雨梨云启动维护系统 https://www.xyboot.com/  
> 加餐：[无忧启动论坛](http://bbs.wuyou.net/forum.php)

##### 虚拟光驱 下载
- UltraISO软碟通 https://cn.ezbsystems.com/ultraiso/download.htm  
> 简体中文版 注册信息  

| 注册名  | 注册码 |
| :--- | :--- |
| Guanjiu | A06C-83A7-701D-6CFC |
| 累累 | 4EE9-A156-B015-A70E |
| 李明 | 509F-BA54-BBA6-73C5 |
| 王涛 | 7C81-1689-4046-626F |

##### 解压软件 下载
- 7-zip https://www.7-zip.org/

##### 运行库 下载
- 微软常用运行库合集_果壳剥壳 https://www.ghxi.com/yxkhj.html
- 微软.NET运行库合集 https://www.ghxi.com/nethj.html
- 微软常用运行库合集_Dreamcast http://dreamcast2.ysepan.com/
- VisualCppRedist AIO https://github.com/abbodi1406/vcredist
> 加餐：《Windows常用运行库（VC++、DirectX、.NET）》 https://blog.csdn.net/cbing2002/article/details/121263687

#### 激活工具 下载一 知彼而知己HEU_KMS_Activator https://github.com/zbezj/HEU_KMS_Activator
#### 激活工具 下载二 ZD423Down_Microsoft_Activation_Tools https://pan.lanzou.com/b0f1t9l0b

#### IT天空-万能驱动 下载一 http://www.wandrv.com/
#### 驱动精灵 下载二 http://www.drivergenius.com/
#### 360驱动大师 下载三 http://www.drivergenius.com/


# 进PE开始安装
## 快速分区：DiskGenius（原PartitionGuru）
#### 分区表类型选择
Windows7 及以下，MBR格式，Legacy启动模式
Windows8 及以上，GUID（GPT）格式，UEFI启动模式
###### 加餐：《BIOS中的UEFI和Legacy启动模式》 https://blog.csdn.net/z15732621736/article/details/49048779
###### 加餐：《硬盘分区表格式GUID和MBR知识普及》 https://blog.csdn.net/z15732621736/article/details/49046367
#### 4K对齐
[勾选] 对齐分区到此扇区数的整数倍：[固态硬盘选4096扇区/机械硬盘2048扇区]
###### 加餐：《分区4K对齐那些事，你想知道的都在这里》 https://diskgenius.cn/exp/about-4k-alignment.php

## 系统安装：WinNTSetup
#### 选择包含Windows安装文件的文件夹
选 X:\sources\install.wim

#### 选择引导驱动器 （右侧三盏灯，绿灯、黄灯均为正常，若亮红灯说明选择引导驱动器磁盘选择错误）
选 C盘 或 引导盘

#### 安装磁盘的位置
选 C盘

#### 开始安装
引导扇区 [使用bootsect.exe 更新引导代码] [ALL]
关机：[勾选]安装成功后自动重新启动计算机


# 进入系统并完成安装
## 开启Administrator账户

## 激活系统（提前准备的激活工具）

## 安装运行库（提前准备的微软常用运行库合集）

## 安装驱动（提前准备的驱动）


# 我的 Windows Apps
## 科学上网工具
#### 科学上网工具 下载一 ShadowsocksR https://github.com/HMBSbige/ShadowsocksR-Windows/releases
#### 科学上网工具 下载二 Clash https://github.com/Fndroid/clash_for_windows_pkg/releases
###### 加餐：《SS/SSR免费账号/节点（长期更新）》 https://github.com/Alvin9999/new-pac/wiki/ss免费账号

## 浏览器
#### Google Chrome https://www.google.com/chrome/

## 输入法
#### 讯飞输入法 https://srf.xunfei.cn/

## 系统优化维护
#### 腾讯电脑管家 https://guanjia.qq.com/
#### WPD https://wpd.app/
#### Geek Uninstaller https://geekuninstaller.com/

## 腾讯聊天套件
#### TIM https://office.qq.com
#### 微信 https://weixin.qq.com/
#### 腾讯会议 https://meeting.tencent.com/

## 常用办公软件
#### Microsoft Office https://www.office.com/
###### 加餐：Office Tool Plus https://otp.landian.vip/zh-cn/
#### Adobe Acrobat / Adobe Photoshop .. https://www.adobe.com/cn/
###### 加餐：vposy_Adobe全家桶 https://weibo.com/vposy
#### Xmind https://www.xmind.cn/
#### 桌面日历 https://chs.desktopcal.com/chs/
#### 企业微信 https://work.weixin.qq.com/
#### 钉钉 https://www.dingtalk.com/
#### 飞书 https://www.feishu.cn/

## 看图
#### FastStone Image Viewer https://www.faststone.org/FSViewerDetail.htm
#### XnView Shell Extension https://www.xnview.com/en/xnshell/

## 截图/录屏
#### Snipaste https://www.snipaste.com/
#### ScreenToGif https://github.com/NickeManarin/ScreenToGif

## 听音乐
#### AIMP https://www.aimp.ru/
#### Listen 1 音乐播放器 https://listen1.github.io/listen1/

## 看视频
#### Potplayer https://potplayer.daum.net/

## 个性化
#### Bing Wallpaper https://www.microsoft.com/zh-cn/bing/bing-wallpaper
#### f.lux https://justgetflux.com/
#### FlipIt https://github.com/phaselden/FlipIt/releases
