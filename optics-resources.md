# Optics, Photonics & Wave Simulation Resources (大学级)

专门整理光学、波光学、高斯光束、光子学相关的交互仿真与开源工具，适合大学教学与先进仿真教学平台。

## 1. VisuPhy — Interactive Optics & Laser Simulations

- **Website**: https://www.visuphy.org/
- **特点**: 完全浏览器基础，无需安装/账号，开源。
- **主要工具**:
  - BeamBench: 3D 高斯光束传播 + 偏振沙盒（https://github.com/visuphy/BeamBench）
  - Polarization 3D: Jones 矩阵偏振仿真（https://github.com/visuphy/Polarization）
  - Gaussian Beam Propagation (ABCD matrices)
  - Laser Pulse Simulator (超快光学)
  - Diffraction Grating
  - NLSE Solver (非线性光纤)
- 适合激光、偏振、波光学大学课程。

## 2. Photonics Toys

- **GitHub**: https://github.com/rkotynski/photonicstoys
- HTML/JS + Python notebooks 教育演示。
- 覆盖：行波/驻波、干涉、波前、薄透镜、Fresnel zone plates、axicons、偏振等。
- 适合大学波光学课程，支持英文/波兰语。

## 3. 其他高级光学工具

| 工具 | 描述 | 链接 |
|------|------|------|
| optrace | Python 脚本光线追踪 + 3D GUI（TH Köln） | https://github.com/drocheam/optrace |
| OpticsLab | Rust + WebGPU 光学设计工作站（像差分析、优化） | https://github.com/AlexCri5an/optics-lab |
| WaveDudeNext | 2D 波光学仿真（折射、演射、干涉，支持图像导入） | https://github.com/graealex/WaveDudeNext |
| PhotonLab | 浏览器 FDTD 电磁波仿真（Rust/WASM） | https://github.com/SpaceEngineerSS/PhotonLab |
| LightFlow | TensorFlow 光传播仿真（UNC，GPU 加速） | https://github.com/UNC-optics/LightFlow |
| LightPipes / Optics | Jupyter 笔记本物理光学 | https://github.com/opticspy/Optics |
| RayOptics / rayopt | 开源光学设计与光线追踪 | 搜索 GitHub |

## 4. PhET 与经典光学仿真

- PhET Light & Radiation Collection: Bending Light, Geometric Optics, Color Vision 等。
- PhysSandbox Optics: https://physandbox.com/optics （包含许多大学级如 Michelson、Fabry-Pérot、Gaussian Beam、Fourier Optics）

## Opus 5.5 相关光学例子

- Ryan Sael 的 **Interactive Lens Lab**: https://lens.lab.sael.net  
  Opus 5.5 一次生成的交互式镜头实验室（对焦环、玻璃元件移动、焦平面扫描、光圈调整）。成本约 $25，1 小时 26 分钟。
- 更多三维光学解释器可见 Techartist 光学系列及 airsup.ai/lab 中的光学相关机器。

## 建议用法

- 浏览器仿真（VisuPhy、PhET、PhotonLab）可直接嵌入平台。
- Python/Jupyter 仿真可预跑后导出图像/视频/数据。
- 结合 Opus 5.5 生成定制三维交互光学解释器（如镜头实验室、光束传播）。

更新时间：2026-11-18
