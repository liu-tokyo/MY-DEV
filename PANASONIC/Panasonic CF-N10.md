# Panasonic CF-N10 (CF-N10EWHDS)

## 1. 设备配置

| 项目               | 配置                | 备注         |
| ------------------ | ------------------- | ------------ |
| ＣＰＵ             | Intel Core i5 2540M | 2.5GHz/2コア |
| 内存               | 4GB                 | 最大16GB     |
| 重量               | 1.27kg              |              |
| BIOS               | V3.00L16            |              |
| INTEL® ME Firmware | 7.1.14.1107         |              |

安装 Windows10 之后，速度很慢的原因：https://kekaku.addisteria.com/wp/20190504005219

## 2. 驱动安装

> 官方驱动下载地址：https://askpc.panasonic.co.jp/s/download/install/n10ewh.html#model2  
> https://askpc.panasonic.co.jp/s/download/install/n10ath.html
>
> https://ikt-s.com/cf-lx4-drivers/
>
> https://ikt-s.com/cf-lx4-drivers/
>
> https://ikt-s.com/cf-lx4-drivers/

- Windows10 安装之后无法自动识别的硬件

  | 硬件名称                    | 硬件ID                                       | 驱动名称                                                     | 驱动下载                                                     |
  | --------------------------- | -------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
  | PCI串行端口                 | PCI\VEN_8086&DEV_1C3D&SUBSYS_833810F7&REV_04 | Intel® Active Management Technology- SOL                     | ✅官方下载 `ME ドライバー`                                    |
  | PCI简单通讯控制器           | PCI\VEN_8086&DEV_1C3A&SUBSYS_833810F7&REV_04 | Intel® Management Engine Interface                           | ✅〃 (※3)                                                     |
  | PCI设备                     | PCI\VEN_10EC&DEV_5209&SUBSYS_833810F7&REV_01 | Realtek PCIE CardReader Drivers                              | ❌[INTEL官网](https://www.intel.com/content/www/us/en/download/19417/realtek-card-reader-driver-for-windows-10-64-bit-for-intel-nuc6cayh-nuc6cays.html) 下载最新驱动 |
  | PCI数据捕获和信号处理控制器 | PCI\VEN_8086&DEV_0103&SUBSYS_833810F7&REV_09 | Intel Dynamic Platform and Thermal Framework                 | ❌可选驱动<br />`Intel - DPTF - 8.1.10605.221` 第一个 (※2)    |
  | 未知设备                    | ACPI\VEN_MAT&DEV_0019                        | Microsoft ACPI-Compliant System<br />System Interface Device Driver | ❌Intel Smart Connect Technology (※1)                         |

  ※1 `Windows 10` 不支持英特尔智能连接`(Intel Smart Connect Technology`)技术。准确地说，英特尔智能连接技术是一项已停产的技术。  
  　解决方案是在 BIOS (UEFI) 中禁用英特尔智能连接技术。  
  ※2 不能使用 INTEL 的最新驱动，会直接导致画面蓝屏。  
  ※3 ME 的版本一旦升级为最新版本，则系统几乎无法运转。一旦安装了 INTEL 最新的 11 的版本，一样会出现问题；  
  　所以，不能安装 INTEL 的驱动安装助手之类的软件，导致无故被升级到最新版本的驱动。

### 2.1 疑问解决

- **PCIデータ取得およびシグナル処理コントローラー**

  PCIデータ取得およびシグナル処理コントローラに該当するドライバは`Intel(R) Dynamic Platform & Thermal Framework` ドライバーをインストールすると認識しました。

  需要安装 Windows8 的驱动，该型号没有 WIN8 的驱动，需要稍微新一点的型号 NX2：https://askpc.panasonic.co.jp/win8/up/

  CF-NX2J、NX2K 系列更新模块：https://faq.askpc.panasonic.co.jp/faq/docs/003107 (旧版本 6.x，新版本安装的话，导致无法启动)

- **不明なデバイス**

  オプションの更新プログラム `Panasonic - System Devices for Panasonic OC`

## 3. 设备升级

### 3.1 内存升级

- 适用内存

  | チップ規格     | 動作周波数 | モジュール | データ転送速度 | ピン数  |
  | -------------- | ---------- | ---------- | -------------- | ------- |
  | DDR4-2666      | 2666MHz    | PC4-21300  | 21.3GB/s       | 260ピン |
  | DDR4-2400      | 2400MHz    | PC4-19200  | 19.2GB/s       | 260ピン |
  | DDR4-2133      | 2133MHz    | PC4-17020  | 17.02GB/s      | 260ピン |
  | **DDR3L-1600** | 1600MHz    | PC3L-12800 | 12.8GB/s       | 204ピン |
  | DDR3-1600      | 1600MHz    | PC3-12800  | 12.8GB/s       | 204ピン |
  | DDR3-1333      | 1333MHz    | PC3-10600  | 10.6GB/s       | 204ピン |
  | DDR3-1066      | 1066MHz    | PC3-8500   | 8.5GB/s        | 204ピン |
  | DDR2-800       | 800MHz     | PC2-6400   | 6.4GB/s        | 200ピン |
  | DDR2-667       | 667MHz     | PC2-5300   | 5.3GB/s        | 200ピン |
  | DDR2-533       | 533MHz     | PC2-4200   | 4.2GB/s        | 200ピン |
  | DDR-333        | 333MHz     | PC2700     | 2.7GB/s        | 200ピン |

  机载内存：4GB  
  最大内存：16GB（8GB x 2）

- 拆解设备  
  ![img](https://sysbloblog.com/wp-content/uploads/2021/09/img_2776-scaled-e1631353003498-2-1024x768.jpg)
  该设备的内存交换比较简单，只需要拆解一个螺丝，即可增设内存。

### 3.2 硬盘升级

- 设备拆解  
  ![img](https://office-mos.com/wp-content/uploads/2020/05/IMG_4760-2.jpg)  
  首先要去掉电池，只需要拆解2个螺丝。  
  ![img](https://office-mos.com/wp-content/uploads/2020/05/IMG_4764.jpg)  
  打开该连接，就可以抽出HDD。

## 4. 其它事项
