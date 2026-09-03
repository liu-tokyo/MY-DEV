# ThinkSystem HR650X

> 序列号 J30AHFRV

## 阵列卡

- RAID 530-8i

  ```
  https://iknow.lenovo.com.cn/detail/164186
  ```

  画面的最下部，有驱动下载的地址。

## 官方支持

- 驱动下载

  https://datacentersupport.lenovo.com/cn/zh/products/servers/thinksystem-hyperscale/hr650x/downloads/driver-list/



## WinPE导出阵列卡驱动

> 在优启通 PE 中找出 **530-8i 实际正在使用的驱动 → 找到对应 `.inf/.sys/.cat` → 注入到已经安装在硬盘上的 Windows 10 → 再启动测试。**

不过有一个重要区别：**不要简单把整个 PE 的 `DriverStore` 全部复制进去**，而是应该先确定 530-8i 的实际驱动包，再用 `DISM` 或 `pnputil` 正确注入。

### 1. 先在优启通 PE 找 530-8i 的驱动

在 PE 中运行：

```powershell
pnputil /enum-devices /class SCSIAdapter
```

或者：

```powershell
pnputil /enum-devices /connected
```

找到类似：

```powershell
Broadcom / LSI MegaRAID
RAID 530-8i
SAS
```

然后记下它的：

```powershell
Driver Name
Driver Version
Provider Name
```

尤其是：

```powershell
Published Name : oemXX.inf
Driver Version : ...
Provider Name  : ...
```

------

### 2. 找到这个 `oemXX.inf` 对应的完整驱动包

例如：

```powershell
pnputil /enum-drivers
```

找到对应的：

```powershell
Published Name : oem42.inf
Original Name  : ...
Provider Name  : Broadcom
Class Name     : SCSIAdapter
Driver Version : ...
```

然后可以进一步找到实际文件位置。

通常驱动会在：

```powershell
X:\Windows\System32\DriverStore\FileRepository\
```

例如：

```powershell
X:\Windows\System32\DriverStore\FileRepository\megasas2.inf_amd64_xxxxxxxx
```

**不要只复制一个 `.sys` 文件。**

一个完整驱动通常至少包括：

```powershell
.inf
.sys
.cat
```

以及 INF 引用的其他文件。

------

### 3. 更推荐：直接把驱动包导出来

如果 PE 的 `pnputil` 支持 `/export-driver`，可以直接：

```powershell
pnputil /export-driver oem42.inf D:\5308i-driver
```

或者：

```powershell
pnputil /export-driver * D:\AllDrivers
```

但我**不建议一开始导出 PE 的全部驱动**。

最好先确定 530-8i 对应的 `oemXX.inf`，然后只导出它。

------

### 4. 把驱动注入已经安装好的 Win10

假设：

```powershell
C: = Windows 10 所在分区
D: = PE U盘
D:\5308i-driver = 530-8i 驱动
```

可以：

```powershell
dism /Image:C:\ /Add-Driver /Driver:D:\5308i-driver /Recurse
```

如果成功，会看到类似：

```powershell
The operation completed successfully.
```

然后：

```powershell
wpeutil reboot
```

------

### 5. 甚至可以不需要重新安装 Windows

这是我比较建议你现在尝试的方案。

你现在的情况是：

```powershell
Windows 10 已经安装
       ↓
第一次启动
       ↓
Windows Logo
       ↓
一直转圈
```

你可以进入优启通 PE，然后直接对现有 Windows 10：

```powershell
DISM /Image:C:\ /Add-Driver /Driver:D:\5308i-driver /Recurse
```

**这样相当于在 Windows 10 第一次启动之前，把 530-8i 驱动强行塞进去。**

然后重新启动。

如果这次能够正常进入 Windows 10，那么基本就能证明：

> **之前就是 Windows 10 启动阶段缺少/没有正确加载 530-8i 驱动。**

------

### 6. 一个很重要的细节

你的目标不是“找一个 RAID 驱动就行”。

**530-8i 的驱动版本必须尽量匹配。**

因为 PE 里面可能存在：

```powershell
旧版 MegaRAID 驱动
新版 MegaRAID 驱动
Windows 10 驱动
Windows 11 驱动
Server 2019/2022 驱动
```

所以我建议你先在优启通 PE 执行：

```
pnputil /enum-devices /class SCSIAdapter
```

以及：

```powershell
pnputil /enum-drivers
```

把**与 530-8i 有关的那几段完整输出**贴给我。

我可以帮你判断：

**① PE 实际使用的是哪个 INF → ② 驱动包在哪 → ③ 是否适合 Windows 10 → ④ 应该用 `pnputil` 还是 `DISM` 注入 → ⑤ 注入后还需要不要修改启动配置。**

而且，**如果你把优启通 PE 的 `pnputil /enum-devices /class SCSIAdapter` 输出贴出来，我可以直接从里面开始判断，不需要你先重新安装一次。**



## 离线清除消费级驱动

使用 Dism++ 清理系统中的多余驱动（尤其是消费级显卡驱动），需要进入优启通 PE 中操作。由于此时系统还未正式装好或无法进入桌面，必须通过 **Dism++ 的“离线管理”功能**来挂载并修改目标系统的驱动库。

操作步骤如下：

### 1. 进入 PE 并打开 Dism++

1. 用优启通 PE 引导启动 ThinkSystem HR650X。
2. 进入 PE 后，打开 **Dism++** 工具。
3. 点击左上角的 **“文件”** -> **“打开会话”**。
4. 在弹出的窗口中，选择你刚刚安装了系统的那个盘（例如 `C:\`），然后点击确定。Dism++ 会开始加载该系统的运行环境和驱动缓存。

### 2. 进入驱动管理界面

1. 载入会话成功后，点击左侧导航栏中的 **“驱动管理”**。
2. 稍等几秒钟，Dism++ 会列出该系统当前加载的所有第三方驱动程序。

### 3. 识别并清理多余/显卡驱动

1. 在驱动列表中，仔细查看“驱动描述”、“类别”或“提供商”这一栏。
2. 寻找与显卡相关的第三方驱动（例如包含 **Intel Graphics**、**NVIDIA**、**AMD** 或消费级集显/独显名称的驱动包）。
   - *注意：联想服务器通常使用的是 **ASPEED（阿斯派德）** 显示芯片，或者基础的微软基本显示驱动。如果里面有消费级的核显/独显驱动，通常就是导致启动卡死的罪魁祸首。*
3. 勾选这些需要清理的消费级显卡驱动。
4. 点击右下角的 **“删除驱动”** 按钮。

### 4. 保存与收尾

1. 清理完成后，可以顺便在驱动管理里看一下有没有缺失的服务器芯片组或存储驱动，顺便点“添加驱动”把HR650X的官方INF驱动注入进去。
2. 关闭 Dism++ 会话，拔掉 U盘，重启服务器，观察是否能正常跳过 Windows Logo 进入系统。