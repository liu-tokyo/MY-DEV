# Thinkpad X250

## 1. 电脑配置

| 项目         | 说明                                        | 备注                      |
| ------------ | ------------------------------------------- | ------------------------- |
| 系统制造商   | LENOVO                                      |                           |
| 系统型号     | 20CLA03PJP                                  |                           |
| 主板产品     | 20CLA03PJP                                  |                           |
| 主板版本     | SDK0E50510 WIN                              |                           |
| 系统 SKU     | LENOVO_MT_20CL_BU_Think_FM_ThinkPad X250    |                           |
| CPU          | Intel Core i5-5300U @ 2.30GHz               | `1632`/`2730` - `Q1 2015` |
| 内存         | 8GB                                         | `PC3-12800 DDR3L SDRAM`   |
| 硬盘         | 256GB（SSD）                                |                           |
| 主机编号     | 20CLS2A11JPCO7P713                          | WDCWDS250G2B0A-00SM50     |
| 主板         | 20CLS2A11J（SDKOE50510WIN）<br />20CLA03PJP |                           |
| 网卡（有线） | Intel(R）Ethernet Connection (3）1218-LM    |                           |
| 网卡（无线） | Intel（R) Dual Band Wireless-AC 7265        |                           |
| 声卡         | Realtek High Definition Audio               |                           |
| 显卡         | Microsoft Remote Display Adapte             |                           |



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

- 设备分解  
  https://jp.ifixit.com/Guide/Lenovo+ThinkPad+X250+Ram+-+Storage+Replacement/178042?lang=en

### 3.1 磁盘信息

- 磁盘信息

  ```
  PS C:\Users\VIP> Get-WmiObject -Class Win32_DiskDrive | Select-Object Model, FirmwareRevision
  
  Model                      FirmwareRevision
  -----                      ----------------
  SAMSUNG MZ7TY128HDHP-000L1 MAT04L0Q
  ```

  硬盘的详细信息和评价：

  #### 🔍 产品概述

  | **规格**     | **描述**                                                     |
  | ------------ | ------------------------------------------------------------ |
  | **型号系列** | **Samsung CM871a 系列**                                      |
  | **容量**     | **128 GB**                                                   |
  | **接口**     | SATA 6.0 Gbps (SATA III)                                     |
  | **尺寸**     | 2.5 英寸，7mm 厚度 (标准笔记本硬盘尺寸)                      |
  | **闪存类型** | **TLC** (Triple-Level Cell)                                  |
  | **目标用途** | 通常用于 **OEM 市场** (即预装在品牌电脑如联想 ThinkPad 等笔记本中)。 |

  #### 🌟 性能与特点

  作为一款 OEM 市场面向的入门级或主流级 SSD，它的主要特点如下：

  - **性能方面：**
    - **读写速度：** 属于 SATA 接口 SSD 的正常范畴。根据测试数据，其**连续读取速度**大约在 **487 MB/s** 左右，**连续写入速度**在 **237 MB/s** 左右（写入速度相对较低）。
    - **随机读写 (IOPS)：** 随机读取 IOPS 约为 94000，随机写入 IOPS 约为 32000，性能表现一般，但对于日常家用和办公来说，仍远优于传统的机械硬盘（HDD）。
  - **可靠性：**
    - **MTBF (平均故障间隔时间)：** 标称为 **150 万小时**，属于消费级 SSD 的标准水平。
  - **用途：**
    - 这款 SSD 是许多老款笔记本电脑或台式机进行升级的理想选择，可以将系统从机械硬盘迁移到 SSD，大幅提升系统启动速度和程序加载速度。

  #### 👍 总结评价

  这款 SSD **怎么样**，取决于您的需求和它目前的状况：

  | **场景**              | **评价**                                                     |
  | --------------------- | ------------------------------------------------------------ |
  | **日常使用 (系统盘)** | **非常好**。对于老旧电脑来说，从机械硬盘升级到这款 128GB SSD，能带来巨大的性能飞跃，用于安装操作系统和日常软件绰绰有余。 |
  | **作为全新产品**      | **性能一般**。如果与当前市场上的主流消费级 SSD（如三星 870 EVO）相比，它的性能参数要略低一些，尤其是写入速度。 |
  | **作为二手/拆机件**   | **性价比高**。由于是 OEM 型号，市面上多为拆机或二手良品。如果价格合适，且**健康度（如通过 CrystalDiskInfo 检查）良好**，它仍然是一个可靠且划算的选择。 |
  | **专业/重度应用**     | **不适合**。如果您是专业用户，需要频繁进行大量数据的写入（如视频编辑、大型文件传输），建议选择性能更强、容量更大的 NVMe 或更高端的 SATA SSD。 |

  **简而言之：** MZ7TY128HDHP-000L1 是一款 **可靠、成熟的三星 OEM 级 SSD**，特别适合作为**旧电脑的系统升级盘**，提供稳定且快速的日常使用体验。
