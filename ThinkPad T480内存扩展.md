# ThinkPad T480 硬件扩展

> https://blog.kabocy.com/repair-custom/5062/

该机价格低廉，但是拥有很好的硬件可扩展性，很多笔记本电脑缺乏这种可扩展性。当然了，一般也不需要什么扩展，购买的时候，保证电脑性能够用就好。

- 具备 2 个内存插槽；

  内存容量（16GB、8GB x 2）（32GB、16GB x 2）  
  根据他人实践，该电脑支持 （64GB、32GB x 2）  

  - Crucial 16GB DDR4-3200 SODIMM
  - Crucial 8GB **DDR4-2666** SODIMM
  - Crucial 8GB DDR4-3200 SODIMM
  - Crucial 4GB DDR4-2400 SODIMM（DDR4-2400　PC4-19200　SO-DIMM）

- 硬盘接口： 1 个 M.2 SSD，1 个 2.5inch 的 SATA 接口。

- 至于CPU的更换，是装在BGA上的，不能轻易升级。不过，想升级 CPU 的个人，估计是基本没有的。

  该 CPU 跑分不高，6000分左右；相对于当前的动辄就是 10000 分，AMD的 20000 分比较，是比较落后了。但是足够用。  
  注）关键是找不到一台能够像 E480 这样可以扩展的好笔记本电脑。

- 重量：1.75kg～

- 屏幕：180度开放展示

- USB Type-C 供电

注）ThinkPad E490 是完全一样的框体，理论上具有 ThinkPad E480 一样的可扩展性。

## 1. 内粗扩展

### 1.1 拆机

- 拆卸电池  
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-Image_20230927_111309_411.jpg?resize=750%2C562&ssl=1)

- 将 ThinkPad T480 翻转过来，卸下圈出的所有螺丝。  
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T4804-1024x768.jpg?resize=750%2C563&ssl=1)
  
- 拆开位置  
    ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T4806-1024x768.jpg?resize=750%2C563&ssl=1)

  拆开难度较大。

- 内存图像  
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T4807-1024x768.jpg?resize=750%2C563&ssl=1)
  
- 拆除内部电池  
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T4808-1024x768.png?resize=750%2C563&ssl=1)
  
- 内存插槽  
![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T4809.jpg?resize=750%2C562&ssl=1)



### 1.2 取出内存

- 从 ThinkPad T480 中取出内存。
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T48015.jpg?resize=750%2C485&ssl=1)
  
- 然后，DIMM 移动（竖起）大约 30 度，慢慢地将它从主板上取下。

  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T48015.jpg?resize=750%2C485&ssl=1)

### 1.3 最大 64GB 内存支持

不管是 Lenovo 的官网、还是 Intel 的官网，i5-8250u 支持的最大内存都是 32GB。但是个别网站给的说明却是可以支持最大 64GB 的内存。

- https://www.compuram.biz/memory/lenovo/notebook/thinkpad/e-series/e480/64gb-dual-channel-memory-kit-xb13d.htm

  为啥会出现内存容量较官方资料更高？
  https://www.compuram.de/blog/en/maximise-the-maximum/

  大部分可能是：当产品出现的时候，还没有更高密度的内存。例如 E480 出现的时候，还没有单条 32GB 的内存模块，只有最大单条 16Gb 的内存，所以官方没有验证过 32GB 的内存条到底是否可以用。作为官方，必然是保守的，所以他们声明的最大内存只能是 16GBx2=32GB。  
  而后期，出现了 32GB 的单条内存，官方并不会去验证新出现的内存是否可以用。毕竟更新旧的各种文档，对官方来说，是很要命的事情。

## 2. 硬盘改造 - M.2 SSD

### 2.1 M.2 SSD - 2280

ThinkPad T480的 m.2 SSD 支持高速PCIe连接和NVMe接口。
可更换的 SSD 为 CT500P2SSD8 (500GB) 或 CT1000P2SSD8 (1TB)。

- 拔除SSD连接线  
![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T48013-1024x768.jpg?resize=750%2C563&ssl=1)
- 拔除之后的图像  
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T48014-1024x768.jpg?resize=750%2C563&ssl=1)
- 拆除固定螺丝  
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T48016-1.jpg?resize=750%2C562&ssl=1)
- 取出硬盘盒  
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T48019.jpg?resize=750%2C562&ssl=1)

### 2.2 M.2 SSD - 2242

这类SSD较少，估计很难买到，虽然大多数设备都有该接口，主要用于WIFI接口。

- 设备位置  
  ![img](https://i0.wp.com/object-storage.tyo1.conoha.io/v1/nc_87e0d0f3f9904537b1d6cf637a61937a/blog/2023-09-T4807-1.jpg?resize=750%2C562&ssl=1)

## 3. Wi-Fi 模块拆卸

我认为更换Wi-Fi模块的机会不多，但希望在ThinkPad E480上使用Hacintosh或Wi-Fi时用BCM94352Z更换Wi-Fi模块时有所帮助模块发生故障。

- ThinkPad E480拆Wi-Fi模块时，用刮刀将红圈处的天线拆下，拆下红圈处的螺丝，将Wi-Fi模块从连接器中拔出。

  ![img](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4917_R-1024x683.png)



## 其它型号电脑的可扩展性

- ThinkPad E490

  完全一样的框体，具有和 ThinkPad E480 完全一样的可扩展性。

- ThinkPad E14 Gen 3(AMD)

  - 只有一个内存插槽。 所有型号都有 8GB 板载内存（直接连接到主板）。 8GB内存款只有8GB板载，12GB有4GB板载+8GB插槽，16GB有8GB板载+8GB插槽，24GB有8GB板载+16GB插槽。
  - 一共有3个M.2插槽，其中2个用于存储。 靠近 CPU 冷却器的 M.2 插槽仅适用于 Type-2242，靠近扬声器的 M.2 插槽适用于 Type-2280。

  ThinkPad E14 Gen 2(Intel) 具有完全一样的框体，具有一样的可扩展性。
  
- Thinkpad T14s

  - 内存：板载内存，没有任何增设的可能。