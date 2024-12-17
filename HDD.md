# 硬盘信息



## ST2000DL003-9VT166

> https://www.seagate.com/files/docs/pdf/ja-JP/datasheet/disc/barracuda-green-ds1720.3-1105jp.pdf

| 项目                              | 仕様                   | 备注 |
| --------------------------------- | ---------------------- | ---- |
| モデル番号                        | ST2000DL003            |      |
| インターフェイス・オプション      | NCQ機能搭載SATA 6Gb/秒 |      |
| 回転速度 (RPM)                    | 5900                   |      |
| マルチセグメント・キャッシュ (MB) | 64                     |      |

## 个人设备

- 列表

  | 型号                      | 最大读入速度 | 最大写入速度 | 界面      | 接口         | 颗粒                   | 发布       | 备注                                                         |
  | ------------------------- | -----------: | -----------: | --------- | ------------ | ---------------------- | ---------- | ------------------------------------------------------------ |
  | Samsung SSD 960 EVO 500GB |   3,200 MB/s |   1,900 MB/s | NVMe 2280 | SATA         | 48L SSV3 V-NAND TLC 3D | 2016.09.21 | [官方介绍](https://semiconductor.samsung.com/jp/consumer-storage/internal-ssd/960evo/) |
  | Samsung SSD 970 EVO       |   3,500 MB/s |   2,500 MB/s | M.2 2280  | PCIe3.0 NVMe | 64L SSV4 V-NAND TLC 3D | 2018.04.24 | [官方介绍](https://semiconductor.samsung.com/us/consumer-storage/internal-ssd/970evo/) 5年 |
  | 970 EVO Plus（老版）      |   3,500 MB/s |   3,300 MB/s | M.2 2280  | PCIe3.0 NVMe | 92L SSV5 V-NAND TLC 3D | 2019.01.22 | [官方介绍](https://semiconductor.samsung.com/us/consumer-storage/internal-ssd/970evoplus/) |
  | Samsung SSD 850 Pro 1TB   |     550 MB/s |     520 MB/s | 2.5 HDD   | SATA 6Gb/s   | 3D NAND Flash MLC      |            | [官方介绍](https://semiconductor.samsung.com/jp/consumer-storage/internal-ssd/850pro/) 10年 |
  | Samsung SSD 980 Pro       |   7,000 MB/s |   5,100 MB/s | M.2 2280  | PCIe4.0 NVME | TLC                    |            | [官方介绍](https://semiconductor.samsung.com/consumer-storage/internal-ssd/980pro/) |
  
  

## SSD固态硬盘颗粒

- 列表

  | 类型 | 说明                                   | 单元储存 | 擦写寿命    | 备注                                             |
  | ---- | -------------------------------------- | -------- | ----------- | ------------------------------------------------ |
  | SLC  | 单层单元（Single Level Cell，简称SLC） | 1bit数据 | 9万到10万次 | 最长寿命，容量小、价格贵、读写快，从来没有见到过 |
  | MLC  | 多层单元（Multi Level Cell，简称MLC）  | 2bit数据 | 1万次       |                                                  |
  | TLC  | 三层单元（Triple Level Cell，简称TLC） | 3bit数据 | 500~1000次  | 比较普遍， 寿命短、大容量、读写慢                |
  | QLC  | 四层单元（Quad-level cells，简称QLC）  | 4bit数据 | 1000次      | 容量更大、寿命有所降低，但与TLC相当              |

- QLC：

  QLC每个单元可储存4bit数据，跟TLC相比，QLC的储存密度提高了33%。QLC不仅能经受1000次编程或擦写循环（与TLC相当，甚至更好），而且容量提升了，成本也更低。

  前几年外界预测QLC（四层单元）可擦写寿命仅有100-150次，有很多用户都担心QLC不耐用。但后来美光、东芝等品牌商均表示**3D QLC闪存能经受1000次擦写**，比外界预测的寿命多了十倍。其实，QLC的擦写寿命有所延长要归功于**3D NAND**。
   一般来说，采用更先进的制作工艺能显著提升SSD的存储容量，但是SSD的寿命会变短。如今有一种新型的**3D NAND**技术，一方面能让固态硬盘的寿命不变，另一方面能让固态硬盘获得更大容量。该技术的概念其实非常简单：不同于将存储芯片放置在单面，3D NAND技术可以把存储单元堆叠最高32层。这样一来，单个MLC存储芯片上可以增加最高32GB的存储空间，而单个TLC存储芯片可增加48GB。

## 耗电情况

- 品牌信息

  | SSD品牌与型号            | 闪存类型 | 读取功耗 | SSD读取时的耗电量（1小时） | 写入功耗 | SSD写入时的耗电量（1小时） |
  | ------------------------ | -------- | -------- | -------------------------- | -------- | -------------------------- |
  | 西部数据S240G1G0A  240GB | SLC      | 2.000 W  | 0.002000 kW·h              | 2.5 W    | 0.002500 kW·h              |
  | 三星970 PRO  512GB       | MLC      | 5.200 W  | 0.005200 kW·h              | 5.2 W    | 0.005200 kW·h              |
  | 金士顿A1000  480GB       | TLC      | 0.458 W  | 0.000458 kW·h              | 0.908 W  | 0.000908 kW·h              |
  | 英特尔SSD  660p 542GB    | QLC      | 0.100 W  | 0.000100 kW·h              | 0.1 W    | 0.000100 kW·h              |

  其实，SSD的耗电量会因不同的品牌、型号、闪存类型、读写功耗等因素而不同。就以上参考型号为例，TLC与QLC SSD的读写效能比SLC与MLC的要低，但整体上SSD耗电量还是比较低，基本可以忽略不计。

## SSHD

> | 项目        | ST1000LX015        | 备注                        |
> | ----------- | ------------------ | --------------------------- |
> | 型号        | ST1000LX015-107172 |                             |
> | SN          | WL11SCQS           |                             |
> | 序列号      | WQ93ME2W           |                             |
> | Part Number | 1U7172-500         |                             |
> | FW          | SDM1               | 2024.12为止，没有更新的固件 |
>
> 