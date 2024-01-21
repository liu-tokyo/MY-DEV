# Panasonic CF-LX5

> 型号：CF-LX5PDP6S

## 1. 设备配置

> 参照：Panasonic CF-LX5PDP6S.pdf

- 设备配置表：

  | 项目 | 配置                                                         | 备注                 |
  | ---- | ------------------------------------------------------------ | -------------------- |
  | CPU  | Core i5 6300U(Skylake)/2.4GHz/2コア                          | 3239                 |
  | 内存 | 8GB LPDDR3 SDRAM（拡張スロットなし）                         |                      |
  | 硬盘 | SSD*:256GB（Serial ATA）                                     |                      |
  | 屏幕 | 14.0型（16:9）Full HD 広視野角液晶（1920×1080ドット）アンチグレア | 解像度:Full HD 1080p |
  | 无线 | インテル® Dual Band Wireless-AC 8260                         |                      |
  | 蓝牙 | Bluetooth v4.0（Windows 10 Pro使用時はBluetooth v4.1）       |                      |
  | 安全 | TPM（TCG V1.2準拠）                                          |                      |
  | 尺寸 | 幅333mm×奥行225.6mm×高さ24.5mm（突起部除く）                 |                      |
  | 重量 | 約1.21kg（付属のバッテリーパック（S）（約190g）装着時）<br />电源：約220g（電源コード（約60g）除く） |                      |

- CF-LX5PDT5S

  | 项目 | 配置                                  | 备注 |
  | ---- | ------------------------------------- | ---- |
  | 硬盘 | HDD：HGST HTS545032A7E680 （8MB缓存） |      |
  |      |                                       |      |
  |      |                                       |      |

  

## 2. 驱动更新

- 官方驱动

  https://askpc.panasonic.co.jp/s/download/install/lx5.html

- WIN10更新之后，缺乏的驱动都是属于 `Intel` 的相关内容。

  需要注意的是 `ME` 的版本，最新的话，电脑很容易宕机。

### 2.1 ME 固件

> `Intel® Converged Security and Management Engine` 或　`Intel Management Engine Software`  
> 固件更新需要到电脑生厂商的网页下载

- ME 固件（firmwire）更新：

  https://www.intel.cn/content/www/cn/zh/support/articles/000025619/software.html

## 3. 硬件升级

### 3.1 内存增设

### 3.2 硬盘更换

## 4. 系统安装

### 4.1 无法找到系统

- 原因描述

  安装过程中，出现错误，因为是 `UEFI` 方式，再启动的时候，BIOS会自动选择 HDD 进行启动。   
  然而，因为系统未能安装成功，所以导致出现 `An operating system wasn't found.`，无法启动。

- 解决方案

  进入 `BIOS` 设置，开启 `Popup Menu`;  
  再次启动，按 `ESC` 键，这样就可以选择从 `USB硬盘` 方式启动，再次进行安装。

  > 注意：BIOS未更新之前，可能是 USB3.0 的支持不是很好，所以在安装到 81% 的时候，无法继续前进，然后出现安装错误的错误。  
  > 把 USB硬盘，插入 USB2.0 的端口，就可以正常安装结束。

### 4.2 安装 `winget`

- 首先更新 `Microsoft Store`

  不更新的话，无法找到 `winget` 项目