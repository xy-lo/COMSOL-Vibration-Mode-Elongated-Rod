# 基于COMSOL的细长杆弯曲振动App开发  
**Application Design for Elongated Thin Rod Bending Vibration Analysis**

---

## 📘 项目简介 | Project Overview

本项目基于 **COMSOL Multiphysics** 平台开发了一款用于分析**细长杆弯曲振动**的 **交互式仿真App**，旨在提升物理实验教学效果并服务于工程结构振动分析。

This project develops an **interactive simulation App** based on **COMSOL Multiphysics** to analyze the flexural vibration behavior of slender beams. It aims to enhance teaching efficiency and serve structural vibration analysis in engineering.

---

## 🎯 研究目的 | Objectives

- 辅助学生理解动态法测杨氏模量实验的振动特性；
- 提供一款集建模、仿真与动画演示于一体的教学工具；
- 拓展至非均匀（变截面）结构的振动模态分析。

---

## ⚙️ 主要功能 | Key Features

| 中文功能描述                     | English Description                          |
|------------------------------|---------------------------------------------|
| 参数化建模：支持等/变截面结构         | Parametric modeling of uniform/variable beams |
| 模态仿真：计算前6阶固有频率与振型     | Modal analysis of the first six natural modes |
| 谐响应分析：考虑瑞利阻尼与强迫振动     | Harmonic response with Rayleigh damping      |
| 节点定位与模态动画展示               | Node detection and animated mode shapes     |
| 与理论结果误差对比分析               | Comparison with analytical solutions        |
| 一键打包为独立App                   | One-click deployment as standalone App      |

---

## 📸 结果展示 | Simulation Results

### 🎬 模态动画示例 | Mode Shape Animation

> 模态1~3展示（建议插入动态图或截图）  
> Mode 1~3 animation (suggest insert gif or screenshots)

![模态动画示意图](./figures/mode_shapes.png)

---

### 📊 频率结果对比 | Frequency Comparison

> 理论值 vs COMSOL仿真值  
> Analytical vs COMSOL simulation results

| 模态序号 | 理论频率 (Hz) | COMSOL仿真频率 (Hz) | 相对误差 (%) |
|--------|---------------|---------------------|--------------|
| 1      | 138.49        | 139.78              | 0.93%        |
| 2      | 867.72        | 881.22              | 1.55%        |
| 3      | 2432.97       | 2507.93             | 3.08%        |

---

### 🧱 变截面建模 | Variable Section Beam

> 自定义函数实现变截面结构几何建模  
> Custom function-based geometry generation

![变截面建模图](./figures/variable_section.png)

---

## 🖥️ 技术实现 | Technical Details

- 软件平台：COMSOL Multiphysics + COMSOL App Builder  
- 建模理论：Euler-Bernoulli梁理论 + 瑞利阻尼  
- 主要模块：固体力学、频域研究、模态分析、结果后处理  
- App界面：自定义输入面板、图形展示窗口、结果导出按钮

---

## 💡 应用前景 | Applications

- 🎓 教学：大学物理、结构动力学、材料力学等课程演示与探究  
- 🏗️ 工程：高层结构、机械振动、天线塔、桥梁模态分析  
- 🔬 研究：多物理场耦合仿真、变截面非线性振动等拓展应用

---

## 🏆 项目成果 | Achievements

- ✅ 成功开发COMSOL App，交互友好、功能完整；
- ✅ 实现从几何建模到振动分析的自动化流程；
- ✅ 控制仿真误差在5%以内，具有较高准确性；
- ✅ 获批山东省大学生创新创业训练计划立项（编号：S202410425036）；
- ✅ 项目文档与App已提交课程论文及开源仓库。

---

## 🙏 致谢 | Acknowledgements

感谢指导教师在模型建立、仿真分析和功能拓展上的全程指导。感谢项目组成员的通力合作与不懈努力，使本项目得以顺利完成。

We sincerely thank our supervisor for the guidance in modeling, simulation, and application development. Also thanks to all team members for their contributions and collaboration.

---

📁 **项目文件结构建议** | Project Folder Structure:

```
├── README.md
├── figures/
│   ├── mode_shapes.png
│   ├── variable_section.png
├── App/
│   └── BeamVibrationApp.mph
├── doc/
│   └── Project_Report.pdf
```
