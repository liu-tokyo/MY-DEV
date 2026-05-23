# Thinkpad X240

> 电脑型号：20AL00BAJP

## 1. 电脑配置

| 项目         | 说明                                     | 备注                                                        |
| ------------ | ---------------------------------------- | ----------------------------------------------------------- |
| CPU          | Intel Core i3-4010U @ 1.70GHz            | `903`/`1659` - `Q1 2013`                                    |
| 内存         | 4GB                                      | Max. Memory Size: 16 GB (DDR3L 1333/1600, LPDDR3 1333/1600) |
| 硬盘         | 1TB（HDD）                               |                                                             |
| 主机编号     | 20CLS2A11JPCO7P713                       | WDCWDS250G2B0A-00SM50                                       |
| 主板         | 20AL00B9JP（SDKOE50510WIN）              |                                                             |
| 网卡（有线） | Intel(R）Ethernet Connection (3）1218-LM |                                                             |
| 网卡（无线） | Intel（R) Dual Band Wireless-AC 7265     |                                                             |
| 声卡         | Realtek High Definition Audio            |                                                             |
| 显卡         | Microsoft Remote Display Adapte          |                                                             |



## 2. 驱动安装

- BIOS  
  更新 2024.12

- 官网  
  https://pcsupport.lenovo.com/us/en/products/laptops-and-netbooks/thinkpad-x-series-laptops/thinkpad-x240/downloads/driver-list

- `Lenovo System Update` 更新部分：
  
  关键更新：
  
  | 项目                                       | 说明         | 备注 |
  | ------------------------------------------ | ------------ | ---- |
  | Intel HD Graphics Driver-10[64]            | 显卡驱动     |      |
  | Realtek High Definition Audio Driver-10 64 | 声卡驱动     |      |
  | Intel WLAN Driver for 7260-10 [64]         | 无线网卡驱动 |      |
  
  推荐更新：
  
  | 项目                                                         | 说明              | 备注               |
  | ------------------------------------------------------------ | ----------------- | ------------------ |
  | Intel Rapid Storage Technology Driver-10 164]                | 磁盘快速存取      | 下载失败，手动更新 |
  | RealtekMedia Card Reader Driver CWindows 10 Version 1607 orLaten | SD读卡器驱动      |                    |
  | Realtek Media Card Reader Driver CWindows 10 Version 1607 orLaten | SD读卡器驱动（2） | 估计是错误识别     |
  | Lenovo Power Management Driver-7/8/8.1/10 [64]               | 电源管理驱动      |                    |
  | Synaptics UltraNav Driver-10 [32,64]                         | 触控板驱动        |                    |
  | ThinkPad Hotkey Features Integration Package Setup- 10/11    |                   | 可选更新           |
  
  手动更新：
  
  | 项目                                                         | 说明            | 备注         |
  | ------------------------------------------------------------ | --------------- | ------------ |
  | Intel Management Engine 9.5 Firmware                         | ME固件更新      | 9.5.65.3000  |
  | Lenovo Power and Battery Driver                              | Lenovo 电池驱动 | 10.1.10.0    |
  | Intel Collaborative Processor Performance Control (CPPC) driver |                 | 1.0.0.1018   |
  | Intel Rapid Storage Technology Driver                        | 磁盘快速存取    | 14.8.16.1063 |
  | Intel Bluetooth Software                                     | 无线蓝牙驱动    | 20.60.0.4    |
  
  
  
- Windows10安装之后，无法自动识别的设备：

  | 设备名称 | 硬件ID                         | 驱动名称                                                     |
  | -------- | ------------------------------ | ------------------------------------------------------------ |
  | 未知设备 | USB\VID_8087&PID_07DC&REV_0001 | 无线蓝牙驱动                                                 |
  | 未知设备 | ACPI\VEN_INT&DEV_33A0          | Intel Smart Connect Technology<br />在 BIOS (UEFI) 中禁用英特尔智能连接技术。 |
  
  

## 3. 设备升级

- 设备分解  
  https://jp.ifixit.com/Guide/Lenovo+ThinkPad+X240+Ram+-+Storage+Replacement/178042?lang=en
