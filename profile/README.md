# Hermod-Robotics

> 机器人工程的 AI Agent 原生基础设施。
>
> AI-native infrastructure for robot engineering.

---

## 我们做什么

**一份硬件描述文件，生成从固件到仿真的完整机器人项目。**

你写一个 `robot.hardware.yaml`，Hermod 自动生成：

| 输出 | 说明 |
|------|------|
| 固件 | STM32/ESP32 HAL 驱动，含自动 CAN ID 分配 + 冲突检测 |
| 机器人模型 | URDF/XACRO，从硬件清单直接生成 |
| ROS 2 驱动包 | ros2_control 硬件接口 + launch 文件 |
| 仿真 | Gazebo / MuJoCo 配置 |
| 文档 | BOM 物料清单 + 供电预算 + 接线图 |
| AI 上下文 | CLAUDE.md + .ai-workflows，Agent 开箱即用 |

## 核心仓库

| 仓库 | 说明 |
|------|------|
| [hermod](https://github.com/Hermod-Robotics/hermod) | 主仓库 — CLI + 代码生成引擎 + 模板 |
| [.github](https://github.com/Hermod-Robotics/.github) | 组织级配置 |

## 参与贡献

Hermod 是开源项目。欢迎提交硬件参数、模板或代码。

→ [贡献指南](https://github.com/Hermod-Robotics/hermod/blob/main/CONTRIBUTING.md)
