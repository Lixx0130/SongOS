# SongOS
A really simple toy OS that can be done in a few hours.

### Step 1 简单引导启动程序
设置软盘启动，软盘映像文件选择 [boot.img](step1/boot.img)<br>
启动后可看到下面界面，并听到蜂鸣器响声。
（若虚拟机为bochs则听不到，这里用的是VMware）

![image](boot界面.png)

### Step 2 简单多任务操作系统
本操作系统参考了Linux-0.00，具体网址点击 [Linux.old](http://oldlinux.org/Linux.old/bochs/)<br>

设置软盘启动，软盘映像文件选择 [SongOS.img](step2/SongOS.img)<br>
启动后可看到下面界面，

![image](SongOS_1.png)

任务0和任务1分别输出A，B

![image](SongOS_2.png)

### U盘实机启动
在 linux 下 make 得到 **Image文件**<br>
将 **Image文件** 的值复制到U盘起始位置后保存（即修改第一个扇区值）<br>
修改U盘工具随意，winHex示例如下:

![image](U盘启动.png)

之后只要确保PC支持从U盘启动即可。
