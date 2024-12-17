# NEC LaVie L LL750/B (PC-LL750BS1YD)

> PC-LL750BS1YD  
> 08009331A

## 1. 设备规格

- 主要配置规格

  | 项目         | 规格                                                         | 备注                                               |
  | ------------ | ------------------------------------------------------------ | -------------------------------------------------- |
  | 芯片组       | Mobile Intel® HM55 Express Chipset                           |                                                    |
  | 屏幕         | 16英寸                                                       | WXGA(最大1366×768)                                 |
  | CPU          | Core i5 450M/2.4GHz/2核心/4线程                              |                                                    |
  | 内存         | 8GB （最大8GB，感觉不止，官方所说8GB，是最高配置的内存量？） | 标配4GB DDR3 ※升级到8GB (PC3-8500)                 |
  | 显卡         | 内置 Intel HD Graphics                                       | 内存：最大1696MB                                   |
  | 系统         | Windows 7 Home Premium 32/64bit                              |                                                    |
  | 重量         | 3.1kg                                                        |                                                    |
  | CD-ROM       | ブルーレイディスクドライブ(DVDスーパーマルチドライブ機能付き) |                                                    |
  | Office       | Microsoft® Office Home and Business 2010                     |                                                    |
  | FeliCaポート | 搭載(Version 2.0)                                            |                                                    |
  | USB          | USB 3.0×2、2.0×3                                             |                                                    |
  | LAN          | 1000BASE-T/100BASE-TX/10BASE-T対応                           |                                                    |
  | 无线         | IEEE802.11b/g/n                                              |                                                    |
  | 硬盘         | 約500GB(Serial ATA、5400回転/分)                             | WDC WD5000BEVT-26A0RT0<br />※ 该硬盘的性能相对较好 |
  
  注：其它项目参照[官方信息](https://lenovo-nec.jp/navigate/products/pc/102q/06/lavie/lvl/spec/index.html)。

## 2. 设备性能

- 主要设备性能

  | 设备         | 性能        | 备注                                                         |
  | ------------ | ----------- | ------------------------------------------------------------ |
  | Core i5 450M | `1045/1233` | [Passmark](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Core+i5-450M+%40+2.40GHz&id=3) |
  | -            |             |                                                              |
  | -            |             |                                                              |

## 3. 驱动更新

- BIOS更新  
  http://search.casnavi.nec.co.jp/download/pc/module/bios/pc98-nx/330a1700/index.htm  
  `1960-1600/576A1600`
  
- 驱动官方网址  
  https://support.nec-lavie.jp/driverlist?productId=PC-LL750BS1YB

- driverscape 辅助驱动网页  
  https://www.driverscape.com/manufacturers/nec/laptops-desktops/pc-ll750wg6w/58333  
  https://www.driverscape.com/manufacturers/nec/laptops-desktops/pc-lm750es6w/193984  
  
- Intel ME

  WIN10 的情况，`Intel ME` 的驱动，可以通过 `Windows 更新` → `查看可选更新`，选择 `Intel Management Engineering Interface` 进行安装。

- O2Micro

- FeliCa Port

- `USB\DEVICE_DESCRIPTOR_FAILURE`

- Windows10安装后，无法自动识别的硬件：

  | 硬件名称          | 硬件ID                                       | 驱动                                                         |
  | ----------------- | -------------------------------------------- | ------------------------------------------------------------ |
  | PCI简单通讯控制器 | PCI\VEN_8086&DEV_3B64&SUBSYS_89341033&REV_06 | Intel(R) Management Engine Interface                         |
  | 大容量存储控制器  | PCI\VEN_1217&DEV_8130&SUBSYS_89341033&REV_01 | O2Micro Integrated MS/MSPRO/xD Controller                    |
  | 未知设备          | USB\VID_054C&PID_02E1\6&1041377&0&2          | [SONY Felica（NEC）](https://www.sony.co.jp/Products/felica/consumer/support/download/nfcportsoftware.html?j-short=fsc_dl) `FeliCa Port/PaSoRi` |

  ※ WIN11 安装之后，也是一样的问题。

## 4. 硬件升级

- 购入的二手，已经内存升级到了 `8GB` 。

## 5. 系统安装

### 5.1 Windows11

- 速度虽然不快，但是可以正常安装，使用起来没啥问题。    
最好还是用 WIN10，用 WIN11 的话，确实压力很大。