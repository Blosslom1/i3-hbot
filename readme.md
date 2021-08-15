# 3Dimension Printer

## 机器简介

本项目中含有三台打印机结构。依次迭代更新。

i3进程&远程挤出结构，家用级，适合慢速打印，快速会出现较多震纹，精度普通最高达到0.1mm。

主控芯片采用的mega2560芯片，固件改写的为marlin1.1.9

驱动使用4个A4988（双z并联），可以根据自己经济能力改用TMC2209或闭环驱动。

hbot，高精工业级，可以实现高速打印在影响质量较小的情况下是i3速度的4-8倍速，最高精度可达0.025mm。主控是32位LPC1768，固件升级为marlin2.0.x

本hbot打印机是由上一版本i3结构改造，设计理念围绕低成本，高性能 ，在采购原始材料尽量使用的未加工的材料成本较低。

制作流程请跟随本文指示。

### 第一步

参看原始设计图，使用solid work2019，打开根目录的装配体1，看懂机械原理有大概机器布局印象后进行材料采购。

### 第二步

使用excel打开根目录BOM表。名称为i3_BOM（由于零件细碎未整理hbot的bom，仅仅增加几个2020铝型材大体没有怎么变）。

### 第三步

打印件定制，设计图纸的非标零件都需要定制，使用FMD打印定制即可，可以进入hbot打印件中查看需要定制的零件种类。

### 第四步

主板如果使用mega2560，使用arduino(先安装程序固件\arduino-1.8.13-windows.exe)写入程序固件中的程序程序目录：程序固件\Marlin-2.0.x\Marlin\Marlin.ino

主板使用skr等32位主板，使用卡烧录，firmware.bin文件，文件已经调试编译好可以直接烧录。

## 暂停更新











