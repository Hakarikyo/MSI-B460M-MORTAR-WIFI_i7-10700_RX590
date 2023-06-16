# MSI-B460M-WIFI_i7-10700_RX590
黑苹果 intel i7 10700+MSI MAG B460M MORTAR WIFI+RX590

## 硬件配置

| 配置        | 型号                         | 说明                              |
| ----------- | ---------------------------- | --------------------------------- |
| CPU         | Intel i7 10700               |                                   |
| 主板        | 微星 MAG B460M MORTAR WiFi   |                                   |
| 显卡        | 迪兰DEVIL RX 590 8G          |                                   |
| 内存        | 3200MHz 16G * 2              |                                   |
| SSD         | 梵想 2T M.2                  |                                   |
| 机箱        | 傻瓜超人k88                  |                                   |
| 电源        | 振华 铜皇450W                |                                   |
| 散热        | 利民 AK120 MINI              |                                   |
| 有线        | 板载Realtek RTL8125B千兆网卡 | 需手动改为1000baseT               |
| WiFi + 蓝牙 | Intel® AX200                 | Sonoma WIFI需搭配包内HeliPort使用 |
| 声卡        | Realtek® ALC1200             |                                   |

<h3>预览</h3>

<img src="https://github.com/Hakarikyo/MSI-B460M-MORTAR-WIFI-10700-RX590/blob/main/Picture/Ventura_13.4.png?raw=true" alt="Ventura_13.4" style="zoom: 33%;" />

### BIOS

* Settings\高级\内建显示配置——设置第一显卡【PEG】 （强制开启Intel集显）
* Overclocking\CPU特征——CFG 锁定【禁止】
* Overclocking\CPU特征——Intel VT-D技术【禁止】
* Settings\高级——BISO CSM/UEFI Mode【UEFI】
* Settings\高级\USB设置——XHCI Hand-off【允许】
* SATA Mode【AHCI】

### 兼容

| 版本                       | 支持                                                         | 下载                                                         | BUG    |
| -------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------ |
| macOS Sonoma Beta          | ✅ （WIFI需搭配包内HeliPort使用 [@zxystd](https://github.com/OpenIntelWireless/HeliPort)） | [地址](https://github.com/Hakarikyo/MSI-B460M-MORTAR-WIFI-10700-RX590/releases/tag/%E6%B5%8B%E8%AF%95) | 待反馈 |
| macOS Monterey 12.6.7      | ✅                                                            | [地址](https://github.com/Hakarikyo/MSI-B460M-MORTAR-WIFI-10700-RX590/releases/tag/%E5%8F%91%E5%B8%83%E6%9B%B4%E6%96%B0) | 待反馈 |
| macOS Ventura 13.4（13.5） | ✅                                                            | [地址](https://github.com/Hakarikyo/MSI-B460M-MORTAR-WIFI-10700-RX590/releases/tag/%E5%8F%91%E5%B8%83%E6%9B%B4%E6%96%B0) | 待反馈 |

<h3>参考对象：</h3>

https://github.com/maemual/MSI-B460M-10700-5500XT
