# Panasonic CF-N10 (CF-N10EWHDS)

## 1. 设备配置

## 2. 驱动安装

> 官方驱动下载地址：https://askpc.panasonic.co.jp/s/download/install/n10ewh.html#model2

### 2.1 疑问解决

- **PCIデータ取得およびシグナル処理コントローラー**

  PCIデータ取得およびシグナル処理コントローラに該当するドライバは`Intel(R) Dynamic Platform & Thermal Framework` ドライバーをインストールすると認識しました。

  需要安装 Windows8 的驱动，该型号没有 WIN8 的驱动，需要稍微新一点的型号 NX2：https://askpc.panasonic.co.jp/win8/up/

  CF-NX2J、NX2K 系列更新模块：https://faq.askpc.panasonic.co.jp/faq/docs/003107

- **不明なデバイス**

  `MEドライバー`

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
