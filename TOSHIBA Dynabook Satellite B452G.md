## 东芝笔记本电脑 - Dynabook Satellite B452/G

> https://dynabook.com/direct/pc-static/before2016/pc1/catalog/2012/b552g/spec.html  
> B452/F  
> https://dynabook.com/direct/pc-static/before2016/pc1/catalog/2012/b452f/spec.html  
> dynabook Satellite B452/G  PB452GNAP25A71  
> https://dynabook.com/pc/catalog/satellit/121119b452/spec.htm

### 1. 电脑规格

| 项目                              | 配置                                                         | 备考                |
| --------------------------------- | ------------------------------------------------------------ | ------------------- |
| 生产日期                          | 2012年                                                       |                     |
| CPU                               | Celeron® プロセッサーB830                                    | BenchMarks：**814** |
| 内存                              | Crucial 4GB DDR3L-1600 SODIMM                                |                     |
|                                   | 標準/最大：2GB（2GB×1）／8GB                                 | 升级4GB             |
|                                   | 仕様：**PC3-10600**（DDR3-1333）対応 SDRAM、デュアルチャネル対応 |                     |
|                                   | メモリ専用スロット：2スロット（空きスロット×1）              |                     |
| チップセット                      | モバイル インテル® HM70 Express チップセット                 |                     |
| 表示機能                          | 最大1,366×768ドット(※9)/1,677万色                            |                     |
| ビデオRAM                         | 32ビット版： 最大775MB（メインメモリと共用）<br />64ビット版： 最大778MB（メインメモリと共用） |                     |
| グラフィック<br/>アクセラレーター | インテル® HD グラフィックス（CPUに内蔵）                     |                     |
| HDD                               | 320GB HDD(5,400rpm、Serial ATA対応)                          |                     |
| 光学ドライブ                      | DVD-ROMドライブ                                              |                     |
| 質量                              | 標準バッテリーパック装着時：約2.4kg<br />バッテリパック62W（オプション）装着時：約2.6kg |                     |

### 2. CPU跑分

| CPU型号                           | BenchMarks跑分 |                                       |
| --------------------------------- | -------------- | ------------------------------------- |
| Celeron Dual-Core T3100 @ 1.90GHz | 557            | CPU First Seen on Charts: Q4 2009     |
| Intel Core2 Duo P8700 @ 2.53GHz   | 968            | CPU First Seen on Charts: Q1 2009     |
| Intel Core i3-3110M @ 2.40GHz     | 1627           | CPU First Seen on Charts: Q3 2012     |
| Intel Celeron B830 @ 1.80GHz      | **814**        | **CPU First Seen on Charts:** Q1 2012 |

### 3. 设备评价

用作办公还能勉强用，对专业人士来说，没有任何价值。2012年的CPU，虽然性能不行，但是开机速度还算很快，20秒就能开机结束。  

都说 Linux 不是那么吃内存，其中另外一台同配置电脑安装了 Ubuntu 22.04 ，开机速度巨慢，还是受到硬盘的影响更大。

**建议：**

- 内存升级：2GB → 8GB
- 硬盘类型：机械硬盘 → SSD（只能一块硬盘，SATA接口的2.5英寸硬盘）

### 4. 设备扩展

1. 只有一个 SATA 的硬盘位，主板上没有 M.2 接口。

   实在想要安装 M.2 接口的固态硬盘，只能用转换设备，转为 SATA 接口方式。

### 5. 驱动下载

- TOSHIBA官方下载：

  Windows 8.1

  https://dynabook.com/assistpc/osup/windows81/manu/list/b452g.htm

  Windows 7 with SP1

  https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm

- BIOS更新链接

  ❌ https://dynabook.com/assistpc/download/modify/dynabook/t552/xxg/bios/index_j.htm

  ✔ https://dynabook.com/assistpc/download/modify/sate/b652/xxf/bios/index_j.htm

  BIOS更新的时候，出现如下错误：

  ```
  can not determine the mainboard
  ```
  
  ※ 原因：下载了错误的电脑的BIOS更新程序。

  下载的主板驱动有问题，正确的链接如下：

  https://dynabook.com/assistpc/download/modify/sate/b652/xxf/bios/index_j.htm

- dynabook Satellite B652/G、B552/G、B452/G シリーズ Windows 7 Professional SP1 64bit アップグレードモジュール

  https://dynabook.com/assistpc/download/win7/navigate/satellite/b652g/sp1/64bit/sab652gread7sp164.htm?qry=.%2F%3Ffunc%3Dpi%26category%3D131020%26keyword%3DSatellite%2BB452

Windows10的话，几乎所有硬件都可以自动识别出来，Windows7 的话，首先无线网卡就无法识别，首先是有网络之后，才能干其它的事情。

未能识别的硬件列表：

| 设备名称                   | 硬件ID                                                   |                                                              |
| -------------------------- | -------------------------------------------------------- | ------------------------------------------------------------ |
| PCI简单通讯控制器          | PCI\VEN_8086&DEV_1E3A&SUBSYS_00011179&REV_04             | [Intel Chipset Device Software](https://pcsupport.lenovo.com/id/en/downloads/ds118691) |
| 基本系统设备               | PCI\VEN_1180&DEV_E823&SUBSYS_00011179&REV_04             | Ricoh PCIe SDXC/MMC Host Controller Drivers<br />可选驱动    |
| 基本系统设备               | PCI\VEN_1180&DEV_E232&SUBSYS_00011179&REV_04             | Ricoh Media Card Reader Driver<br />可选驱动                 |
| 基本系统设备               | PCI\VEN_1180&DEV_E852&SUBSYS_00011179&REV_07             | PCI\VEN_1180&DEV_E852&SUBSYS_00011179&REV_07<br />可选驱动   |
| High Definition Audio 设备 | HDAUDIO\FUNC_01&VEN_8086&DEV_2806&SUBSYS_11790001&REV_10 | [Intel(R) Display Audio](https://www.driverscape.com/manufacturers/toshiba/laptops-desktops/dynabook-satellite-b452-g/6146)<br />英特尔(R) 显示器音频 |



### 6. 更新列表

| 名称                                                         | バージョン             | サイズ | 处理标志 | 注意事項                                                     |
| :----------------------------------------------------------- | :--------------------- | :----- | -------- | :----------------------------------------------------------- |
| [Intel Chipset SW Installation Utility](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#chipset) | 9.3.0.1020             | 5.78MB |          |                                                              |
| [Intel Management Engine Interface](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#imei) | 8.00.03.1427           | 55.7MB |          |                                                              |
| [Intel AMT Software](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#amt) | 8.00.03.1427           | 60.3MB |          |                                                              |
| [Intel Display Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#display_i) | 8.15.10.2712           | 154MB  |          | CPUが以下のモデルが対象です。 <br />・インテル(R)Core(TM) i7-3520M vPro(TM)プロセッサー <br />・インテル(R)Core(TM) i7-3520Mプロセッサー<br />・インテル(R)Core(TM) i5-3320M vPro(TM)プロセッサー <br />・インテル(R)Core(TM) i5-3320Mプロセッサー <br />・インテル(R)Core(TM) i5-3210Mプロセッサー |
| [Intel Display Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#display_s) | 8.15.10.2712           | 114MB  |          | CPUが以下のモデルが対象です。 <br />・インテル(R)Core(TM) i3-2370Mプロセッサー <br />・インテル(R)Celeron(R)プロセッサー B820 |
| [Intel Rapid Storage Technology Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#ir_storage) | 11.0.0.1032            | 13.8MB |          |                                                              |
| [TOSHIBA Value Added Package](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tvalue) | 1.6.0027.640202        | 108MB  | ✔✔       |                                                              |
| [Realtek Audio Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#sound) | 6.0.1.6591             | 124MB  | ❌        |                                                              |
| [Intel USB3.0 Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#usb3) | 1.0.4.220              | 7.33MB |          |                                                              |
| [Intel Rapid Start Technology Software](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#ir_start) | 1.0.0.1022             | 4.05MB |          |                                                              |
| [Intel Wireless LAN Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#iwlan) | 15.1.0.21.1.s64_wCAT   | 16.0MB |          | Intel WirelessLAN モデルのみ                                 |
| [Atheros Wireless LAN Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#atwlan) | 9.2.0.500.0.s3264_wCAT | 27.0MB |          | Atheros無線LANモデルのみ                                     |
| [ALPS Pointing Device Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tpad) | v7.x5.303.215          | 38.6MB |          |                                                              |
| [TOSHIBA Software Modem](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#modem) | 2.2.97                 | 4.36MB | ✔？      |                                                              |
| [TOSHIBA HDD Protection](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#thdd_pro) | 2.2.2.15               | 23.2MB | ✔        |                                                              |
| [Bluetooth Monitor](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#btmoni) | v4.08                  | 5.26MB |          |                                                              |
| [Intel LAN Driver](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#lan) | 16.8.46                | 27.1MB |          |                                                              |
| [Ricoh Card Reader](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#card) | 2.15.17.02             | 6.73MB |          |                                                              |
| [TOSHIBA Sleep Utility](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tsleep) | 1.4.0024.000101        | 6.85MB | ✔        |                                                              |
| [TOSHIBA eco Utility](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#teco) | 1.3.21.64              | 15.9MB | ✔        |                                                              |
| [TOSHIBA Peakshift Control](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tpeak) | 3.01.00.64             | 14.4MB | ✔✔       |                                                              |
| [Intel Proset](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#iwu) | 15.1.0.0.2.s64_wCAT    | 71.8MB |          | Intel WirelessLAN モデルのみ                                 |
| [TOSHIBA HDD/SSD Alert](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#talert) | 3.1.64.14              | 32.9MB |          |                                                              |
| [TOSHIBA Service Station](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tservice) | 2.2.13                 | 12.8MB | ✔✔       |                                                              |
| [TOSHIBA PC Health Monitor](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#thealth) | 1.7.16.64              | 27.3MB |          |                                                              |
| [ConfigFree](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#config) | 8.0.43n                | 55.4MB | ✔✔       |                                                              |
| [TOSHIBA Wireless LAN Indicator](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#twlan) | 1.0.5n                 | 6.07MB | ✔        |                                                              |
| [TOSHIBA Recovery Media Creator](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#trecovery) | v2.1.7.52020010        | 10.3MB | ✔        |                                                              |
| [TOSHIBA Disc Creator](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tdc) | 2.1.0.11 for x64       | 9.61MB | ✔        |                                                              |
| [TOSHIBA Sync Utility](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tsync) | v2.0.3090              | 39.3MB | ✔        |                                                              |
| [Infineon TPM Software Professional Package](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tpm) | 3.60.2071.00           | 59.3MB | ✔        |                                                              |
| [TOSHIBA 180 Degrees Rotation Utility](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#t180) | v1.4.0.0M              | 6.91MB | ✔✔       | 180度数旋转实用程序                                          |
| [TOSHIBA Bulletin Board](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tboard) | 2.1.19                 | 56.4MB | ✔✔       | 东芝公告板                                                   |
| [TOSHIBA ReelTime](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#treel) | 1.7.22                 | 26.6MB | ✔        |                                                              |
| [TOSHIBA Device Access Control](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tdevice) | 3.0.14                 | 17.8MB | ✔✔       |                                                              |
| [TOSHIBA Security Assist](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tsecurity) | 2.0.10                 | 6.72MB | ✔✔       |                                                              |
| [オンラインマニュアル](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#manual) | 0001.1202              | 14.5MB |          |                                                              |
| [TPM Manual](https://dynabook.com/assistpc/download/win7/navigate/satellite/b652f/sp1/64bit/sab652fread7sp164.htm#tpm_m) | 300.022.0001           | 6.61MB |          |                                                              |

### 7. 硬件升级

- 内存升级

  只需要拆开一个螺丝

- 硬盘升级

  只需要拆开一个螺丝

- 只有更复杂的硬件升级，才需要拆开背面所有螺丝。

  https://dynabook.biz/fan/13580/

  ![img](https://dynabook.biz/wp/wp-content/uploads/2017/12/b450_1.jpg)

  

### 8. 进入BIOS

- 在 `In Touch with Tomorrow TOSHIBA` 表示之后，按下 F2 键，就会进入 BIOS 设置画面。
- 按下 `Delele` 键，也能进入 BIOS 设置画面面，虽然提示画面没有该信息（过去老旧电脑都是按 DEL 键进入 BIOS）。

| #     | BIOS VER | EC VER | 备注           |
| ----- | -------- | ------ | -------------- |
| 设备1 | 6.30     | 1.00   | 损坏诚度比较大 |
| 设备2 |          |        |                |

