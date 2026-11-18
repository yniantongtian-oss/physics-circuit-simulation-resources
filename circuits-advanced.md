# Advanced Circuit Simulation Tools & AI Methods (电路仿真与模型)

整理专业级电路仿真工具、开源方案以及用 Opus 5.5 / Claude 生成与验证电路的方法。

## 1. 主流开源 / 免费电路仿真工具

| 工具 | 类型 | 最适合 | 链接 / 备注 |
|------|------|--------|-------------|
| **ngspice** | SPICE 引擎 | 脚本化、后端仿真 | https://ngspice.sourceforge.io/ — KiCad、Qucs-S 后端 |
| **Qucs-S** | 图形化 SPICE | 大学教学、RF/混合信号 | https://github.com/ra3xdh/qucs_s — 支持 ngspice/Xyce/SpiceOpus |
| **KiCad + ngspice** | EDA + 仿真 | 从原理图到 PCB | 内置仿真，免费开源 |
| **LTspice** | 专业 SPICE | 功率电子、模拟 | Analog Devices 免费下载 |
| **QSPICE** | 新一代 SPICE | 现代行为模型 | Qorvo，LTspice 原作者开发，支持 C++/Verilog |
| **Xyce** | 高性能 SPICE | 大规模电路 | Sandia National Labs，开源 |
| **Falstad / CircuitJS** | 浏览器动画 | 教学入门 | https://www.falstad.com/circuit/ |
| **Logisim-evolution** | 数字逻辑 | 数字电路教学 | GitHub 开源 |

## 2. AI + SPICE 工作流（Opus 5.5 时代）

### 核心思路
让 LLM 生成可仿真的 netlist / PySpice 代码，而不是纯文字描述。仿真器给出客观验证。

- **实例讨论**: https://github.com/orgs/micropython/discussions/19680  
  Opus 5.5 设计任意波形生成电路、模拟 Pong、超声波测距等，用 pySpice 验证。

- **TouchSynth 项目**: https://github.com/cpldcpu/TouchSynth/  
  完整模拟合成器：KiCad + ngspice 仿真 + Python 行为模型 + PCB + 固件。

- **ltspice-mcp**: https://github.com/cognitohazard/ltspice-mcp  
  MCP 服务器，让 Claude 直接调用 LTspice / ngspice 进行设计、仿真、分析。

- **SPICEBridge / 其他 MCP**: 把设计方程求解与 SPICE 分离，AI 负责拓扑与编排，仿真器负责物理。

- **Anthropic 官方**: Claude 可完成从电路设计到原型的全流程（几何布局、制造约束、固件）。

### 实用流程（推荐教学平台使用）
1. 用 Opus 5.5 生成 SPICE netlist 或 PySpice 脚本。
2. 用 ngspice / LTspice 运行仿真，导出波形数据。
3. 把波形图、参数、原理图嵌入平台页面。
4. 学生可调参数后触盖新结果，或与真实仪器数据对比。

## 3. 大学教学推荐组合

- 入门：Falstad CircuitJS + PhET Circuit Construction Kit
- 中级：Qucs-S 或 KiCad 仿真
- 高级 / 研究：ngspice + Python 后处理，或 LTspice + 厂商模型
- AI 助手：用 Opus 5.5 生成典型电路并自动验证，学生可修改参数再仿真

更新时间：2026-11-18
