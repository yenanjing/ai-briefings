---
title: "AI Research Briefing 2026-07-03"
date: 2026-07-03
tags:
  - AI
  - research
  - briefing
  - daily
pages_url: https://yenanjing.github.io/ai-briefings/2026/07/03/ai-briefing.html
---

# AI 研究简报 2026-07-03

> 在线版：https://yenanjing.github.io/ai-briefings/2026/07/03/ai-briefing.html

---

## 📚 今日精选论文（12 篇）

### 10🌟 WorldDirector: Building Controllable World Simulators with Persistent Dynamic Memory
- **作者**: Hanlin Wang, Hao Ouyang, Qiuyu Wang, Wen Wang, Qingyan Bai, Ka Leong Cheng, Yixuan Li, Yihao Meng, Zichen Liu, Yanhong Zeng, Yujun Shen, Qifeng Chen
- **arXiv**: [2607.02517](https://arxiv.org/abs/2607.02517)
- **代码**: [https://worlddirector.github.io/](https://worlddirector.github.io/)
- **分类**: cs.CV
- **核心创新**: 解耦语义动作编排与视觉生成，通过 LLM 协调 3D 轨迹与相机运动，实现持久化动态物体记忆的世界模型。支持物体长时间离开视野后重新出现时保持精确视觉身份。方法新颖，开源项目页。

---

### 9🌟 PointDiT: Pixel-Space Diffusion for Monocular Geometry Estimation
- **作者**: Haofei Xu, Rundi Wu, Philipp Henzler, Nikolai Kalischek, Michael Oechsle, Fabian Manhardt, Marc Pollefeys, Andreas Geiger, Federico Tombari, Michael Niemeyer
- **arXiv**: [2607.02515](https://arxiv.org/abs/2607.02515)
- **代码**: [https://haofeixu.github.io/pointdit/](https://haofeixu.github.io/pointdit/)
- **分类**: cs.CV
- **核心创新**: ICML 2026。极简像素空间扩散 Transformer，基于 ViT 直接处理原始 3D 点图 patch，无需潜在空间压缩和 tokenizer。在不透明物体等模糊区域更鲁棒，超越复杂潜在扩散模型。

---

### 9🌟 LACUNA: A Testbed for Evaluating Localization Precision for LLM Unlearning
- **作者**: Matteo Boglioni, Thibault Rousset, Siva Reddy, Marius Mosbach, Verna Dankers
- **arXiv**: [2607.02513](https://arxiv.org/abs/2607.02513)
- **分类**: cs.CL
- **核心创新**: 首个参数级定位精度的遗忘评估基准。注入合成 PII 到预定义参数，发现现有 SOTA 遗忘方法定位不精确且易受 resurfacing 攻击。当定位成功时，简单梯度方法也能实现强遗忘。Siva Reddy 参与。

---

### 8.5🌟 Program-as-Weights (PAW): A Programming Paradigm for Fuzzy Functions
- **作者**: Wentao Zhang, Liliana Hotsko, Woojeong Kim, Pengyu Nie, Stuart Shieber, Yuntian Deng
- **arXiv**: [2607.02512](https://arxiv.org/abs/2607.02512)
- **分类**: cs.LG
- **核心创新**: 将 LLM 从"每次调用解决问题"转变为"工具构建者"。4B 编译器将自然语言规格编译为神经 artifact，0.6B Qwen3 解释器匹配 Qwen3-32B 性能，仅用 1/50 推理内存，30 tokens/s (MacBook M3)。发布 FuzzyBench 10M 数据集。

---

### 8.5🌟 NEvo: Neural-Guided Evolutionary Video Synthesis for Dynamic Visual Selectivity
- **作者**: Yingtian Tang, Sogand Salehi, Ming Zhou, Amir Zamir, Leyla Isik, Martin Schrimpf
- **arXiv**: [2607.02317](https://arxiv.org/abs/2607.02317)
- **分类**: cs.CV
- **核心创新**: 神经引导视频合成框架，通过动态编码模型预测视频输入的体素级响应，在结构化 prompt 空间中进化搜索。发现大脑已知的选择性模式，揭示侧向流中社会-动态特征的渐进复杂化。in silico 脑科学研究。

---

### 8🌟 Align4D: Alignment Is All You Need For X-to-4D Generation
- **作者**: Qiaowei Miao, Kehan Li, Yawei Luo, Yi Yang
- **arXiv**: [2607.02516](https://arxiv.org/abs/2607.02516)
- **代码**: [https://miaoqiaowei.github.io/Align4D/](https://miaoqiaowei.github.io/Align4D/)
- **分类**: cs.CV
- **核心创新**: 灵活的多模态输入到 4D 生成框架。三大技术：物体距离对齐（VAOD/MAOD）、运动-几何联合对齐、异步优化。提出 X4D 数据集整合 prompt/image/video/3D 数据，在 X4D 和 Consistent4D 上达到 SOTA。

---

### 8🌟 InvSplat: Inverse Feed-Forward Scene Splatting
- **作者**: Polina Karpikova, Wenjing Bian, Haofei Xu, Hendrik Lensch, Andreas Geiger
- **arXiv**: [2607.02301](https://arxiv.org/abs/2607.02301)
- **代码**: [https://poliik.github.io/invsplat/](https://poliik.github.io/invsplat/)
- **分类**: cs.CV
- **核心创新**: 前馈多视图重建的逆渲染框架，直接预测结构化 3D Gaussian 表示（含内在材质属性：albedo/metallic/roughness）。单次前向传播联合预测几何和反射率，支持物理基础重光照和视角相关效果建模。

---

### 7.5🌟 VICIS: Visual Concept Inference from Sets
- **作者**: Nick Stracke, Kolja Bauer, Stefan Andreas Baumann, Miguel Angel Bautista, Josh Susskind, Björn Ommer
- **arXiv**: [2607.02402](https://arxiv.org/abs/2607.02402)
- **代码**: [https://github.com/CompVis/set-learner](https://github.com/CompVis/set-learner)
- **分类**: cs.CV
- **核心创新**: 提出 VICIS 任务：从图像集合推断共享视觉概念并应用到新输入。发现 SOTA VLM 在此任务上表现差，常忽略视觉上下文。训练框架学习从图像集合推断概念并提取概念特定嵌入，支持草图等模态泛化。

---

### 7.5🌟 CheckRLM: Effective Knowledge-Thought Coherence Checking in RAG Reasoning
- **作者**: Dingling Xu, Ruobing Wang, Qingfei Zhao, Yukun Yan, Zhichun Wang, Daren Zha, Shi Yu, Zhenghao Liu, Shuo Wang, Xu Han, Maosong Sun
- **arXiv**: [2607.02262](https://arxiv.org/abs/2607.02262)
- **代码**: [https://github.com/AI9Stars/CheckRLM](https://github.com/AI9Stars/CheckRLM)
- **分类**: cs.CL
- **核心创新**: ACL 2026。RAG 增强推理框架，从推理链提取事实声明，在推理过程中及时检测和纠正知识不一致。最小代价精确修正，显著降低长链推理中的错误累积，开源代码和数据。

---

### 7🌟 PanoSeeker: Active Panoramic Referring Segmentation
- **作者**: Song Tang, Shuming Hu, Xincheng Shuai, Henghui Ding, Yu-Gang Jiang
- **arXiv**: [2607.02497](https://arxiv.org/abs/2607.02497)
- **代码**: [https://henghuiding.com/APRS/](https://henghuiding.com/APRS/)
- **分类**: cs.CV
- **核心创新**: ECCV 2026。360° 全景主动感知分割新任务。记忆增强 Agent 结合 VLM 与 EgoSphere 空间视觉记忆，主动调整视角探索环境。RL 后训练优化搜索效率，新建 APRS 基准。

---

### 7🌟 Distributed Attacks in Persistent-State AI Control
- **作者**: Josh Hills, Ida Caspary, Asa Cooper Stickland
- **arXiv**: [2607.02514](https://arxiv.org/abs/2607.02514)
- **分类**: cs.AI
- **核心创新**: 引入 Iterative VibeCoding 安全基准，研究持久化状态 AI 控制中的分布式攻击。攻击者可通过多 PR 分布式注入，单个监控器无法同时防御渐进和非渐进攻击。状态链接追踪器 + 4 监控集成将渐进攻击逃避率从 93% 降至 47%。

---

### 6.5🌟 Scaling Laws for LLM Social Simulation
- **作者**: Caleb Ziems, William Held, Su Doga Karaca, David Grusky, Tatsunori Hashimoto, Diyi Yang
- **arXiv**: [2607.02464](https://arxiv.org/abs/2607.02464)
- **分类**: cs.CL
- **核心创新**: 系统研究 LLM 社会模拟的缩放规律。使用 85 个 Qwen3 模型（10^18-10^20 FLOPs）和 35 个 70B 级开源模型，发现意见/行为模拟缩放良好，但纵向预测和代表性不足群体缩放慢。行为校准（风险厌恶等认知偏差）几乎不随规模改善。

---

## 🔥 GitHub Trending（当日新增 Star 排序）

| 排名 | 项目 | 总 ⭐ | 今日 ⭐ | 描述 |
|:---:|:-----|-----:|-------:|:-----|
| 1 | msitarzewski/agency-agents | 125.6k | 3,032 | 完整 AI 机构 Agent 框架 |
| 2 | usestrix/strix | 32.4k | 2,137 | 开源 AI 渗透测试工具 |
| 3 | JuliusBrussee/caveman | 81.2k | 926 | Claude Code 穴居人风格技能 |
| 4 | HKUDS/Vibe-Trading | 17.4k | 939 | 个人交易 Agent |
| 5 | JuliusBrussee/caveman | 81.2k | 926 | Claude Code 穴居人风格技能 |
| 6 | openai/codex-plugin-cc | 22.7k | 352 | Claude Code 中使用 Codex |
| 7 | santifer/career-ops | 57.9k | 372 | AI 求职系统 |
| 8 | obra/superpowers | 244.6k | 897 | Agent 技能框架 |
| 9 | affaan-m/ECC | 225.2k | 486 | Agent 性能优化系统 |
| 10 | browser-use/video-use | 13.9k | 554 | Agent 视频编辑 |

---

*生成时间：2026-07-03 10:55 CST*
