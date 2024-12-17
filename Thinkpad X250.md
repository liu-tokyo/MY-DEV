# Thinkpad X250

## 1. 电脑配置

| 项目         | 说明                                     | 备注                      |
| ------------ | ---------------------------------------- | ------------------------- |
| CPU          | Intel Core i5-5300U @ 2.30GHz            | `1632`/`2730` - `Q1 2015` |
| 内存         | 8GB                                      | `PC3-12800 DDR3L SDRAM`   |
| 硬盘         | 256GB（SSD）                             |                           |
| 主机编号     | 20CLS2A11JPCO7P713                       | WDCWDS250G2B0A-00SM50     |
| 主板         | 20CLS2A11J（SDKOE50510WIN）              |                           |
| 网卡（有线） | Intel(R）Ethernet Connection (3）1218-LM |                           |
| 网卡（无线） | Intel（R) Dual Band Wireless-AC 7265     |                           |
| 声卡         | Realtek High Definition Audio            |                           |
| 显卡         | Microsoft Remote Display Adapte          |                           |



## 2. 驱动安装

- 官网  
  https://pcsupport.lenovo.com/us/en/products/laptops-and-netbooks/thinkpad-x-series-laptops/thinkpad-x250/downloads/driver-list

- Windows11 安装之后，无法自动识别的设备：

  | 设备名称                     | 硬件ID                                       | 驱动名称                                                     |
  | ---------------------------- | -------------------------------------------- | ------------------------------------------------------------ |
  | PCI 设备                     | PCI\VEN_10EC&DEV_5227&SUBSYS_222617AA&REV_01 | [Realtek PCIE CardReader](https://www.driverscape.com/download/realtek-pcie-cardreader) |
  | PCI 数据捕获和信号处理控制器 | PCI\VEN_8086&DEV_9CA4&SUBSYS_222617AA&REV_03 | [Intel(R） Dynamic Platform and Thermal Framwork Chipset Participand](https://www.driverscape.com/download/intel%28r%29-dynamic-platform-%26-thermal-framework-processor-participant-driver) |
  | 未知设备                     | ACPI\VEN_LEN&DEV_0068                        | [Lenovo Power Management driver](https://pcsupport.lenovo.com/us/en/products/laptops-and-netbooks/thinkpad-x-series-laptops/thinkpad-x250/downloads/driver-list/component?name=Power%20Management&id=E1B533C3-16CA-4FBE-8BD8-FB5D7A57F431) |
  | 未知设备                     | ACPI\VEN_INT&DEV_340F                        | [Intel Collaborative Processor Performance Control](https://pcsupport.lenovo.com/us/en/products/laptops-and-netbooks/thinkpad-x-series-laptops/thinkpad-x250/downloads/driver-list/component?name=Power%20Management&id=E1B533C3-16CA-4FBE-8BD8-FB5D7A57F431) |

  

### 3. 设备升级

