![Microduck 改装工作台概念插画：机器鸭与挂载支架、传感器板、滑轮脚和底座](https://microduck-mods-gallery.niftycucumber1.chatgpt.site/assets/github-header.jpg)

# Awesome Microduck Mods & Accessories

[English](README.md) · **简体中文**

## 可视化项目库

用图片和分类浏览全部项目：  
[打开 Microduck Mods Gallery →](https://microduck-mods-gallery.niftycucumber1.chatgpt.site/zh/)

> Microduck 鸭子改装与配件合集：可打印配件、充电底座、触摸传感器、电控改装和装机工具。

Microduck 是 Pollen Robotics / Hugging Face 的双足机器人。围绕这只机器鸭，社区正在做的事情已经从编写新动作延伸到改变它的身体：换上滑轮鞋、背一块计算板、制作能感知抚摸的头盖，或用另一套电机和电路重新组装整机。每一种改变背后，都可能有一套值得复用的图纸、代码和制作经验。

这个合集从“你想改哪一部分”出发，把这些分散的项目整理成八类。你可以来找一个校准托盘，也可以比较几条替代主控路线；既能看到独立发布的小配件，也能找到整机复刻仓库里的结构改件。目录面向想跟着制作的 DIY 用户，以及寻找技术参考、开发方向和合作对象的机器人开发者。

当前收录 **47 个项目**。每个条目介绍项目的用途、可获得的资料和关键进度，并链接作者维护的原项目。希望你看完简介，就能判断下一步是下载模型、阅读教程、研究代码，还是继续关注作者的实验。独立发布的配件和综合项目均按主要用途归类，同一个项目只列一次。

本合集独立维护，与 Pollen Robotics / Hugging Face 无隶属关系。所收录项目归各自作者所有；代码、图纸、模型和图片分别遵循原项目许可。头图为主题概念插画，不代表已验证的配件设计。

## Contents

- [可视化项目库](#可视化项目库)
- [Ecosystem Status · 生态现状](#ecosystem-status)
- [外观装扮](#外观装扮-appearance)
- [随身挂载配件](#随身挂载配件-mounts)
- [运动配件](#运动配件-motion-accessories)
- [供电系统](#供电系统-power-systems)
- [传感器扩展](#传感器扩展-sensors)
- [电控系统改装](#电控系统改装-electronics)
- [机身结构改进](#机身结构改进-mechanical-design)
- [装机辅助工具](#装机辅助工具-assembly-tools)
- [收录与贡献](#收录与贡献)
- [相关资源](#相关资源)

## Ecosystem Status

以下是截至 **2026-11-10**、基于本目录 47 个项目形成的观察。它们呈现出一个仍在边制作、边验证的改装社区：已经有人做出了可以展示和使用的改件，也有开发者在尝试新的结构、控制平台和交互方式。

**不少配件是从整机复刻中长出来的。** 社区作者选择不同的电机、主控和电池后，需要重新安排连接板、机身内部空间、脚掌和校准工具。例如 [Microduck-kissqy](https://github.com/kissqy/Microduck-kissqy) 包含可更换脚掌和腿部支撑，[CMU Microduck](https://github.com/qilinxiaoxiang/cmu-microduck) 则逐步调整头盖、脚踝、线夹和设备收纳结构。找配件时，整机仓库同样值得翻看；其中的小改件往往对应具体装配需求。

**已经有从文件走到实物的参考。** [microduck-tools](https://github.com/jackwuwei/microduck-tools) 同时提供校准托盘的打印文件和实际使用照片，[FabricTouch](https://github.com/JoyrayGu/Microduck-FabricTouch) 记录了触摸信号如何变成关节动作，一些复刻项目也展示了行走样机。想动手的人可以从这些材料了解制作过程，但复用时仍需对应作者的硬件版本：一套结构装得下的板子、一个电机适用的校准姿态，换到另一只鸭子上可能需要调整。

**新的玩法正在推动更完整的系统实验。** 自动回充需要底座、定位、运动控制和电气连接一起工作；[duckmind](https://github.com/joseyarashio/duckmind) 与 [Gonzalo Duck](https://github.com/ggoonnzzaallo/gonzalo_duck) 已公开相关方案和仿真实验，实体完整回充仍未验证。替换主控也有类似的阶段差异：[esp-duck](https://github.com/xingxingRealzyx/esp-duck) 已在真实小板上运行模型，[spacemit-microduck](https://github.com/fivif/spacemit-microduck) 则用开发板控制模拟鸭。这些进展提供了继续开发的起点，下一步还包括真实电机、供电和整机测试。

**资料开放程度决定了你能从哪一步接着做。** 有些项目提供可编辑设计和打印文件，有些公开电路与固件，也有项目主要分享照片、接口和使用步骤。因此，本目录同时记录“公开了什么”和“验证到哪一步”。实机进展来自作者公开记录，并非目录维护者逐项试装；选定项目后，请沿原链接查看对应版本的制造资料、装配说明和许可。

## 外观装扮 Appearance

给 Microduck 换一种样子：主题外壳、配色、服装和装饰件都属于这一类。只要清楚写明数字设计与实物验证的边界，仍在设计阶段的外观项目也可以收录。

- **[Microduck 配色与贴纸预览台](https://github.com/lucienxxxxxx/microduck-console)**（lucienxxxxxx）— 在浏览器里点选身体部件，先试配颜色和预设贴纸，再决定怎样制作外观。它本身不制造零件。工具代码为 MIT；官方网格和装配数据继续遵循 CC BY-NC-SA 非商业条件。

- **[Gritty 主题机器鸭](https://github.com/maddiedreese/gritty-microduck)**（maddiedreese）— 橙色毛绒、大眼睛和球衣造型的可编辑概念方案，并提供两段可复现的 MuJoCo 舞台动作。毛绒和衣服目前只是无质量、无碰撞的视觉几何，没有制作实体服装，也没有完成硬件验证。

## 随身挂载配件 Mounts

给鸭子增加一个携带设备或物品的位置。除了支架怎么固定，这类项目也需要考虑新增重量怎样影响运动。

- **[microduck-jetson-mount](https://github.com/adammong/microduck-jetson-mount)**（adammong）— 为 Microduck 加装 Jetson 计算板和外置电池，让额外的 AI 计算设备有地方安放。作者公开了可调整尺寸的三维设计、打印件，并在 MuJoCo 中模拟鸭子背上设备后的运动。目前还没有实物装机验证，部分仿真检查未通过，适合作为计算板挂载方案继续研究。

## 运动配件 Motion Accessories

从换一双脚掌到尝试高跷和秋千，这些项目把可打印附件与新的运动玩法联系起来。

- **[Microduck Playground](https://github.com/Vottivott/microduck-playground)**（Vottivott）— 围绕 Microduck 做的一组运动实验：包括秋千、高跷、攀爬梯等玩法，并分享附件模型和仿真资料，可以一起看道具怎么做、鸭子怎样使用它。高跷已有打印实物图，各项动作的实机进度不同。仓库还包含 MicroDock 自动回充底座，目前只做了设计与仿真，尚无实体充电结果。

- **[Microduck-kissqy](https://github.com/kissqy/Microduck-kissqy)**（kissqy）— 在 HD1910 电机复刻版上改进脚掌连接，让鸭子可以换用普通脚掌或滑轮鞋，也整理了腿部支撑和配套电路。适合想沿同一复刻路线尝试换脚玩法的人参考。滑轮鞋沿用官方设计，作者有实机资料，具体可用的动作需对应所采用的结构与软件版本。

## 供电系统 Power Systems

让鸭子获得电力，也探索怎样自己回到充电座。当前两项回充项目都把底座与停靠控制放在一起研究，尚未提供经过实体充电验证的完整方案。

- **[duckmind](https://github.com/joseyarashio/duckmind)**（joseyarashio）— 探索让 Microduck 在电量低时寻找底座，调整方向、倒入停靠位置，再坐下充电。项目把底座设计和这串行为一起放进仿真，适合研究自动回充的完整过程。已有[底座硬件规格](https://github.com/joseyarashio/duckmind/blob/HEAD/docs/dock-hardware.md)，目前“充上电”指模拟电池状态变化，实体充电尚未验证。

- **[Gonzalo Duck](https://github.com/ggoonnzzaallo/gonzalo_duck)**（ggoonnzzaallo）— 把自动回充分成找座、靠近、对接、充电监控和离座几个环节逐步开发。仓库有[充电方案](https://github.com/ggoonnzzaallo/gonzalo_duck/blob/HEAD/docs/charging-plan.md)、三维仿真和手动对接实验，可以参考底座与控制程序如何配合。自动找座和完整回充仍未跑通，真实充电条件及量产鸭子的安装适配也待确认。

## 传感器扩展 Sensors

让鸭子知道哪里被碰到，或者身体向哪边倾斜。触摸传感器服务于交互；姿态传感器（IMU）为运动控制提供身体倾斜和转动的信息。

- **[microduck_imu_to_ttl](https://github.com/avanx/microduck_imu_to_ttl)**（avanx）— 为自己组装 Microduck 的人制作姿态传感器板，让 LSM6DSV16X 的读数通过电机通信线路传回控制程序。项目包含电路和固件，适合需要自己接入 IMU 的复刻开发者。电路板已上电，飞特通信固件完成电脑端调试；接入实体鸭和 Dynamixel 通信支持仍待完成。

- **[imu-displace-microduck](https://github.com/Juxi-Technology/imu-displace-microduck)**（Juxi Technology）— 给采用 HD1910 电机的复刻鸭子换用 ICM-42670-P 姿态传感器，提供接线教程、程序补丁和独立的[传感器模块资料](https://github.com/Juxi-Technology/ICM42670P-High-Precision-IMU-Module)。已经能从真实传感器读到数据，下一步是让机器鸭控制程序完整使用这些读数。

- **[Microduck FabricTouch](https://github.com/JoyrayGu/Microduck-FabricTouch)**（JoyrayGu）— 给 Microduck 一层能感知触摸的织物“头皮”，把轻点、抚摸转成歪头或张嘴等反应。作者公开了压力信号采集、手势识别和电机控制实现，并有触摸响应的实机记录。当前需要电脑参与处理，多指触摸和颈部控制仍有限制，适合参考触摸交互如何接到真实动作上。

- **[my-microduck](https://github.com/ReadbytheBeach/my-microduck)**（ReadbytheBeach）— 计划把四块 12×12 压力感应阵列装到 Microduck 的头部和足底：头部用于触摸互动，足底用于感知与地面的接触。仓库整理了读取这些感应点的电路和通信方案，目前处于设计阶段，尚无整套电子皮肤完成实体部署的记录。

- **[LSM6DSV16X 裸 IMU 兼容库](https://github.com/sim336/lsm6dsv16x-sflp)**（sim336）— 让 Linux 主控通过 I2C 直接读取姿态芯片，并输出与现有 MCU 小板相同的 12 字节数据。测试覆盖寄存器、量程和安装方向等容易静默出错的问题。测量来自一块 Radxa 板，换主板或安装方向后仍需重新验证。

## 电控系统改装 Electronics

换一块主控、改用另一种关节电机，往往还要调整接线和控制程序。这里既有复刻用的连接板，也有让 Microduck 动作模型运行在不同计算平台上的尝试。

- **[microduck-community-kit](https://github.com/jyg9/microduck-community-kit)**（jyg9）— 把复刻 Microduck 时用到的几种小板集中整理：姿态传感器板负责读取身体倾斜，电池转接板负责接入电池，集线板负责连接多路电机。面向 HD1910 和 XL330 路线，附接线图、固件、调试工具和板件购买入口。作者报告已批量验证，整机装配仍需配合其他教程。

- **[microduck-replica](https://github.com/fanhao375/microduck-replica)**（fanhao375）— 把三维结构、内部电路和固件放在同一套复刻资料中，便于理解自己组装的鸭子怎样连起来。[硬件部分](https://github.com/fanhao375/microduck-replica/blob/HEAD/hardware/README.md)包含姿态传感器板、分线板和电池接口板，涉及 XL330、HD1910 两条路线。作者有 HD1910 实机运动记录，新版板件的测试进度需分别查看。

- **[Fanduck](https://github.com/7757/fanduck)**（7757）— 整机复刻项目中包含一块 [DCHUB 四口电机分线板](https://github.com/7757/fanduck/blob/HEAD/hardware/dchub-v1.1/README.md)，相当于鸭子内部的小分线插座，便于把头部和腿部的电机线路接在一起。作者公开了可编辑电路、制板文件和元件清单，适合需要自行制作连接板的人参考；采用时要对应接口线序和供电条件。

- **[Dukki](https://github.com/lachlanhurst/dukki)**（lachlanhurst）— 重新选择 Microduck 的“大脑”和关节电机，采用 Radxa CM4 计算模块与 Unitree J288 电机，再设计连接它们的电路和固件。作者希望获得更多计算余量，并探索不同的电机性能取舍。仓库有电路工程和 STM32 通信程序，整机仍在开发中。

- **[DuckBuddy](https://github.com/Animan-AI/DuckBuddy)**（Animan-AI）— 沿自己的硬件路线把语音、动作和自主行为组合成陪伴体验，让鸭子听到指令后连续执行动作。配套扩展板连接音频设备、供电和电机，仓库已有语音触发动作的实机记录，部分视觉和自主任务仍在验证。接口文档公开，PCB 制造设计未公开。

- **[Microduck Companion Project](https://github.com/RomdhoniZidane20/Microduck_companion_project)**（RomdhoniZidane20）— 用树莓派 4 搭建自己的 Microduck，并计划缩小参考的 Dynamixel 电机接口板，让连接电路能装进这套机身。项目目前提供技术规划和原理参考，可用于了解小机身内怎样安排电控；定制小板的制造与实机结果尚未确认。

- **[microduck-opi3w](https://github.com/Jimzjy/microduck-opi3w)**（Jimzjy）— 以采用 A733 芯片的 Orange Pi Zero 3W 作为 Microduck 主控，配合 HD1910 电机，调整扩展板、接线和运行软件。仓库整理了电路设计、姿态传感器固件和部署说明，便于沿这套零件组合继续搭建。主板已能启动，整机行走仍待装配验证。

- **[esp-duck](https://github.com/xingxingRealzyx/esp-duck)**（xingxingRealzyx）— 研究能否让小型 ESP32-S3 控制板承担 Microduck 的动作计算。作者把九个动作模型转换后装进同一份固件，可切换运行，并检查了计算精度、速度和真实姿态传感器输入。目前完成的是板端计算实验，电机通信与关节反馈尚未完整接通。

- **[spacemit-microduck](https://github.com/fivif/spacemit-microduck)**（fivif）— 把 Microduck 运行软件移植到 SpacemiT K3、K1 开发板，探索 RISC-V 主控路线。两款真实开发板都有控制 MuJoCo 模拟鸭的记录，K1 还提供摄像头到网页的传输实现。可参考软件移植与性能测量，当前结果不等于实体鸭已经换板完成。

- **[microduck-imx6ull](https://github.com/TonyRuan/microduck-imx6ull)**（TonyRuan）— 让 i.MX6ULL 开发板计算 Microduck 的关节动作，再连接 Mac 上的 MuJoCo 模拟鸭检查控制效果。作者提供动作模型转 C 代码的实现、性能测量和键盘控制界面，适合研究这类小主控能否带动机器人。真实电机与传感器尚未接入验证，部分动作仍不稳定。

- **[ArduPilot Neural Mixer](https://github.com/virtualrobotix/Ardupilot-Neural-Mixer)**（virtualrobotix）— 把机器鸭动作模型放进 ArduPilot 控制固件，尝试直接利用飞控板的计算、传感器和遥控接口驱动双足机器人。Microduck 是其参考机器人之一，已有仿真及 Pixhawk 6C Mini 真板参与的测试；独立驱动实体鸭还缺电机通信与关节反馈支持。

- **[RDK X5 Microduck](https://github.com/Xiaomiju-x/rdk-x5-microduck)**（Xiaomiju-x）— 记录一只采用 RDK X5 主控的鸭子怎样从采购、打印、装配走到实机调试。旧双电池样机通过动作序列实现短距离前进，新单电源布局已能启动和站立。项目保留了不同版本的接线与调试过程，带载供电和强化学习控制仍在推进。

- **[Xbotics MiniDuck Course](https://github.com/Xbotics-Embodied-AI-club/Xbotics-MiniDuck-Course)**（Xbotics）— 围绕自有电路板、电池和 HD1910 电机组织的 Microduck 复刻课程，将硬件版本、固件、动作模型、训练代码和烧录资料对应起来。适合沿作者的整套路线学习装机与训练；PCB 制造文件是否完整公开，仍需进一步核实。

- **[microduck-hd1910m](https://github.com/zhuoligetu123/microduck-hd1910m)**（zhuoligetu123）— 为采用 Radxa ZERO 3W 主控、HD1910M 电机和 BNO08x 姿态传感器的 Microduck 适配运行与训练软件，附接线资料和安卓控制端。项目解释了电机编号、转动方向与零位怎样对应；部分动作仍有偏航和回稳问题，仿真演示需与实机结果分开看。

- **[duck-a733](https://github.com/weilan157/duck-a733)**（weilan157）— 为已经选择 A733 主控的 Microduck 整理一份可写入 SD 卡的系统镜像，把启动系统和机器人应用按指定版本打包。它帮助这条改装路线减少逐个编译、安装和处理版本组合的工作，属于配套软件；硬件接线、关节校准和动作调试仍由对应方案完成。

- **[Radxa ZERO 3W Robot HAT](https://github.com/juper007/radxa-zero3w-robot-hat)**（juper007）— 为 Radxa ZERO 3W 设计紧凑扩展板，把 15 路 XL330 舵机、身体 IMU、I2C 传感器、麦克风、扬声器和受保护的 5V 供电接到一起。仓库有 KiCad、Gerber、BOM 和调试工具；V1 的电源与大电流布局仍在审查，尚未获得制造放行。

- **[Duck King S288 电机改型](https://github.com/zhanma666/Xihack2026_The_Duck_King)**（zhanma666）— 把 XL330 换成宇树 S288 舵机，提供重建后的 MuJoCo 模型、关节映射、安装脚本和训练任务。电机参数目前仍是占位值，BAM 执行器模型未建立，被动站立还会前倾；训练链路跑通不能当作实体 S288 鸭已经能走。

- **[Microduck 双电机虚拟实验室](https://github.com/gnana70/microduck-virtual-lab)**（gnana70）— 在采购舵机和装机前，用同一套固定版本的动作模型比较 XL330 与 HD-1910 的站立、行走偏航、侧推恢复和低电压表现。项目公开了 MuJoCo 脚本和结果文件，但所有数字都来自模拟，不能代替真实电机的扭矩、齿隙、供电和整机测试。

## 机身结构改进 Mechanical Design

让机身适应新的零件、制造方法或尺寸。这些项目中，有的修正局部装配问题，有的重新设计整只鸭子的结构。

- **[MICDUCK_FTHD1901_REBUILD](https://github.com/fengj4780-sudo/MICDUCK_FTHD1901_REBUILD)**（fengj4780-sudo）— 针对复刻件偏软、安装时互相顶住等问题，修改电机连接结构，并增加五个可选加强件。目标是让零件更牢、装配更顺，仓库提供 3MF 和 SolidWorks 文件。CNC 加强件仍在打样，电机型号还需按具体图纸核对，不能只看仓库名称。

- **[MicroDuck BoBoRedesign](https://github.com/AiBoBoMaker/MicroDuck-BoBoRedesign)**（AiBoBoMaker）— 保留熟悉的 Microduck 外形，把原来面向工厂制造的零件调整为适合个人 3D 打印的结构，并整理配套扩展板、姿态传感器板和代码。项目覆盖 XL330、HD1910 路线，参考了社区上游方案；适合研究打印与装配设计，各版实物进度需分别查看。

- **[microduck-original-look-v2](https://github.com/zhoudongT/microduck-original-look-v2)**（zhoudongT）— 尝试做一只外形尺寸放大两倍的 Microduck，为此重新设计电机夹座、传动支架和转接件，让实际零件能装进更大的身体。仓库提供 STEP 设计和装配检查资料，实物验证及部分连杆适配尚未完成，可作为大尺寸改版的结构研究起点。

- **[microduck-s288](https://github.com/zheflow/microduck-s288)**（zheflow）— 围绕另一套电机、主板和电池重新安排 Microduck 的机身，把外壳、内部支架和柔性脚底一起设计。公开了生成三维零件的 CAD 源码，适合研究替换内部元件后结构如何跟着改变。作者尚未完成整机装配，并明确提示当前版本不宜直接照图采购和打印。

- **[CMU Microduck](https://github.com/qilinxiaoxiang/cmu-microduck)**（qilinxiaoxiang）— 在 A7Z/OpenRB 复刻版上陆续改造头盖、脚踝、脚底、线夹和电子设备收纳结构，也加入触摸感知，让抓握头部能触发相应状态。仓库有零件清单、行走和触摸实机记录，能看到改件如何融入整机。电池背包目前只有设计，尚未装上使用。

- **[MicroDinosaur](https://github.com/eugenewang5425/MicroDinosaur)**（eugenewang5425）— 把 Microduck 改成使用 S288 舵机的小型双足恐龙，公开当前 Blender 总成、30 件打印工程、三件式零位校准架、六层头板和双总线软件。头板尚未打样，整机也没有完成实体装配、站立和行走验证。

- **[DuckLite](https://github.com/charlie8612/DuckLite)**（charlie8612）— 目标是用零售零件做一只约 150 美元、22 厘米高的低成本视觉双足机器人，并继续兼容 Microduck 的 50Hz 控制与 ONNX 动作接口。机械、电控、固件和仿真工作区已经划分，但目前仍在架构和器件选型阶段，下一步才是一条腿的执行器台架。

- **[Micro Cat](https://github.com/hwkim3330/micro-cat)**（hwkim3330）— 保留 Microduck 的 61 输入、14 输出动作接口，重新设计圆头、猫耳、尾巴、脚和内部机电布局。CAD 已检查打印空间、静态干涉和重心；还没有实体打印、装配、行走或耐久测试。

- **[HL-2909 电机适配打印件](https://github.com/MenciousL/microduck-hl2909-print)**（MenciousL）— 提供四个配合检具和 39 件整机 STL，帮助把 XL330 换成飞特 HL-2909。当前仍是图纸验证版，应先打印检具核对实物。项目没有解决供电：HL-2909 需要 9–14V，15 个电机还会增加约 67 克重量。

- **[Microduck × Stack-chan](https://github.com/meganetaaan/microduck-stackchan)**（meganetaaan）— 把竖置 M5Stack Tab5 屏幕变成机器鸭的头部，公开装配结构、暂定 BOM、训练过的无臂步态和浏览器模拟器。薄型手臂目前只是外观，不计入质量、碰撞和重新训练；实机接线、强度和安全仍待验证。

- **[IndieDuck Cyber Edition](https://github.com/armature-ai-labs/indieduck)**（Armature AI Labs）— 围绕一套共享机构组织可编辑 FreeCAD、STEP、STL、55 个打印件、BOM 和交互装配指南，并允许更换不同外壳。R25 的装配步骤只经过 CAD 审查，线缆、强度、传感器、供电和实体步态都尚未验证。

- **[飞特复刻电源支架针脚避让改件](https://github.com/weishengwu6/microduck-build-log)**（weishengwu6）— 在电源支架上增加避让孔，避免 IMU 舵机后方针脚在装配时顶住支架。作者公开了修改后的 STEP 和 SolidWorks 文件，但还没有打印和实物试配；间隙、固定强度和线束位置仍需检查。仓库中的其余结构资料主要来自 fanhao375 上游。

## 装机辅助工具 Assembly Tools

装鸭子时先把身体托稳，再把关节摆到规定位置。这些工具帮助完成安装与零位校准，让软件记录的关节位置对应正确的实体姿势。

- **[microduck-tools](https://github.com/jackwuwei/microduck-tools)**（jackwuwei）— 将电机校准工作台与可打印托盘配合使用：托盘承托 Microduck 的头部、身体和双脚，工作台负责连接电机、检查并设置零位。仓库有 STEP、STL 和实际使用照片，适配 XL330-M288-T 电机及作者指定的校准姿态。

- **[JIG-190](https://github.com/superobk/microduck-cad)**（superobk）— 在安装、检查和校准时托住 Microduck，让操作者腾出双手处理关节与接线。[R5 设计目录](https://github.com/superobk/microduck-cad/tree/HEAD/projects/microduck-stand/r5-compact-full15)公开了 STL、3MF 和组装图，可以查看支架怎样接触身体。R5.0-rc1 尚待切片与实物试配，关节零位仍需配合软件设置。

- **[MHDuck](https://github.com/MHDuck/microduck)**（MHDuck）— HD1910 电机和 BNO085 姿态传感器复刻路线中的[零位校准参考](https://github.com/MHDuck/microduck/blob/master/%E6%A0%A1%E5%87%86.md)，展示怎样用定位工装托住鸭子、摆正身体，再设置关节。运行源码、动作文件和[训练仓库](https://github.com/MHDuck/microduck_rl)已公开；工装目前可参考照片和使用步骤，尚未找到可直接打印的设计文件。

- **[Wamoduck](https://github.com/Wamotech/Wamoduck)**（Wamotech）— 为自己的整机重设计制作[站立零位校准架](https://github.com/Wamotech/Wamoduck/tree/HEAD/hardware/fixtures/standing-zero)，用四个打印件把机器人支承在指定姿态，便于按统一基准调整关节。STEP、STL 和打印工程已公开，实物试配状态待确认；结构对应 Wamoduck，尚未确认适配官方成品。

- **[Microduck 舵机装机工具](https://github.com/masszhou/microduck-notes)**（masszhou）— 包含 DSH 网页操作台和 Mac 命令行台架，用于整机装配前搜索、检查、归中并小心测试 15 个 XL330 舵机。工具记录位置、电流、温度和总线错误，并设置显式运动限制。编码器中位只是台架参考，不是鸭子装好后的站立零位。

## 收录与贡献

欢迎提交配件、改装方案，也欢迎补充现有项目的制作教程和实机进展。请提供原项目链接、作者、建议分类，并用一小段话说清楚：**做了什么、别人能从哪里开始、目前做到哪一步**。只有设计、只有仿真也可以提交，把状态写清楚即可。

整机复刻项目请指出具体改件或硬件适配内容。同一项目只收录一次，仅复制上游的副本不重复收录。提交自己的项目或存在合作关系的项目时，请注明关系。

本目录独立维护，项目由各自作者维护，收录不代表官方推荐。代码、图纸、模型和图片的使用条件以原项目许可为准，引用时请保留作者与来源。

## 相关资源

- [Microduck 官方运行软件](https://github.com/pollen-robotics/microduck) — 原版控制程序、设备接口和使用文档。
- [Microduck 官方训练环境](https://github.com/pollen-robotics/microduck_rl) — 训练动作模型，研究新机身、电机或脚部接触方式对应的运动控制。
- [Awesome Microduck](https://github.com/joeynyc/awesome-microduck) — 更广泛的 Microduck 社区导航，覆盖软件、仿真、动作模型和相关资源。本目录的分类与条目形式参考该项目，内容聚焦改装和配件。
