#  从 U 盘安装系统



## 目录
1. `FAT32`,`NTFS`,`exFAT` 的区别
2. `USB HDD`和`USB ZIP`区别 



## 内容
### 1. `FAT32`,`NTFS`,`exFAT` 的区别

NTFS、FAT32、exFAT是我们使用电脑最常见的分区了，它们之间有什么区别呢。 NTFS、FAT32、exFAT一个比较概念性的东西，建议如果是移动硬盘就算则NTFS，如果是U盘等采用exFAT闪存为介质的存储设备，exFAT或者兼容性的FAT32比较好，下面小编就来给大家分析**NTFS、FAT32、exFAT区别**。如下图：

| **分类**           | **FAT32**       | **NTFS**    | **exFAT**         |
| ------------------ | --------------- | ----------- | ----------------- |
| **操作系统**       | Win 95 OSR2之后 | Win2000之后 | WinCE 6/Vista SP1 |
| **最小扇区**       | 512bytes        | 512bytes    | 512bytes          |
| **最大扇区**       | 64KB            | 64KB        | 32768KB           |
| **最大单一文件**   | 2bytes-4GB      | 无限制      | 16EB(理论值)      |
| **最大格式化容量** | 32GB            | 2TB         | 16EB(理论值)      |
| **档案数量**       | 4194304         | 无          | 至少可以大于1000  |

FAT32是在FAT16基础上发展而来，随着Windows 95 OSR2一起发布，可以被大多数操作系统支持，FAT32更有效地利用了硬盘空间，并且最大分区的上限已经达到了32GB，适合一般家庭使用。

NTFS可以支持的分区(如果采用动态磁盘则称为卷)大小可以达到2TB。而Win 2000中的FAT32支持分区的大小最大为32GB。NTFS可以比FAT32更有效地管理磁盘空间，最大限度地避免了磁盘空间的浪费。

exFAT是Microsoft在Windows Embeded 5.0以上中引入的一种适合于闪存的文件系统，为了解决FAT32等不支持4G及其更大的文件而推出。对于闪存，NTFS文件系统不适合使用，exFAT更为适用。

来自网友的总结: 
1. fat32在该分区有错误的时候会有一个记录生成。然后记着那一点有错误。再次存东西的时候不就会存在那里。但是因为技术问题fat32不支持单文件大于4GB的文件 
2. NTFS虽然可以存放大于4GB的单文件但是又没有记录功能，如果分区有错误然后新数据存到了错误区。。可想而知。等来的只是文件损坏丢失。 
上面说的那些错误区指的是软错误，是可以修复的。 
3. exFAT相当于综合了上面的两个优点。即可以存放单文件4GB以上的（而且那个理论值相当的大），而且还会记录错误。。。


### 2. 启动模式(写入模式)`USB HDD`和`USB ZIP`的区别 
把U盘做启动盘，其实就是要把 U 盘模拟成可启动设备，达到仿真的效果。启动模式就是一种把U盘模拟成相应的启动设备，推荐选择 USB-HDD，这种方式兼容性强，仿真效果较好。不过具体用哪种，还要看电脑主板的支持。现在大多主板都支持 USB-FDD 和 USB-HDD。还有一些可能会有-16和-32的区别，非常古老的电脑一般用-16；支持win7电脑的我一般就采用-32。

1. `USB-HDD`: 硬盘仿真模式，DOS启动后显bai示C:盘，HP U盘格式化工具制作的U盘即采用此启动模式。此模式兼容性很高，但对于一些只支持USB-ZIP模式的电脑则无法启动。 　　

2. `USB-ZIP`: 大容量软盘仿真模式，DOS启动后显示A盘，FlashBoot制作的USB-ZIP启动U盘即采用此模式。此模式在一些比较老的电脑上是唯一可选的模式，但对大部分新电脑来说兼容性不好，特别是大容量U盘。

### 3. 优启通把 U 盘制作成系统启动盘的默认操作界面
| -----------   |
| ------------ |
| 选择磁盘: 对应的 U 盘 |
| 写入模式: USB-HDD; 分区格式: NTFS |
| 选择壁纸: 略 |



