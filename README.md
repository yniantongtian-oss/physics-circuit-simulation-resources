# Physics & Circuit Simulation Resources (Opus 5.5 Related)

整理自 X 和相关来源的物理类、电路类教学仿真资源，适合用于低代码平台搭建仿真教学平台（外部软件先仿真，再填充进平台）。

## 1. 交互式 3D 物理教学资源（强烈推荐 - Techartist）

用 Opus 5.5 + Three.js 构建的浏览器可交互 3D 课本/仿真：

- **GCSE/IGCSE 电学（Electricity）**  
  7 课：电荷、电流 → 插座插头等。  
  - X 帖：https://x.com/techartist_/status/2117659337057517831  
  - 官网：https://iamtechartist.com/

- **Every Joule（能量专题）**  
  完整 10 课：动能、重力势能、弹性、效率、发电站、能量守恒等。  
  - 官网：https://iamtechartist.com/every-joule/  
  - Lesson 1 GitHub：https://github.com/iamtechartist/every-joule-lesson1

- **光与光学**  
  反射、折射、透镜、眼睛、颜色 + A-level 干涉。

- **Moving Charges and Magnetism（电磁学）**  
  电流导线受力、电机原理等。

- **飞机如何飞行**  
  空气动力学 10 课。

官网主页：https://iamtechartist.com/

## 2. 真实电路设计 + SPICE 仿真（硬核模型）

- **模拟合成器完整项目**  
  Claude Code + Opus 5.5 从零设计：KiCad 原理图、**ngspice 仿真**、Python 行为模型、PCB、固件。  
  - 博客：https://cpldcpu.github.io/2026/11/14/touchsynth/  
  - GitHub（含仿真模型、netlist、报告）：https://github.com/cpldcpu/TouchSynth/

- **Opus 设计电路并用 SPICE 验证**  
  https://github.com/orgs/micropython/discussions/19680  
  例子：任意波形生成电路、模拟 Pong（BJT/运放）、超声波测距等，pySpice 代码。

- **Flux AI + Opus 5.5**  
  硬件/电路设计：https://www.flux.ai/p/blog/flux-opus-5-5

## 3. 推荐外部仿真工具（先仿真再填充）

| 工具 | 用途 | 链接 |
|------|------|------|
| Falstad Circuit Simulator / CircuitJS | 网页电路仿真（教学神器） | https://www.falstad.com/circuit/ |
| LTspice / ngspice / SPICE OPUS | 专业电路仿真 | https://www.spiceopus.si/ |
| PhET Interactive Simulations | 物理教学经典 | https://phet.colorado.edu/ |
| MATLAB / Simulink | 复杂物理/电路模型 | - |

## 4. 其他相关 Opus 5.5 仿真示例

- 机械键盘 3D 拆解仿真
- NVIDIA GPU 历代拆解
- PS5 手柄完整拆解
- 跳水物理仿真对比等

## 使用建议（低代码平台教学仿真平台）

1. 用外部工具（Falstad、LTspice、PhET 等）先做好核心仿真实验。
2. 导出视频、数据、图表、动画。
3. 填充进泛微 E10 / E-Builder 平台：
   - 页面嵌入视频/图片
   - 数据导入报表
   - 参数表单 + 预跑结果
   - AI 知识库讲解原理
   - 课程管理与流程

---

整理时间：2026-11-18  
用途：云端杯低代码+AI 平台应用搭建创新大赛 - 仿真教学平台参考
