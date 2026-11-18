# Advanced Opus 5.5 Generated Simulations & Models

Opus 5.5 在交互式 3D 物理解释器、机器拆解仿真、电路设计与验证、复杂物理求解器方面表现出色。以下为可用于教学平台的高级示例与工具链。

## 1. Konstantin Saifoulline — airsup.ai/lab

- **主站**: https://airsup.ai/lab
- Opus 5.5 生成的 30+ 交互机器与仿真，可拆解、参数调整。
- **代表作品**:
  - Raptor 3 火箭发动机（可拆解，观察氧气/甲烷流路、涡轮泵、冲击钻石）
  - 聚变反应堆
  - 5 轴 CNC 机床
  - 机器人狗 / 机器人蜘蛛（完整部件、线缆）
  - Starlink 仿真
  - 光学分拣机、仓库决策系统、火山仿真等
- **教学价值**: “Kids will grow up learning like this.” — 完全可交互的物理/工程解释器。

## 2. Ryan Sael 的交互实验室

- **Lens Lab**: https://lens.lab.sael.net  
  镜头对焦原理（玻璃元件移动、焦平面、光圈、爆炸视图）。一次提示生成。
- 数据中心热管理、河流弯曲、无限程序化城市等其他 3D 交互作品。
- 展示了 Opus 5.5 长时间自主构建复杂 3D 物理场景的能力。

## 3. OpenPhysicsAI

- **Website**: https://openphysicsai.org/
- **GitHub**: https://github.com/molanocortes/OpenPhysicsAI
- 20+ 验证过的物理求解器（流体、冲击波、火、热、固体、声、电磁、轨道等）。
- 原生 3D 应用 + CLI + **MCP 服务器**，AI 智能体可直接驱动。
- 有 “flags” 挑战：用自己的 AI 改进求解器并提交 PR，机器评分。
- 极其适合研究级与高级物理教学。

## 4. 其他高级示例与工具链

- **Carbon Physics Engine + Opus**: Claude 智能体生成复杂物理场景（倒水、螺母、岩石爬行车、衣服折叠等）。
- **Awesome Opus 5.5 Frontend Showcases**: https://github.com/OpenVGLab/awesome-opus5.5-frontend-showcases  
  大量 Three.js / WebGL 3D 交互示例。
- **threejs-skills / Claude Skill Packages**: 专为 Claude 设计的 Three.js 技能包，加速 3D 物理场景生成。
- **build123d-claude-plugin**: Claude 写参数化 CAD，导出 STEP。
- Techartist 系列（已在主 README 中）：完整交互 3D 物理课本。

## 如何用于你的仿真教学平台

1. **嵌入现有交互仿真**：链接或 iframe airsup.ai/lab、lens.lab.sael.net、Techartist 课程。
2. **生成定制仿真**：用 Opus 5.5 + Three.js 生成针对课程的专属 3D 解释器，导出后上传平台。
3. **电路模型**：结合 circuits-advanced.md 中的 SPICE 工作流。
4. **研究级**：引入 OpenPhysicsAI 或自己用 Opus 生成求解器，导出数据与可视化。

更新时间：2026-11-18
