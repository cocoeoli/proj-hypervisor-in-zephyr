# proj-hypervisor-in-zephyr
## 题目
基于Zephyr RTOS实现type-2型虚拟化管理平台。

## 项目描述：
基于实时操作系统Zephyr的虚拟机 Zephyr-based Virtual Machine（ZVM），是一种参考Kernel-based Virtual Machine（KVM）实现的虚拟机，其面向高性能嵌入式计算环境，提供嵌入式平台上的资源隔离和共享服务。

本项目以Zephyr实时操作系统为基础，使用C（C++）在Zephyr RTOS中实现一个面向嵌入式平台的虚拟机管理器。Zephyr RTOS是一个小型的实时操作系统，用于连接、资源受限和嵌入式设备，支持多种架构，发布于Apache License 2.0下。Zephyr包括内核、所有组件和库、设备驱动程序、协议栈、文件系统和固件更新，以开发连接、资源受限和嵌入式设备。Zephyr RTOS易于部署、安全、连接和管理。它具有不断增长的软件库集，可用于各种应用和行业领域，如工业物联网、可穿戴设备、机器学习等。

Zephyr系统整体结构和Linux类型，可以参考KVM思路，实现基于Zephyr RTOS的虚拟化管理平台，有助于更好的理解KVM等复杂虚拟化系统的实现原理。同时考虑在嵌入式等资源受限场景下的虚拟化实现需要注意哪些内容。

## 参考资料：
##### (1) https://docs.zephyrproject.org/latest/ 
##### (2) kvm in linux
##### (3) https://gitee.com/openeuler/zvm（arm64平台基础功能）

## 所属赛道
2023全国大学生操作系统比赛的“OS功能挑战”赛道

## 参赛要求
以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2023年春季学期或之后本科毕业的大一~大四的学生）或研究生
如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
请遵循“2023国大学生操作系统比赛”的章程和技术方案要求

## 项目导师
谢国琪 xgqman@hnu.edu.cn

## 难度
中等 ~ 高 等

## 特征：
1. 使用 C/C++ 语言实现
2. 至少支持一种硬件平台（比如x86, arm, riscv等）
3. 支持 QEMU模拟机器上运行/支持在物理机器上运行
4. 为了兼容Zephyr社区开源协议，License建议为：Apache License 2.0 license

## 预期目标
#### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标
#### 注：为了避免重复造轮子，本项目既可以从头开发，也可以联系导师在其项目基础上进行进一步的开发

1. 能够在QEMU模拟平台上运行，能够支持启动至少两个及以上虚拟机（Linux, Zephyr）。
2. 能够支持对虚拟机的基本操作，例如创建、运行、挂起、终止等。
3. 能够支持虚拟机间的通信（可选拓展）。
4. 能够支持虚拟机上运行实时应用（可选拓展）。
5. 能够支持virtIO等设备虚拟化框架（可选拓展）。

