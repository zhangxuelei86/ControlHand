---
title:  "机械手控制程序"

---
该程序实现是的对仿人机械手双手的正逆运动学控制，同时包括数据手套的连接和数据读取部分，同时还包括连接python程序的手势识别和掌腕关节角度预测部分。
### 文件

* 3DSModel 文件包括所有的模型的3DS文件，其中的robotic hand包括程序所需要用到的仿人机械手模型。
* 5DT文件夹中包括数据手套连接所需要用到的库文件和头文件，还有.jc的数据手套校准文件，以及两个识别模型
* CalculateThetaByCoordinate.m等matlab文件用于计算机械手的逆运动学部分
---
### GloableVariable
包括定义的一些机械手的全局变量，包括手指的长度及坐标值
### 3DSReader
读取3ds文件的程序
### 3DSLoaderView
下拉菜单的点击事件函数实现
### MainFrm
mfc的主界面
### getPythonData
初始化python模块并完成函数的调用和值得返回
### GloveSampleDlg
数据手套数据读取界面
### RobotHand
机械手的主要控制程序，包括正逆运动学的实现