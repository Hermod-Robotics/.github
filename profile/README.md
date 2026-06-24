<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)">
    <img alt="Hermod-Robotics" height="64">
  </picture>
</p>

<h1 align="center">Hermod-Robotics</h1>

<p align="center">
  <strong>AI-native infrastructure for robot engineering.</strong><br>
  <sub>机器人工程的 AI Agent 原生基础设施。</sub>
</p>

---

## What We Build &nbsp;/&nbsp; 我们在做什么

**One hardware description file. A complete robot project — from firmware to simulation.**

一份硬件描述文件，生成从固件到仿真的完整机器人项目。

Write a `robot.hardware.yaml`. Hermod generates:

写一个 `robot.hardware.yaml`，Hermod 自动生成：

| Output &nbsp;/&nbsp; 输出 | Description &nbsp;/&nbsp; 说明 |
|---|---|
| Firmware &nbsp; 固件 | MCU HAL drivers with auto CAN ID allocation & conflict detection &nbsp; 含自动 CAN ID 分配与冲突检测 |
| Robot Model &nbsp; 机器人模型 | URDF/XACRO generated directly from hardware manifest &nbsp; 从硬件清单直接生成 |
| ROS 2 Driver &nbsp; ROS 2 驱动 | `ros2_control` hardware interface + launch files &nbsp; 硬件接口与启动文件 |
| Simulation &nbsp; 仿真 | Gazebo / MuJoCo configuration &nbsp; 仿真配置 |
| Documentation &nbsp; 文档 | BOM, power budget, wiring diagram &nbsp; 物料清单、供电预算、接线图 |
| AI Context &nbsp; AI 上下文 | `CLAUDE.md` + `.ai-workflows` — agents understand your robot out of the box &nbsp; Agent 开箱即用 |

### How It Works &nbsp;/&nbsp; 工作流程

```
robot.hardware.yaml          # You write this / 你只需要写这个
        │
        ▼
   Hermod Engine              # Validates, resolves knowledge base, generates
   引擎层                      # 校验、查询知识库、生成
        │
        ▼
  Complete Project            # Firmware + URDF + ROS 2 + Sim + Docs
  完整项目                    # 固件 + 模型 + 驱动 + 仿真 + 文档
```

### Why Hermod? &nbsp;/&nbsp; 为什么用 Hermod？

Traditional robot development requires manually wiring together hardware datasheets, firmware boilerplate, URDF modeling, ROS drivers, and simulation configs. Weeks of setup before you write a single line of application logic. Hermod collapses this to **one file and one command**, with AI agents that understand your hardware constraints from day one.

传统机器人开发需要手动翻阅硬件手册、编写固件样板代码、手写 URDF 模型、配置 ROS 驱动和仿真环境，数周准备之后才能开始写业务逻辑。Hermod 将这一切压缩为「一个文件 + 一条命令」，且 AI Agent 从第一天就理解你的硬件约束。

---

## Repositories &nbsp;/&nbsp; 仓库

| Repository &nbsp;/&nbsp; 仓库 | Description &nbsp;/&nbsp; 说明 |
|---|---|
| [hermod](https://github.com/Hermod-Robotics/hermod) | Core — CLI, code generation engine, templates &nbsp; 主仓库：CLI、代码生成引擎、模板 |
| [.github](https://github.com/Hermod-Robotics/.github) | Org-level defaults &nbsp; 组织级配置 |

---

## Contribute &nbsp;/&nbsp; 参与贡献

Hermod is open source. Hardware parameters, templates, and code contributions are welcome.

Hermod 是开源项目。欢迎提交硬件参数、模板或代码。

→ [Contribution Guide &nbsp; 贡献指南](https://github.com/Hermod-Robotics/hermod/blob/main/CONTRIBUTING.md)

---

<p align="center">
  <sub>Named after Hermóðr, the Norse messenger who crossed boundaries between worlds — carrying intent across hardware, software, and AI.</sub><br>
  <sub>以北欧神话信使 Hermóðr 命名 — 在硬件、软件与 AI 之间传递设计意图。</sub>
</p>
