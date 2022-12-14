# 飞控设置

## 固件烧写

下载QGC：[QGC - QGroundControl - Drone Control](http://qgroundcontrol.com/)

打开QGC到该界面

![](../img/set_uav1.png)

刷入PX4最新发布版固件。

如需刷入老板固件则在该网站下载：[Releases · PX4/PX4-Autopilot (github.com)](https://github.com/PX4/PX4-Autopilot/releases)

## 飞控初始化设置

按照QGC软件提示分别设置

**机架**为X8型

![](../img/set_uav2.png)

按提示校准标红的传感器

校准遥控器

![](../img/set_uav3.png)

设置飞行模式以及7通道断电

![](../img/set_uav4.png)

设置电源

![屏幕截图 2022-12-17 164836](../img\屏幕截图 2022-12-17 164836.png)

## QGC相关参数更改

`CBRK_USB_CHK`为197848 为了让插了USB之后还可以解锁

`CBRK_IO_SAFETY` 为22027 跳过安全开关

`CBRK_SUPPLY_CHK` 为894281 跳过电源检测

`SYS_TEL1_BAUD`为921600 改串口波特率

`EKF2_HGT_MODE`

![](../img/set_uav6.png)

`EKF2_AID_MASK`

![](../img/set_uav7.png)

## 调整电机转向

转向见桨叶安装

在此界面逐个测试电机，若电机转向错误，任意调换该电机的两根三相电源线。切记带电调试勿安装桨叶

![](../img/set_uav8.png)
