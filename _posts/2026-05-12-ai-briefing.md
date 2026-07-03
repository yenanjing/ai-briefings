---
layout: default
title: "AI Research Briefing - 2026-05-12"
date: 2026-05-12T10:00:00+08:00
---

# AI Research Briefing — 2026-05-12

> **在线版**: [https://yenanjing.github.io/ai-briefings/2026/05/12/ai-briefing.html](https://yenanjing.github.io/ai-briefings/2026/05/12/ai-briefing.html)

---

## 📄 精选论文 Top 12

### 1. 9🌟 DeepLog: A Software Framework for Modular Neurosymbolic AI
- **机构**: KULeuven
- **作者**: Robin Manhaeve, Stefano Colamonaco, Vincent Derkinderen, Rik Adriaensen, Lucas Van Praet
- **arXiv**: [2605.10279](https://arxiv.org/abs/2605.10279)
- **代码**: [https://github.com/ML-KULeuven/deeplog](https://github.com/ML-KULeuven/deeplog) 🌟 开源
- **分类**: cs.LG
- **核心创新**: 将多种神经符号语言统一编译为 PyTorch 中的算术电路，作为通用后端支持 LNN、DeepProbLog、NeurASP 等系统的组合。开源框架大幅降低神经符号 AI 的工程门槛，使逻辑推理可作为可组合模块嵌入标准深度学习工作流。

### 2. 8🌟 Follow the Mean: Reference-Guided Flow Matching
- **机构**: Leiden University
- **作者**: Pedro M. P. Curvo, Maksim Zhdanov, Floor Eijkelboom, Jan-Willem van de Meent
- **arXiv**: [2605.10302](https://arxiv.org/abs/2605.10302)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 揭示 Flow Matching 速度场完全由条件端点均值决定，提出通过修改参考集实现训练-free 的可控生成。Reference-Mean Guidance 可在冻结的 FLUX.2-klein (4B) 上实现颜色、身份、风格、结构的精确控制，无需任何参数更新。

### 3. 7🌟 PaMoSplat: Part-Aware Motion-Guided Gaussian Splatting for Dynamic Scene Reconstruction
- **机构**: Zhejiang University
- **作者**: Yinan Deng, Jianyu Dou, Jiahui Wang, Jingyu Zhao, Yi Yang
- **arXiv**: [2605.10307](https://arxiv.org/abs/2605.10307)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 提出部件感知的运动引导 3DGS 框架，通过图聚类将多视图分割掩码提升为 3D 部件，利用差分进化算法从光流估计刚性运动作为优化热启动。在复杂大运动场景中显著提升渲染质量和跟踪精度，并支持 4D 场景编辑等下游应用。

### 4. 7🌟 LeapTS: Rethinking Time Series Forecasting as Adaptive Multi-Horizon Scheduling
- **机构**: Monash University / Wuhan University
- **作者**: Sheng Pan, Ming Jin, Bo Du, Shirui Pan
- **arXiv**: [2605.10292](https://arxiv.org/abs/2605.10292)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 将时序预测重新定义为预测视野上的动态调度过程，通过层级控制器动态选择最优预测尺度和推进长度，配合神经受控微分方程驱动连续时间状态演化。性能提升 ≥7.4% 同时实现 2.6×-5.3× 推理加速。

### 5. 7🌟 AgentRx: A Benchmark Study of LLM Agents for Multimodal Clinical Prediction Tasks
- **机构**: New York University Abu Dhabi
- **作者**: Baraa Al Jorf, Farah E. Shamout
- **arXiv**: [2605.10286](https://arxiv.org/abs/2605.10286)
- **代码**: 暂无
- **分类**: cs.AI
- **核心创新**: 首次系统评估 LLM Agent 在多模态临床风险预测中的表现，使用大规模真实 EHR+影像+报告数据。发现单 Agent 框架优于朴素多 Agent 系统，在多模态数据融合和校准方面更优，揭示了多 Agent 协作在异构输入场景下的关键不足。

### 6. 7🌟 DP-LAC: Lightweight Adaptive Clipping for Differentially Private Federated Fine-tuning of Language Models
- **机构**: Microsoft
- **作者**: Haaris Mehmood, Jie Xu, Karthikeyan Saravanan, Rogier Van Dalen, Mete Ozay
- **arXiv**: [2605.10272](https://arxiv.org/abs/2605.10272)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 提出无需额外超参数调优的差分隐私联邦微调方法，先通过隐私直方图估计初始裁剪阈值，再训练中自适应调整且不消耗隐私预算。平均准确率提升 6.6%，显著降低 DP-SGD 的实用性门槛。

### 7. 6🌟 Active Tabular Augmentation via Policy-Guided Diffusion Inpainting (TAP)
- **机构**: University of Tübingen
- **作者**: Zheyu Zhang, Shuo Yang, Bardh Prenkaj, Gjergji Kasneci
- **arXiv**: [2605.10315](https://arxiv.org/abs/2605.10315)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 形式化生成增强中的「保真度-效用差距」问题，提出 TAP 框架将扩散修复与轻量学习器条件策略耦合。策略引导生成器向高效用区域偏移，显式门控控制注入时机。在 7 个数据集上分类准确率提升最高 15.6%。

### 8. 6🌟 Robust Probabilistic Shielding for Safe Offline Reinforcement Learning
- **机构**: Radboud University
- **作者**: Maris F. L. Galesloot, Thomas Rhemrev, Nils Jansen
- **arXiv**: [2605.10293](https://arxiv.org/abs/2605.10293)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 首次将安全策略改进（SPI）与概率屏蔽（Shielding）整合到离线 RL 中，仅利用可用数据集和安全/不安全状态知识即可保证策略安全性。在低数据场景下显著提升平均和最差情况性能。

### 9. 6🌟 Sample-Mean Anchored Thompson Sampling for Offline-to-Online Learning with Distribution Shift
- **机构**: Microsoft Research
- **作者**: Bochao Li, Yao Fu, Wei Chen, Fang Kong
- **arXiv**: [2605.10289](https://arxiv.org/abs/2605.10289)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 提出 Anchor-TS 算法，通过中位数锚定规则将在线后验样本、混合后验样本与在线样本均值结合，系统性纠正分布偏移引起的偏差。提供理论保证量化偏移程度和离线数据量对遗憾减少的影响。

### 10. 6🌟 BROS: Bias-Corrected Randomized Subspaces for Memory-Efficient Single-Loop Bilevel Optimization
- **机构**: Peking University
- **作者**: Hengrui Zhang, Boao Kong, Engao Zhang, Kun Yuan
- **arXiv**: [2605.10288](https://arxiv.org/abs/2605.10288)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 提出内存高效的单循环随机双层优化方法，在随机子空间中执行下层和辅助更新，通过 Rademacher 双探针校正恢复无偏 Hessian-action 估计。在 ViT 重加权等任务中峰值内存降低达 44.9%。

### 11. 6🌟 PolarVSR: A Unified Framework and Benchmark for Continuous Space-Time Polarization Video Reconstruction
- **机构**: Peking University
- **作者**: Chenggong Li, Yidong Luo, Junchao Zhang, Boxin Shi, Degui Yang
- **arXiv**: [2605.10275](https://arxiv.org/abs/2605.10275)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 首个时空偏振视频重建架构，联合建模空间和时间方向的偏振，使用偏振感知隐式神经表示实现连续高保真上采样。同时建立首个大规模彩色 DoFP 偏振视频基准。

### 12. 6🌟 Positive Alignment: Artificial Intelligence for Human Flourishing
- **机构**: Oxford University
- **作者**: Ruben Laukkonen, Seb Krier, Chloé Bakalar, Shamil Chandaria, Morten Kringelbach
- **arXiv**: [2605.10310](https://arxiv.org/abs/2605.10310)
- **代码**: 暂无
- **分类**: cs.AI
- **核心创新**: 提出「正向对齐」范式，将 AI 对齐从仅关注安全和防伤害扩展到主动促进人类繁荣。类比积极心理学，提出多中心治理、社区定制、持续适应等设计原则，涵盖数据过滤、预训练、评估、Agent 全生命周期等技术方向。

---

## 🔥 GitHub Trending AI 项目

### 1. [NousResearch/hermes-agent](NousResearch/hermes-agent?not_a_link) — ⭐ 2,065/today
- **语言**: Python
- **简介**: The agent that grows with you — 自适应成长的 AI Agent

### 2. [CloakHQ/CloakBrowser](CloakHQ/CloakBrowser?not_a_link) — ⭐ 1,320/today
- **语言**: Python
- **简介**: Stealth Chromium 浏览器，通过源码级指纹修补绕过所有 bot 检测

### 3. [bytedance/UI-TARS-desktop](bytedance/UI-TARS-desktop?not_a_link) — ⭐ 956/today
- **语言**: TypeScript
- **简介**: 开源多模态 AI Agent Stack，连接前沿 AI 模型与 Agent 基础设施

### 4. [decolua/9router](decolua/9router?not_a_link) — ⭐ 941/today
- **语言**: JavaScript
- **简介**: 免费 AI 编程路由，连接 Claude Code/Codex/Cursor 到 40+ Provider

### 5. [datawhalechina/easy-vibe](datawhalechina/easy-vibe?not_a_link) — ⭐ 812/today
- **语言**: JavaScript
- **简介**: vibe coding 2026 — 面向初学者的现代编程入门课程

### 6. [playcanvas/supersplat](playcanvas/supersplat?not_a_link) — ⭐ 531/today
- **语言**: TypeScript
- **简介**: 3D Gaussian Splat Editor — 3D 高斯泼溅编辑器

### 7. [rohitg00/agentmemory](rohitg00/agentmemory?not_a_link) — ⭐ 430/today
- **语言**: TypeScript
- **简介**: #1 AI 编程 Agent 持久化记忆方案（基于真实基准测试）

### 8. [Lordog/dive-into-llms](Lordog/dive-into-llms?not_a_link) — ⭐ 422/today
- **语言**: Jupyter Notebook
- **简介**: 《动手学大模型》系列编程实践教程

### 9. [tinyhumansai/openhuman](tinyhumansai/openhuman?not_a_link) — ⭐ 366/today
- **语言**: Rust
- **简介**: 个人 AI 超级智能，Rust 实现的私有化方案

### 10. [rasbt/LLMs-from-scratch](rasbt/LLMs-from-scratch?not_a_link) — ⭐ 337/today
- **语言**: Python
- **简介**: 从零构建大语言模型（ Sebastian Raschka 著）

---

*Generated on 2026-05-12 by AI Research Briefing Automation*
