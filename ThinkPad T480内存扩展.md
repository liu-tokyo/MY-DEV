# ThinkPad E480 硬件扩展

该机价格低廉，但是拥有很好的硬件可扩展性，很多笔记本电脑缺乏这种可扩展性。当然了，一般也不需要什么扩展，购买的时候，保证电脑性能够用就好。

- 具备 2 个内存插槽；

  内存容量（16GB、8GB x 2）（32GB、16GB x 2）  
  根据他人实践，该电脑支持 （64GB、32GB x 2）  

  - Crucial 16GB **DDR4-3200** SODIMM
  - Crucial 8GB DDR4-2666 SODIMM
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

- 将 ThinkPad E480 翻转过来，卸下圈出的所有螺丝。

  ![img](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4952_R-1024x683.png)

- 将抹刀插入 ThinkPad E480 的一角，然后慢慢取下爪子。  
    如果在这里用力过大，可能会折断爪子，损坏零件，甚至伤到自己，所以要小心。

  ![img](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4958_R-1024x683.png)

- 当所有的爪子都被移除时，底盖就会从主体上脱落。  

  ![img](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4950_R-1024x683.png)

- 打开ThinkPad E480的底盖，可以看到内存、M.2 SSD、2.5英寸（7mm厚）SATA存储、Wi-Fi卡、电池等。

    ![ThinkPad E480のボトムカバーを外した様子](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4896_R-1024x683.png)



### 1.2 取出内存

- 从 ThinkPad E480 中取出内存。  
  向外移动每个锁定臂。

  ![img](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4909_R-1024x683.jpg)

- 然后，DIMM 移动（竖起）大约 30 度，慢慢地将它从主板上取下。

  ![img](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4921_R-1024x683.jpg)

### 1.3 插入新内存

我这里用的是三星的16GB（8GB x 2）（推荐是Crucial的8GB x 2），不过32GB也可以装。 另外，虽然超过了厂商的最大容量，但似乎可以用64GB。

- 将新内存插入插槽并向下推内存，直到它被锁定臂固定。
  注）内存是有方向的，插入前检查槽口的位置。

  ![img](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4943_R-1024x683.jpg)

  

## 2. 硬盘改造 - m.2 SSD

ThinkPad E480的 m.2 SSD 支持高速PCIe连接和NVMe接口。
可更换的 SSD 为 CT500P2SSD8 (500GB) 或 CT1000P2SSD8 (1TB)。

- 拆卸时，拆下红色圈出的螺丝，轻轻取下立起的SSD。

  ![img](https://blog.kabocy.com/wp-dir/wp-content/uploads/2020/11/IMG_4908_R-1024x683.png)

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