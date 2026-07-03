---
layout: default
title: "AI 研究简报 2026-06-22"
date: 2026-06-22
---

# AI 研究简报 — 2026-06-22

## 📄 精选论文（12 篇）

### 1🌟 StylisticBias: A Few Human Visual Cues Drive Most Social Biases in MLLMs

- **作者**: Shaghayegh Kolli, Timo Cavelius, Nafiseh Nikeghbal et al.
- **arXiv**: [2606.20527](https://arxiv.org/abs/2606.20527)
- **代码**: [github.com/timo-cavelius/StylisticBias](https://github.com/timo-cavelius/StylisticBias)
- **分类**: cs.CL, cs.CV
- **核心创新**: 针对多模态大模型（MLLMs）的社会偏见问题，构建了首个属性级偏见基准 StylisticBias，通过 500 张逼真人脸图控制视觉线索，分离身份效应与外貌效应，揭示了少量视觉风格线索即可驱动大部分社会偏见。

### 2🌟 S-Agent: Spatial Tool-Use Elicits Reasoning for Spatial Intelligence

- **作者**: Yalun Dai, Hao Li, Shulin Tian et al.
- **arXiv**: [2606.20515](https://arxiv.org/abs/2606.20515)
- **分类**: cs.CV
- **核心创新**: 针对 VLM 对连续 3D 世界缺乏推理能力的问题，提出 S-Agent，通过空间工具使用来激发空间推理，利用一系列空间 API（测距、遮挡检测等）让模型在交互中建立 3D 理解，显著提升空间智能任务表现。

### 3🌟 HumanScale: Egocentric Human Video Can Outperform Real-Robot Data for Embodied Pretraining

- **作者**: Juncheng Ma, Jianxin Bi, Yufan Deng et al.
- **arXiv**: [2606.20521](https://arxiv.org/abs/2606.20521)
- **分类**: cs.CV
- **核心创新**: 提出人类第一人称视频作为机器人预训练数据的规模化替代方案，证明在大规模预训练场景下，人类视频数据在多样性和覆盖面上优于遥操作机器人数据，为具身基础模型的数据瓶颈提供了新路径。

### 4🌟 Contagion Networks: Evaluator Bias Propagation in Multi-Agent LLM Systems

- **作者**: Zewen Liu
- **arXiv**: [2606.20493](https://arxiv.org/abs/2606.20493)
- **分类**: cs.LG, cs.AI, cs.MA
- **核心创新**: 提出 Contagion Networks 框架，形式化建模多 Agent 系统中 LLM 评估者偏差在网络中的传播机制，分析偏差如何通过评估结果在 Agent 间扩散，对多 Agent 系统的可靠性与公平性有重要意义。

### 5🌟 SSD: Spatially Speculative Decoding Accelerates Autoregressive Image Generation

- **作者**: Shilong Xiang, Zirui Zhang, Lijun Yu et al.
- **arXiv**: [2606.20543](https://arxiv.org/abs/2606.20543)
- **分类**: cs.CV
- **核心创新**: 提出空间猜词解码（SSD），利用图像的 2D 空间局部性并行预测多个相邻 token，显著加速自回归图像生成。相比 1D 序列解码，SSD 在保持生成质量的同时大幅降低推理计算量。

### 6🌟 Fast Human Attention Prediction for Fixation-guided Active Perception in Autonomous Navigation

- **作者**: Fatma Youssef Mohammed, Grzegorz Malczyk, Kostas Alexis
- **arXiv**: [2606.20491](https://arxiv.org/abs/2606.20491)
- **分类**: cs.RO, cs.CV
- **核心创新**: 将人类视觉注意力扫描路径机制引入机器人自主导航，提出快速注意力预测模型以引导主动感知。通过预测人类会关注的区域，让机器人优先处理关键视觉信息，提高导航效率。

### 7🌟 JanusMesh: Fast and Zero-Shot 3D Visual Illusion Generation via Cross-Space Denoising

- **作者**: Siang-Ling Zhang, Huai-Hsun Cheng, Tsung-Ju Yang et al.
- **arXiv**: [2606.20563](https://arxiv.org/abs/2606.20563)
- **分类**: cs.CV
- **核心创新**: 提出零样本、无需训练的 3D 视觉错觉生成框架 JanusMesh，通过跨空间去噪使单一 3D 网格从不同视角呈现完全不同语义。相比现有优化方法速度提升显著，且避免了颜色过饱和和几何不连贯问题。

### 8🌟 TimeProVe: Propose, then Verify for Efficient Long Video Temporal Reasoning

- **作者**: Arkaprava Sinha, Dominick Reilly, Siddharth Krishnan et al.
- **arXiv**: [2606.20561](https://arxiv.org/abs/2606.20561)
- **分类**: cs.CV
- **核心创新**: 提出先提议后验证的混合框架 TimeProVe，用于长达数小时视频的时序推理。先用稀疏方案定位候选证据片段，再针对性验证，相比密集处理 VLM 方案大幅降低计算成本，同时保持高精度。

### 9🌟 How Transparent is DiffusionGemma?

- **作者**: Joshua Engels, Callum McDougall, Bilal Chughtai et al.
- **arXiv**: [2606.20560](https://arxiv.org/abs/2606.20560)
- **分类**: cs.LG, cs.AI
- **核心创新**: 系统研究扩散架构 LLM（DiffusionGemma）的推理透明性。将透明性分解为变量透明度和算法透明度两个维度，分析连续隐空间中的计算过程是否比自回归模型更不透明，为扩散模型的可解释性提供基础分析框架。

### 10🌟 UNIEGO: Proxies as Mediators for Unified Egocentric Video Representation Learning

- **作者**: Wenhao Chi, Arkaprava Sinha, Dominick Reilly et al.
- **arXiv**: [2606.20559](https://arxiv.org/abs/2606.20559)
- **分类**: cs.CV, cs.LG
- **核心创新**: 提出分层多教师蒸馏框架 UNIEGO，解决第一人称视频的多视角、多模态、多基础模型的知识融合问题。通过代理作为中介，从外部视角、其他模态和预训练模型中提取互补知识，仅用第一人称视频即可部署。

### 11🌟 Thinking in Boxes: 3D Editing in Real Images Made Easy

- **作者**: Pradhaan S Bhat, Naveen Chandra R, Rishubh Parihar et al.
- **arXiv**: [2606.20556](https://arxiv.org/abs/2606.20556)
- **分类**: cs.CV
- **核心创新**: 提出以 3D 边界框作为结构化规范进行图像编辑，用户只需指定输入和输出框即可完成大物体运动和相机变换编辑。将编辑转化为良定的几何变换问题，克服了文本/2D 条件对空间变换控制模糊的局限。

### 12🌟 The Token Is a Group Element: On Lie-Algebra Attention over Matrix Lie Groups

- **作者**: Przemyslaw Musialski
- **arXiv**: [2606.20547](https://arxiv.org/abs/2606.20547)
- **分类**: cs.LG, cs.CV, cs.GR, cs.RO, math.DG
- **核心创新**: 提出将注意力 token 建模为矩阵李群元素的新范式，token 本身是李群上的变换无需额外特征负载。Score 由相对位姿的闭式代数范数计算而非学习核，可处理仿射全帧变换群，为计算机视觉和机器人学提供新的注意力机制。

---

## 🔥 GitHub Trending AI 项目（8 个）

1. **[bytedance/deer-flow](https://github.com/bytedance/deer-flow)** — 72,780 stars
   Open-source long-horizon SuperAgent harness that researches, codes, and creates. 字节跳动开源的长周期 SuperAgent 框架，集成沙箱、记忆、工具、子 Agent 和消息网关。

2. **[chopratejas/headroom](https://github.com/chopratejas/headroom)** — 45,181 stars
   Compress tool outputs, logs, files, and RAG chunks before they reach the LLM. 60-95% fewer tokens, same answers.

3. **[mattpocock/skills](https://github.com/mattpocock/skills)** — 140,269 stars
   Skills for Real Engineers. 从 Matt Pocock 的 .claude 目录公开的 AI 技能集合，工程技能的最佳实践模板。

4. **[asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks)** — 44,651 stars
   Extracted system prompts from Claude, ChatGPT, Gemini, Grok, Cursor, Copilot and more. 各大 AI 产品系统提示词提取集合。

5. **[topoteretes/cognee](https://github.com/topoteretes/cognee)** — 18,780 stars
   Open-source AI memory platform for agents with persistent long-term memory across sessions.

6. **[mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills)** — 17,918 stars
   754 structured cybersecurity skills for AI agents mapped to 5 security frameworks.

7. **[DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp)** — 10,665 stars
   High-performance code intelligence MCP server. Indexes codebases into persistent knowledge graph.

8. **[calesthio/OpenMontage](https://github.com/calesthio/OpenMontage)** — 9,522 stars
   World's first open-source, agentic video production system with 12 pipelines, 52 tools, 500+ agent skills.

---

*简报生成于 2026-06-22 14:22 | arXiv 论文来自 2026-06-18 批次（周末无新发布）*
