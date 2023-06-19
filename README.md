# MSI-B460M-WIFI_i7-10700_RX590
Intel i7 10700+MSI MAG B460M MORTAR WIFI+RX590 黑苹果

## 电脑配置

| 名称        | 型号                                        | 说明                                    |
| ----------- | ------------------------------------------- | --------------------------------------- |
| 显示器      | DELL U2720Q                                 | 4K  60Hz                                |
| CPU         | Intel® i7 10700                             |                                         |
| 主板        | 微星 MAG B460M MORTAR WiFi                  |                                         |
| 显卡        | Intel® UHD Graphics 630+迪兰DEVIL RX 590 8G | 支持核显加速                            |
| 内存        | DDR4 3200MHz 16G * 2                        |                                         |
| SSD         | 梵想 2T M.2                                 |                                         |
| 机箱        | 傻瓜超人k88                                 |                                         |
| 电源        | 振华 铜皇450W                               |                                         |
| 散热        | 利民 AK120 MINI                             |                                         |
| 有线        | 板载Realtek® RTL8125B千兆网卡               | 需手动改为1000baseT                     |
| WiFi + 蓝牙 | Intel® AX200                                | macOS Sonoma WIFI需搭配包内HeliPort使用 |
| 声卡        | Realtek® ALC1200                            |                                         |

### 更新说明

2023.06.18

- 更新蓝牙补丁文件 [@zxystd](https://github.com/zxystd/BrcmPatchRAM)

2023.06.16_New

- 定制USB端口

- 修复启动页面出现EFI引导项问题

2023.06.16

- 同步更新至Opencore 0.9.3


- 更新Kext
- 修复Ventura 13.4蓝牙问题 [@zxystd](https://github.com/zxystd/BrcmPatchRAM)
- 关闭啰嗦模式
- 修正config.plist错误、调整Kext
- 支持在线增量升级
- 更新主题

### **正常功能**

- 定制的USB端口
- 支持核显加速
- Intel® AX200 无线+蓝牙（隔空只能收）
- 板载Realtek® ALC1200声卡
- 板载Realtek® RTL8125B千兆网卡（有线网卡使用需要去设置-网络-以太网-高级-硬件-手动设置速度:1000baseT）
- 支持睡眠、唤醒（如有问题，使用Hackintool选择电源选项卡点击下方的螺丝刀图标即可修复）
- 支持传感器
- 定制的OC引导界面（引导界面按空格可以出现重置Nvram的功能，双系统按Ctrl+回车可以设置默认启动项）
- 测试无崩溃，稳定使用（因为自己也在用，并且有些需强迫症，所以官方有更新会抽时间更新的）

<h3>预览图片</h3>

<img src="https://github.com/Hakarikyo/MSI-B460M-MORTAR-WIFI-10700-RX590/blob/main/Picture/Ventura_13.4.png?raw=true" alt="Ventura_13.4" style="zoom: 33%;" />

### BIOS设置

* Settings\高级\内建显示配置——设置第一显卡【PEG】 （强制开启Intel集显）
* Overclocking\CPU特征——CFG 锁定【禁止】
* Overclocking\CPU特征——Intel VT-D技术【禁止】
* Settings\高级——BISO CSM/UEFI Mode【UEFI】
* Settings\高级\USB设置——XHCI Hand-off【允许】
* SATA Mode【AHCI】

### 兼容版本

| 版本                       | 支持                                                         | 下载                                                         | BUG    |
| -------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------ |
| macOS Sonoma Beta          | ✅ （WIFI需搭配压缩包内HeliPort使用 [@zxystd](https://github.com/OpenIntelWireless/HeliPort)） | [地址](https://github.com/Hakarikyo/MSI-B460M-MORTAR-WIFI-10700-RX590/releases) | 待测试 |
| macOS Monterey 12.6.7      | ✅                                                            | [地址](https://github.com/Hakarikyo/MSI-B460M-MORTAR-WIFI-10700-RX590/releases) | 待反馈 |
| macOS Ventura 13.4（13.5） | ✅                                                            | [地址](https://github.com/Hakarikyo/MSI-B460M-MORTAR-WIFI-10700-RX590/releases) | 待反馈 |

### **其他支持**

##### 网卡支持：

- Intel无线网卡

##### CPU支持：

- 理论上支持所有10代CPU

##### 显卡支持：

- 支持仅有核显的Intel® UHD Graphics 630显卡
- 支持AMD RX400 RX500 系显卡，且不需要改动设置
- 其他系列的显卡，需自行探索

> PS: 使用独显的需在BIOS里强制打开CPU核显（高级 -> 内建显示配置 -> 集成显卡多显示器(IGD Multi-monitor) -> 允许），否则核显硬件解码失效，只使用核显的可以忽略

<h3>参考对象</h3>

https://github.com/maemual/MSI-B460M-10700-5500XT

https://github.com/leggod/Hackintosh-B460M-MORTAR
