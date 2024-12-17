# 个人设备的配置、规格、维护等信息

> 在进行 Office2016 更新的过程中，感觉 WIN11 要比 WIN10 流畅；WIN10 的话，更新画面几乎无法滚动，而 WIN111 的滚动非常流畅。  
> - 感觉是 WIN11 的内存释放更合理，更新过程中，内存使用率一直没有上涨；也不会有安装必须 `正在等待重启` 的要求（另外一台电脑有1件）。  
>   但是，也可能是远程桌面的原因；如果电脑是机械硬盘，在大量更新数据的情况下，会影响到连接的速度，显示出来的情况就是比较卡顿。  
>   总之，WIN11 的内存管理可能要比 WIN10 更加优秀。
> - 而 WIN10 在更新 Office 的时候，内存一直上升，直到最终结束，感觉一直没有被释放；因为内存不足导致的内存交换，操作非常卡顿。  
>   发现 `Thinkpad 13` 在更新的时候，也没有内存无限上涨的情况。

## 1. 本人保有设备信息

| 设备                              | 型号           | IP地址        | CPU型号               | 备注                     |
| --------------------------------- | -------------- | ------------- | --------------------- | ------------------------ |
| DELL INSPIRON 1545                |                |               | Intel Core2 Duo P8400 | 张冬的电脑、性能严重不足 |
| FUJITSU LIFEBOOK A573/GX          | FMVA0301WP     | 192.168.5.88  | Intel Core i5-3340M   |                          |
| FUJITSU LIFEBOOK A574/KX          | FMVA0802YP     | 192.168.5.150 | Intel Celeron 2950M   |                          |
| KURO-DACHI_CLONE_U3               |                |               |                       |                          |
| Lenovo G580                       | 2189           | 192.168.5.206 |                       |                          |
| NEC LaVie L LL750/B               | PC-LL750BS1YD  | 192.168.5.201 | Intel Core i5 450M    |                          |
| Panasonic CF-LX5                  | CF-LX5PDT5S    | 192.168.5.220 | Intel Core i5-6300U   | 4GB内存+256GB-SSD        |
| Panasonic CF-N10                  | CF-N10EWHDS    | 192.168.5.165 | Intel Core i5-2540M   |                          |
| Panasonic CF-SZ5                  | CF-SZ5PDA5S    | 192.168.5.60  | Intel Core i5-6300U   | 4GB内存+256GB-SSD        |
| 〃                                | CF-SZ5PDY6S    | 192.168.5.53  | Intel Core i5-6300U   | 8GB内存+256GB-SSD        |
| Lenovo Thinkpad 13                | 20J2A0C1JP     | 192.168.5.158 | Intel Celeron 3865U   | 8GB内存+128GB-SSD        |
| Lenovo S510 small                 |                |               |                       |                          |
| ThinkCentre M92 Tower             |                |               |                       |                          |
| ThinkPad E450                     |                |               |                       |                          |
| Thinkpad E480                     |                |               | Intel Core i5-8250U   | 本人工作用电脑           |
| ThinkPad E480内存扩展             |                |               |                       |                          |
| ThinkPad T480内存扩展             |                |               | Intel Core i5-8250U   |                          |
| Thinkpad X250                     |                | 192.168.5.87  | Intel Core i5-5300U   |                          |
| Thinkpad X280                     |                |               | Intel Core i5-8250U   |                          |
| Thinkpad X61s                     |                | 192.168.5.248 | Intel Core2 Duo L7300 | 4GB内存+256GB-HDD        |
| TOSHIBA Dynabook Satellite B452/G | PB452GNBPR7A71 | 192.168.5.75  | Intel Celeron B830    | Gitlab服务器             |
| 〃                                | 〃             | 192.168.5.45  | 〃                    | Windows 10               |
| TOSHIBA Dynabook Satellite B551/C |                | 192.168.0.4   |                       | 没有无线网卡             |
| HDD                               |                |               |                       |                          |
| 打印机                            |                |               |                       |                          |



## 2. 进入BIOS设置的办法

根据制造商，有所不同

- 「F2」键的制造商
  NEC、富士通、東芝、SONY、Lenovo(IBM)、Dell、日立、Panasonic、Mouse Computer、Sharp、ASUS、Intel、ASROCK 、Gateway、acer

- 「Del」键的制造商
  Epson、ASUS、Gigabyte、ESC、MSI、ASROCK(也有`F2`的情况)

- 「F10」键的制造商
  HP(Compaq)

- 「Ctrl+Alt+Enter」键的制造商
  Dell

- 【ENTER】键的制造商

  Lenovo的新系列（Thinkpad主要系列之外）

## 3. 电脑CPU跑分

### 3.1 笔记本电脑

| 型号                            |  C/T  | 跑分[单] | 跑分[多] | 发布日期 | TDP Down | Typical TDP | TDP Up: | 备注（自有设备）          |
| ------------------------------- | :---: | -------: | -------: | -------- | -------: | ----------: | ------: | ------------------------- |
| Intel Core i5-1235U             | 10/12 |     3218 |    13388 | Q1 2022  |        - |        15 W |    55 W |                           |
| Intel Core i5-8365U @ 1.60GHz   |  4/8  |     2121 |     6102 | Q2 2019  |     10 W |        15 W |    25 W |                           |
| Intel Core i5-8350U @ 1.70GHz   |  4/8  |     2021 |     6211 | Q4 2017  |     10 W |        15 W |    25 W |                           |
| Intel Core i5-8250U @ 1.60GHz   |  4/8  |     1904 |     5865 | Q3 2017  |     10 W |        15 W |    25 W |                           |
| Intel Core i7-7660U @ 2.50GHz   |  2/4  |     2153 |     4078 | Q2 2017  |    9.5 W |        15 W |       - |                           |
| Intel Core i5-7300U @ 2.60GHz   |  2/4  |     1904 |     3653 | Q1 2017  |    7.5 W |        15 W |    25 W |                           |
| Intel Core i7-6820HQ @ 2.70GHz  |  4/8  |     1953 |     6817 | Q4 2015  |        - |        45 W |       - |                           |
| Intel Core i5-6300U @ 2.40GHz   |  2/4  |     1657 |     3232 | Q3 2015  |        - |        15 W |       - | Panasonic  CF-SZ5         |
| Intel Core i5-5300U @ 2.30GHz   |  2/4  |     1632 |     2730 | Q1 2015  |        - |        15 W |       - | Thinkpad X250             |
| Intel Core i5-4300U @ 1.90GHz   |  2/4  |     1482 |     2495 | Q3 2013  |        - |        15 W |       - |                           |
| Intel Core i5-4200U @ 1.60GHz   |  2/4  |     1287 |     2180 | Q1 2013  |        - |        15 W |       - |                           |
| Intel Core i5-3340M @ 2.70GHz   |  2/4  |     1652 |     2695 | Q1 2013  |        - |        35 W |       - | LIFEBOOK A573/GX          |
| Intel Core i5-3210M @ 2.50GHz   |  2/4  |     1525 |     2464 | Q1 2012  |        - |        35 W |       - | Lenovo G580               |
| Intel Celeron 3865U @ 1.80GHz   |  2/2  |     1034 |     1321 | Q2 2017  |     10 W |        15 W |       - | Lenovo ThinkPad 13        |
| Intel Core i7-2620M @ 2.70GHz   |  2/4  |     1459 |     2423 | Q1 2011  |        - |        35 W |       - | Thinkpad X220             |
| Intel Core i5-2540M @ 2.60GHz   |  2/4  |     1409 |     2365 | Q4 2010  |        - |        35 W |       - | Panasonic CF-N10          |
| Intel Celeron 2950M @ 2.00GHz   |  2/2  |     1143 |     1234 | Q2 2014  |        - |        37 W |       - | LIFEBOOK A574/KX          |
| Intel Core i3-2310M @ 2.10GHz   |  2/4  |      942 |     1220 | Q1 2011  |        - |        35 W |       - | Dynabook Satellite B551/C |
| Intel Core i5-450M @ 2.40GHz    |  2/4  |     1045 |     1239 | Q2 2010  |        - |        35 W |       - | NEC LaVie L LL750/B       |
| Intel Celeron B830 @ 1.80GHz    |  2/2  |      821 |      857 | Q1 2012  |        - |        35 W |       - | Dynabook Satellite B452/G |
| Intel Core2 Duo L7300 @ 1.40GHz |  2/2  |      551 |      536 | Q2 2009  |        - |        15 W |       - | Thinkpad X61s             |

### 3.2 Surface

| 型号                         | Cores/Threads | 跑分（单线程） | 跑分（多线程） | 发布日期 | TDP Down | Typical TDP | TDP Up: | 备注 |
| ---------------------------- | :-----------: | -------------: | -------------: | -------- | -------: | ----------: | ------: | ---- |
| Snapdragon X Elite - X1E-80-100 | 12/12 | 3283 | 23144 | Q2 2024 | - | - | - |  |
| Snapdragon 8350 | 8/8 | 2484 | 4608 | Q1 2021 | - | - | - |  |
| Intel Core m3-8100Y @ 1.10GHz | 2/4 | 1702 | 2864 | Q4 2018 | 4.5 W | 5 W | 8 W |  |
| Intel Pentium 4415Y @ 1.60GHz | 2/4 | 864 | 1583 | Q3 2018 | 4.5 W | 6 W | - |  |
| Intel Atom x7-Z8700 @ 1.60GHz | 4/4  |      650 |     1324 | Q2 2015  |        - |         4 W |       - |                     |

### 3.3 台式机

| 型号                         | Cores/Threads | 跑分（单线程） | 跑分（多线程） | 发布日期 | TDP Down | Typical TDP | TDP Up: | 备注 |
| ---------------------------- | :-----------: | -------------: | -------------: | -------- | -------: | ----------: | ------: | ---- |
| Intel Core i3-4130 @ 3.40GHz |      2/4      |           1884 |           3315 | Q1 2013  |        - |        54 W |       - |      |



## 4. Windows进入安全模式

安全模式是Windows的一種故障排除选项，可在有限狀態下启动电脑。仅启动运行 Windows 所需的基本软件和驱动。安全模式对于解決可能无法正確启动或可能阻止 Windows 正常启动的软件和驱动程序问题非常有用。如何到达該位置取決于PC是否可以正常启动 Windows 。

相较于老版本的 XP，从 WIN7 开始，进入安全模式的方法已经改变，请参阅如下网址：  
https://pcsupport.lenovo.com/in/ja/products/laptops-and-netbooks/lenovo-g-series-laptops/lenovo-g580-notebook/solutions/HT116905
