---
layout: default
title: "AI Research Briefing - 2026-07-02"
date: 2026-07-02 10:55:00 +0800
---

# AI Research Briefing - 2026-07-02

> 论文来源：arXiv API 返回 25 篇候选（2026-07-01 提交），精选 12 篇

## 📚 论文精选

### 8.5🌟 TiRex-2: Generalizing TiRex to Multivariate Data and Streaming
- **作者**: Patrick Podest, Sepp Hochreiter 等（LIT AI Lab / JKU Linz）
- **arXiv**: [2607.01204](https://arxiv.org/abs/2607.01204)
- **分类**: cs.LG
- **核心创新**: 基于 xLSTM 的时序基础模型，将单变量 TiRex 扩展到多变量预测，支持过去和未来协变量。实现 O(1) 上下文复杂度和真正的流式推理，相比 Transformer 的 O(n²) 复杂度有根本性优势。Sepp Hochreiter 参与，理论基础扎实。

### 8.3🌟 World from Motion: Generative Dynamic Gaussian Reconstruction from Monocular Video
- **作者**: Liyuan Zhu, Shengyu Huang, Gordon Wetzstein, Iro Armeni 等（Stanford）
- **arXiv**: [2607.01202](https://arxiv.org/abs/2607.01202)
- **分类**: cs.CV, cs.AI, cs.GR
- **核心创新**: 从单目视频生成可自由渲染的动态 3DGS 表示。通过视频模型条件化密集像素对齐渲染，编码外观、几何和 3D 场景运动。构建多视图视频对齐数据集训练。Gordon Wetzstein 团队持续在 3DGS 领域领先。

### 8.1🌟 AutoMem: Automated Learning of Memory as a Cognitive Skill
- **作者**: Shengguang Wu, Hao Zhu, Serena Yeung-Levy（Stanford）
- **arXiv**: [2607.01224](https://arxiv.org/abs/2607.01224)
- **分类**: cs.AI, cs.CL, cs.MA
- **核心创新**: 将记忆管理视为可训练的认知技能（metamemory）。将文件系统操作提升为与任务动作同级的记忆动作，让模型自己决定如何管理记忆。沿结构和提示两个轴改进，认知科学视角独特。

### 7.9🌟 Is One Layer Enough? Training A Single Transformer Layer Can Match Full-Parameter RL Training
- **作者**: Zijian Zhang, Athanasios Glentis, Hongzhou Lin, Mingyi Hong 等
- **arXiv**: [2607.01232](https://arxiv.org/abs/2607.01232)
- **分类**: cs.LG, cs.CL
- **核心创新**: 系统研究 RL 训练在 Transformer 各层的分布。发现仅训练单层可匹配全参数 RL 收益，挑战"所有层贡献相似"的假设。对高效 RLHF 和模型压缩有重要启示。

### 7.8🌟 Distill to Detect: Exposing Stealth Biases in LLMs through Cartridge Distillation
- **作者**: Shayan Talaei, Amin Karbasi, Azalia Mirhoseini, Amin Saberi（Google Brain / Yale / Stanford）
- **arXiv**: [2607.01208](https://arxiv.org/abs/2607.01208)
- **分类**: cs.CL, cs.AI, cs.LG
- **核心创新**: 利用上下文蒸馏检测 LLM 中隐蔽偏见。模型在无关数据上通过语义无关蒸馏传递偏好，仅在相关主题上暴露偏好。Azalia Mirhoseini（Google Brain）参与，对模型供应链安全有重要价值。

### 7.6🌟 FurnitureVLA: Learning Long-Horizon Bimanual Furniture Assembly with Vision-Language-Action Model
- **作者**: Chenyang Ma, Diego Romeres 等
- **arXiv**: [2607.01212](https://arxiv.org/abs/2607.01212)
- **分类**: cs.RO, cs.AI
- **核心创新**: 首个真实规模双臂家具组装 VLA 研究。开发可扩展仿真管道和 VR 遥操作系统收集高质量真实演示，解决极端长时域双臂组装任务。Diego Romeres 团队在机器人 VLA 领域持续深耕。

### 7.5🌟 Perceive-to-Reason: Decoupling Perception and Reasoning for Fine-Grained Visual Reasoning
- **作者**: Hongxing Li, Weiming Lu, Jun Xiao, Yueting Zhuang, Yongliang Shen 等
- **arXiv**: [2607.01191](https://arxiv.org/abs/2607.01191)
- **分类**: cs.CV
- **核心创新**: 将细粒度视觉推理公式化为两阶段过程：感知阶段定位关键视觉线索，推理阶段基于感知结果推理。解决现有方法重复裁剪但不区分感知与推理的问题。对高分辨率图像中的小目标推理有重要价值。

### 7.4🌟 Right in the Right Way: LM Training with Verifiable Rewards and Human Demonstrations
- **作者**: Mehul Damani, Isha Puri, Idan Shenfeld, Jacob Andreas（MIT）
- **arXiv**: [2607.01181](https://arxiv.org/abs/2607.01181)
- **分类**: cs.LG, cs.AI, cs.CL
- **核心创新**: RLVR 优化仅可客观评分的方面，忽视风格和结构等主观方面，导致多样性崩溃、不自然响应和奖励黑客。提出结合可验证奖励和人类示范的混合训练，保留主观质量。

### 7.3🌟 Theoria: Rewrite-Acceptability Verification over Informal Reasoning States
- **作者**: Ben Slivinski, Michael Saldivar
- **arXiv**: [2607.01223](https://arxiv.org/abs/2607.01223)
- **分类**: cs.AI, cs.CL, cs.LG, cs.LO, cs.SE
- **核心创新**: 形式化验证架构，将候选解答重写为带类型的状态转移序列，每个转移有显式理由。填补形式化证明助手和 LLM 标量判断之间的鸿沟，可审计且透明。

### 7.2🌟 QuasiMoTTo: Quasi-Monte Carlo Test-Time Scaling
- **作者**: Michael Y. Li, Noah D. Goodman, Emily B. Fox（Stanford）
- **arXiv**: [2607.01179](https://arxiv.org/abs/2607.01179)
- **分类**: cs.LG, cs.CL
- **核心创新**: 利用准蒙特卡洛采样减少推理计算浪费。独立并行采样产生冗余解，QMC 生成相关但精确的样本，完全在并行采样设计空间内，不牺牲独立性。

### 7.1🌟 The State-Prediction Separation Hypothesis
- **作者**: Giovanni Monea, Kianté Brantley, Yoav Artzi（Cornell）
- **arXiv**: [2607.01218](https://arxiv.org/abs/2607.01218)
- **分类**: cs.CL, cs.AI, cs.LG
- **核心创新**: 提出状态预测分离假设：将 Transformer 的预测和状态存储两个功能解耦到两个计算流。实验证明分离一致提升语言建模性能。Yoav Artzi 团队持续探索 Transformer 架构创新。

### 7.0🌟 Ink3D: Sculpting 3D Assets with Extremely Complex Textures via Video Generative Models
- **作者**: Yue Han, Chong Li, Fangyun Wei, Yan Lu 等
- **arXiv**: [2607.01222](https://arxiv.org/abs/2607.01222)
- **分类**: cs.CV
- **核心创新**: 利用大规模视频生成模型桥接到 3D 生成，解决复杂纹理参考图像复现难题。视频模型训练数据比 3D 大几个数量级，通过桥接释放其建模复杂视觉模式的能力。

## 🔥 GitHub Trending AI 项目

| 项目 | 总 ⭐ | 今日 ⭐ | 描述 |
|------|-------|---------|------|
| msitarzewski/agency-agents | 123.7k | 2,114 | 完整 AI 代理机构框架 |
| hasaneyldrm/exercises-dataset | 8.5k | 2,470 | 433 个健身动作综合数据集 |
| usestrix/strix | 29.9k | 1,211 | 开源 AI 渗透测试工具 |
| microsoft/AI-For-Beginners | 50.6k | 1,096 | 12 周 AI 入门课程 |
| diegosouzapw/OmniRoute | 9.6k | 1,010 | 免费 AI 网关，231+ 供应商 |
| ogulcancelik/herdr | 9.7k | 609 | 终端代理多路复用器 |
| altic-dev/FluidVoice | 5.5k | 572 | macOS 语音听写应用 |
| HKUDS/Vibe-Trading | 16.6k | 694 | 个人交易代理 |
| browser-use/video-use | 13.3k | 693 | 编程代理编辑视频 |
| 0xNyk/council-of-high-intelligence | 2.7k | 161 | 多 AI 人格多轮讨论决策 |

## 📊 统计

- **论文数**: 12 篇精选（25 篇候选）
- **GitHub 项目**: 10 个
- **数据来源**: arXiv API（2026-07-01 提交）
