<p align="center">
  <img src="https://raw.githubusercontent.com/Hermod-Robotics/.github/main/assets/Hermod_Logo.png" alt="Hermod" height="120">
</p>

<h1 align="center">Hermod-Robotics</h1>

<p align="center">
  <strong>机器人工程的 AI Agent 原生基础设施。</strong>
</p>

<p align="center">
  <a href="README.md">English</a>
</p>

---

## 我们在做什么

**一份硬件描述文件，生成从固件到仿真的完整机器人项目。**

写一个 `robot.hardware.yaml`，Hermod 自动生成：

| 输出 | 说明 |
|---|---|
| 固件 | MCU HAL 驱动，含自动 CAN ID 分配与冲突检测 |
| 机器人模型 | URDF/XACRO，从硬件清单直接生成 |
| ROS 2 驱动 | `ros2_control` 硬件接口与启动文件 |
| 仿真 | Gazebo / MuJoCo 仿真配置 |
| 文档 | BOM 物料清单、供电预算、接线图 |
| AI 上下文 | `CLAUDE.md` — AI Agent 开箱即用 |

### 工作流程

```
robot.hardware.yaml          # 你只需要写这个
        │
        ▼
   Hermod 引擎               # 校验、查询知识库、生成
        │
        ▼
  完整项目                   # 固件 + 模型 + 驱动 + 仿真 + 文档
```

### 为什么用 Hermod？

传统机器人开发需要手动翻阅硬件手册、编写固件样板代码、手写 URDF 模型、配置 ROS 驱动和仿真环境，数周准备之后才能开始写业务逻辑。Hermod 将这一切压缩为「一个文件 + 一条命令」，且 AI Agent 从第一天就理解你的硬件约束。

---

## 仓库

| 仓库 | 说明 |
|---|---|
| [hermod](https://github.com/Hermod-Robotics/hermod) | 主仓库 — CLI、代码生成引擎、模板 |
| [.github](https://github.com/Hermod-Robotics/.github) | 组织级配置 |

---

## 参与贡献

Hermod 是开源项目。欢迎提交硬件参数、模板或代码。

→ [贡献指南](https://github.com/Hermod-Robotics/hermod/blob/main/CONTRIBUTING.md)

---

<p align="center">
  <sub>以北欧神话信使 Hermóðr 命名 — 他在九个世界之间传递消息，不畏任何边界。正如 Hermod 在硬件、软件与 AI 之间传递设计意图。</sub>
</p>
