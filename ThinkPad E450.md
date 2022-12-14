## ThinkPad E450

> 这款机器是不附带 **M.2** 固态硬盘接口的，机器只有一个 SATA 硬盘位，可以将机械硬盘替换成 SATA 接口的固态硬盘。
>
> 型号：20DC-CT01WW
>
> Memory Support: Max. Memory Size: 16 GB (DDR3L 1333/1600, LPDDR3 1333/1600)  
> Socket: FCBGA1168  
> Typical TDP: 15 W

### 设备规格

| 项目                   | 规格                                    | 备注                                    |
| ---------------------- | --------------------------------------- | --------------------------------------- |
| CPU                    | Core i3 4005U(Haswell)<br/>1.7GHz/2コア | **1647**                                |
| 画面サイズ             | 14 型(インチ)                           |                                         |
| 解像度                 | WXGA (1366x768)                         |                                         |
| メモリ規格             | DDR3L PC3-12800                         |                                         |
| メモリ容量             | 4GB                                     |                                         |
| メモリスロット（空き） | 2(1)                                    |                                         |
| ストレージ容量         | HDD：500GB                              | 5400 rpm                                |
| OS                     | Windows 8.1 Update 64bit                | Microsoft Office Home and Business 2013 |
| ビデオチップ           | Intel HD Graphics 4400                  |                                         |
| 重量                   | 1.81 kg                                 |                                         |
| 幅x高さx奥行           | 339x24.4x239 mm                         |                                         |

### 设备性能

| 型号                          | 性能     | 备注                              |
| ----------------------------- | -------- | --------------------------------- |
| Intel Core i3-4005U @ 1.70GHz | **1645** | CPU First Seen on Charts: Q1 2014 |
| -                             |          |                                   |
| -                             |          |                                   |



### 驱动更新

> 官方网址：https://pcsupport.lenovo.com/jp/ja/products/laptops-and-netbooks/thinkpad-edge-laptops/thinkpad-e450/downloads/driver-list
>
> 联想驱动工具：https://newsupport.lenovo.com.cn/driveDownloads_index.html  
> 　　需要把内核语言修改为 中文简体 之后，再安装该工具比较合适，否则可能出现乱码。好像是多虑了，最新版本已经能够对应日文。

Windows 10 22H2 安装之后，至少如下驱动需要更新：

| 驱动问题                                      | 说明                 | 解决办法 |
| --------------------------------------------- | -------------------- | -------- |
| PCIデータ取得およびシグナル処理コントローラー | 联想驱动工具可以解决 |          |
| SMバスコントローラー                          | 联想驱动工具可以解决 |          |
| 电池显示无法充电                              | 电池电芯驱动更新     |          |

### CPU升级

**Socket: FCBGA1168**

| 可以升级CPU型号               | 跑分 | 生产日期 | 功率TDP |
| ----------------------------- | ---- | -------- | ------- |
| Intel Core i3-4005U @ 1.70GHz | 1647 | Q1 2014  | 15 W    |
| Intel Core i7-5500U @ 2.40GHz | 2752 | Q1 2015  | 15 W    |
|                               |      |          |         |

二手市场很难找到 低电压版 的 CPU 。



### 系统安装

#### 1. Windows 10 22H2 日文版

- 已经更新到最新日期（2022.12.30）

- 追加了中文语言输入

  中文输入的时候，键盘布局适应日语 106 键盘，可以免去中日文键盘布局不同的困扰。

#### 2. Microsoft Office 2007 Enterprice 日文版

- 已经更新到最新日期（2022.12.30）

虽然不是最新的 Office，但是对于普通办公已经足够用。

#### 3. 驱动更新

- Lenovo System Update

  官方的驱动更新工具

- 联想驱动工具

  是对 `Lenovo System Update` 的一个补充，虽然 `Lenovo System Update` 可以更新大部分的驱动，但是对个别驱动的支持还有有缺陷，所以需要安装这个工具。

  注意：该工具为中文的 Lenovo 官方工具，并不提供日文版本，所以安装的时候需要把 OS 的内核设置为 简体中文，否则会出现乱码的情况。

  该工具可以正确识别到 OS 为日文，安装每个驱动的时候，也能自动显示日文安装。

- 补充说明

  经过上面 2 个官方工具，驱动都能够正常找到、安装。

  如果出现驱动未被安装的情况，一般来说，都是下载 驱动精灵 来解决问题；当然也有很多其它解决驱动问题的工具，例如 鲁大师 等。

#### 4. Typora 安装

作为最流行的 Markdown 编辑工具，用 Typora 编辑文档，可以代替我们日常工作中的大部分 Office 文档。尤其是在团体协作的时候，Markdown 可以更好的作差分，所以是 IT 人士的必备工具。

- Windows 版的最终免费版本（0.9.96）；
- 调整了显示画面宽度（E450 的显示宽度本身只有 1366，所以效果不是很好，对 1920 宽度的屏幕效果很好）
- 调整了代码显示宽度（E450 的显示宽度本身只有 1366，所以效果不是很好，对 1920 宽度的屏幕效果很好）

#### 5. 清除 Windows 自带无用软件

- Windows 10 开始，安装之后带有很多我们日常工作中完全不需要的软件，清除这些软件。
- Windows 10 开始，还会自动帮你安装一些它自认为有用的软件，这些功能一律关闭。

