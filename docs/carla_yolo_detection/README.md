* # 自动驾驶感知与控制系统研究 (基于 CARLA)

  ## 1. 项目简介
  本项目旨在通过 Python 脚本与 CARLA 仿真环境进行深度交互，搭建一个基础的自动驾驶测试环境。项目将探索如何利用深度学习视觉算法和虚拟传感器数据，实现对仿真世界中动态物体的检测、环境感知以及基础的车辆控制。

  ## 2. 选题说明
  * **参考开源项目:** [kamilkolo22/AutonomousVehicle](https://github.com/kamilkolo22/AutonomousVehicle)
  * **重构思路:** 原项目部分模块对 Windows 系统兼容性较差，本项目提取其“视觉识别 + 传感器交互”的核心架构，在 Windows 环境下使用纯 Python 配合 PyTorch 进行完全重构，以确保跨平台的易用性和代码的可读性。

  ## 3. 开发运行环境
  * **操作系统:** Windows 10/11
  * **仿真平台:** HUTB CARLA_Mujoco_2.2.1
  * **编程语言:** Python 3.8
  * **核心框架:** PyTorch (支持 CUDA 加速), OpenCV
  * **开发工具:** Visual Studio Code / Anaconda

  ## 4. 模块结构与入口
  * 本模块的所有核心代码存放于 `src/carla_yolo_detection` 目录下。
  * 模块的主程序入口为 `main.py`。