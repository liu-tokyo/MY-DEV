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

  https://dynabook.com/assistpc/download/modify/dynabook/t552/xxg/bios/index_j.htm

  BIOS更新的时候，出现如下错误：

  ```
  can not determine the mainboard
  ```

  下载的主板驱动有问题，正确的链接如下：

  https://dynabook.com/assistpc/download/modify/sate/b652/xxf/bios/index_j.htm

- dynabook Satellite B652/G、B552/G、B452/G シリーズ Windows 7 Professional SP1 64bit アップグレードモジュール

  https://dynabook.com/assistpc/download/win7/navigate/satellite/b652g/sp1/64bit/sab652gread7sp164.htm?qry=.%2F%3Ffunc%3Dpi%26category%3D131020%26keyword%3DSatellite%2BB452

Windows10的话，几乎所有硬件都可以自动识别出来，Windows7 的话，首先无线网卡就无法识别，首先是有网络之后，才能干其它的事情。

