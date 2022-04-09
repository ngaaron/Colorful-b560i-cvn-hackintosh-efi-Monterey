# Hackintosh Monterey EFI B560i cvn
* A Hackintosh Monterey EFI for Colorful B560i cvn + i7-10700 + R7 370


### EFI详情
* 支持MacOS版本：目前支持最新的Monterey 12.4 Beta版
* OpenCore版本：0.8.0
* 更新日期：2022年04月10日


### 配置清单
* 主板：Coloful CVN B560I GAMING FROZEN V20
* CPU：Intel i7-10700 八核心十六线程
* 显卡：Sapphire R7 370 蓝宝石
* 网卡：BCM94360CS/BCM94360CD/BCM943602CS 都用过可以完美免驱
* 内存：铭瑄/MAXSUN DDR4 2600MHZ 16GX2 （超频3600mhz）
* 固态硬盘：海康威视C2000 512G 
* 机械硬盘：西部数据 3T + 东芝 3T （1T作为TimeMachine备份）

### 完美程度
* 有线/无线耳机麦克风使用正常。
* 接力、随航功能正常使用。
* iMessage、FaceTime正常登陆使用。
* 有线网络/无线网络2G+5G正常使用。
* 前后各IO接口正常使用。
* 支持2k输出/4K未测试，显卡支持双显示器输出。
* 随眠唤醒不是100%成功。
* 独显硬件加速后续完善。
* 其他问题欢迎反馈，目前还在继续完善中。

### BIOS推荐设置
* 关闭 CSM启动
* 关闭 Secure Boot 安全启动
* 关闭 CFG Lock
* 开启 USB鼠标/键盘唤醒
* 开启 XHCI Hand-off（默认开启）
* 硬盘模式 SATA Mode: AHCI
* 其他设置似乎没有太大影响，我保持主板默认了。

### 使用说明
* 目前只测试了支持Monterey系统，并试过从12.3升级到12.4beta版。
* 尝试了放在BigSur的启动盘使用能够成功进入安装界面安装系统，已有系统就没有继续安装了。

### 可能问题及解决方案
* 更新完系统后没有Hipi的话，可以使用one-key-hidpi-master脚本一键开启。
* 系统可以正常休眠，不过睡眠唤醒不是100%能成功，建议在节能中设置「防止系统进入睡眠」。
* 如果无法登陆使用iMessage和FaceTime等功能，可以自行替换三码和ROM参数，详细可以参考下方链接。

### Fixing iMessage and other services with OpenCore
* [https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#clean-out-old-attempts](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#clean-out-old-attempts)
