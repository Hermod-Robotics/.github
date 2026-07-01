<p align="center">
  <img src="https://raw.githubusercontent.com/Hermod-Robotics/.github/main/assets/Hermod_Logo.jpg" alt="Hermod" height="120">
</p>

<h1 align="center">Hermod-Robotics</h1>

<p align="center">
  <strong>AI-native infrastructure for robot engineering.</strong>
</p>

<p align="center">
  <a href="README.zh-CN.md">中文</a>
</p>

---

## What We Build

**One hardware description file. A complete robot project — from firmware to simulation.**

Write a `robot.hardware.yaml`. Hermod generates:

| Output | Description |
|---|---|
| Firmware | MCU HAL drivers with auto CAN ID allocation and conflict detection |
| Robot Model | URDF/XACRO generated directly from the hardware manifest |
| ROS 2 Driver | `ros2_control` hardware interface and launch files |
| Simulation | Gazebo / MuJoCo configuration |
| Documentation | BOM, power budget, and wiring diagram |
| AI Context | `CLAUDE.md` — AI agents understand your robot out of the box |

### How It Works

```
robot.hardware.yaml          # You write this
        │
        ▼
   Hermod Engine              # Validates, resolves knowledge base, generates
        │
        ▼
  Complete Project            # Firmware + URDF + ROS 2 + Sim + Docs
```

### Why Hermod?

Traditional robot development requires manually wiring together hardware datasheets, firmware boilerplate, URDF modeling, ROS drivers, and simulation configs — weeks of setup before you write a single line of application logic. Hermod collapses this to **one file and one command**, with AI agents that understand your hardware constraints from day one.

---

## Repositories

| Repository | Description |
|---|---|
| [hermod](https://github.com/Hermod-Robotics/hermod) | Core — CLI, code generation engine, templates |
| [.github](https://github.com/Hermod-Robotics/.github) | Org-level defaults |

---

## Contribute

Hermod is open source. Hardware parameters, templates, and code contributions are welcome.

→ [Contribution Guide](https://github.com/Hermod-Robotics/hermod/blob/main/CONTRIBUTING.md)

---

<p align="center">
  <sub>Named after Hermóðr, the Norse messenger who crossed boundaries between worlds — carrying intent across hardware, software, and AI.</sub>
</p>
