---
title: "AI Research Briefing 2026-05-19"
date: 2026-05-19
layout: default
---

# AI Research Briefing - 2026-05-19

## 🔬 Top 论文精选

### 1🌟 Code as Agent Harness
- **机构**: 综述
- **作者**: Xuying Ning, Katherine Tieu, Dongqi Fu, Tianxin Wei, Zihao Li 等
- **arXiv**: [2605.18747](https://arxiv.org/abs/2605.18747)
- **代码**: 暂无
- **分类**: cs.CL, cs.AI
- **核心创新**: 提出代码即 Agent 线索（Code as Agent Harness）的统一视角，系统梳理代码作为 Agent 推理、行动、环境建模和执行验证的运行基座。从接口层（harness interface）、机制层（规划/记忆/工具使用/反馈控制）到多 Agent 扩展三层展开，为 Agent 基础设施化提供理论框架。

### 2🌟 General Preference Reinforcement Learning
- **机构**: 综述
- **作者**: Muhammad Umer, Muhammad Ahmed Mohsin, Ahsan Bilal, Arslan Chaudhry, Andreas Haupt
- **arXiv**: [2605.18721](https://arxiv.org/abs/2605.18721)
- **代码**: 暂无
- **分类**: cs.LG, cs.CL
- **核心创新**: 提出 GPRL 框架，利用广义偏好模型（GPM）将偏好嵌入 k 个斜对称子空间，解决标量奖励模型在开放式任务中的信息损失问题。通过逐维度群组相对优势计算和上下文依赖特征值聚合，统一在线 RL 探索与偏好优化，实现开放式文本质量对齐。

### 3🌟 DashAttention: Differentiable and Adaptive Sparse Hierarchical Attention
- **机构**: 未知机构
- **作者**: Yuxiang Huang, Nuno M. T. Gonçalves, Federico Alvetreti, Lei Li, Xu Han
- **arXiv**: [2605.18753](https://arxiv.org/abs/2605.18753)
- **代码**: 暂无
- **分类**: cs.CL
- **核心创新**: 用自适应稀疏 α-entmax 变换替代固定 top-k 块选择，使分层注意力的稀疏-密集阶段完全可微分。证明 DashAttention 具有非扩散性（non-dispersive），在 75% 稀疏度下达到全注意力精度，高稀疏区间优于 NSA 和 InfLLMv2。

### 4🌟 Dexora: Open-source VLA for High-DoF Bimanual Dexterity
- **机构**: 未知机构
- **作者**: Zongzheng Zhang, Jingrui Pang, Zhuo Yang, Kun Li, Minwen Liao 等
- **arXiv**: [2605.18722](https://arxiv.org/abs/2605.18722)
- **代码**: 暂无
- **分类**: cs.RO
- **核心创新**: 首个开源双臂双手高自由度 VLA 系统，设计混合遥操作管线（外骨骼背包+Apple Vision Pro 无标记手势追踪）。构建 100K 仿真 + 10K 真实数据集，提出数据质量感知训练配方（离线判别器+扩散 Transformer 策略训练）。

### 5🌟 LongLive-2.0: An NVFP4 Parallel Infrastructure for Long Video Generation
- **机构**: 未知机构
- **作者**: Yukang Chen, Luozhou Wang, Wei Huang, Shuai Yang, Bohan Zhang 等
- **arXiv**: [2605.18739](https://arxiv.org/abs/2605.18739)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 基于 NVFP4 精度的长视频生成全流程并行基础设施，提出 Balanced SP 序列并行自回归训练，在 Blackwell GPU 上实现 W4A4 NVFP4 推理。无需 ODE 初始化和 DMD 蒸馏，直接将扩散模型调优为长程 AR 扩散模型，可进一步用 LoRA 实时生成（4→2 步）。

### 6🌟 Aurora: Unified Video Editing with a Tool-Using Agent
- **机构**: 未知机构
- **作者**: Yongsheng Yu, Ziyun Zeng, Zhiyuan Xiao, Zhenghong Zhou, Hang Hua 等
- **arXiv**: [2605.18748](https://arxiv.org/abs/2605.18748)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 用工具增强的 VLM Agent 统一视频编辑——Agent 将原始用户请求映射为结构化编辑计划，解析文本/视觉欠指定问题后再交给扩散 Transformer 生成。引入 AgentEdit-Bench 评测基准，实验表明 Agent 增强显著优于纯模型方案。

### 7🌟 ESI-Bench: Towards Embodied Spatial Intelligence that Closes the Perception-Action Loop
- **机构**: Stanford (Leonidas Guibas)
- **作者**: Yining Hong, Jiageng Liu, Han Yin, Manling Li, Leonidas Guibas
- **arXiv**: [2605.18746](https://arxiv.org/abs/2605.18746)
- **代码**: 暂无
- **分类**: cs.CV, cs.AI, cs.CL
- **核心创新**: 基于 Spelke 核心知识理论构建具身空间智能基准，涵盖 10 类任务 29 子类，要求 Agent 主动选择感知/运动/操控能力序列来积累任务相关证据。发现主动探索大幅优于被动观察，随机多视角反而增加噪声。

### 8🌟 Predictable Confabulations: Factual Recall by LLMs Scales with Model Size and Topic Frequency
- **机构**: 未知机构
- **作者**: Matthew L. Smith, Jonathan P. Shock, Samuel T. Segun, Iyiola E. Olatunji, Tegawendé F. Bissyandé
- **arXiv**: [2605.18732](https://arxiv.org/abs/2605.18732)
- **代码**: 暂无
- **分类**: cs.CL, cs.AI, cs.LG
- **核心创新**: 在 38 个模型和 8900+ 学术引用上建立事实回忆的 scaling law：回忆质量遵循参数量×主题频率对数线性组合的 sigmoid 函数，仅两个变量即可解释 60% 方差（同族内 74-94%）。提出叠加噪声模型——信号强度随概念频率缩放，噪声地板随模型容量缩放。

### 9🌟 SafeDiffusion-R1: Online Reward Steering for Safe Diffusion Post-Training
- **机构**: 未知机构
- **作者**: Komal Kumar, Ankan Deria, Abhishek Basu, Fahad Shamshad, Hisham Cholakkal
- **arXiv**: [2605.18719](https://arxiv.org/abs/2605.18719)
- **代码**: [GitHub](https://github.com/MAXNORM8650/SafeDiffusion-R1.)
- **分类**: cs.CV
- **核心创新**: 利用 CLIP 嵌入空间的内在属性设计 steering reward 机制——将文本表示推向安全方向、远离不安全方向，无需训练专用安全/不安全奖励模型。在线 GRPO 策略学习，避免灾难性遗忘，显著减少不当内容生成。🌟 开源

### 10🌟 SURGE: Approximation-free Training Free Particle Filter for Diffusion Surrogate
- **机构**: 未知机构
- **作者**: Lifu Wei, Yinuo Ren, Naichen Shi, Yiping Lu
- **arXiv**: [2605.18745](https://arxiv.org/abs/2605.18745)
- **代码**: 暂无
- **分类**: stat.ML, cs.LG
- **核心创新**: 基于 Girsanov 测度变换的无梯度推理时间缩放算法，通过路径级重要性重加权替代梯度粒子权重计算。证明路径级 SMC 与粒子级 SMC 的等价性，无需评分函数/Hessian/PDE 评估即可提升生成质量。

### 11🌟 WavFlow: Audio Generation in Waveform Space
- **机构**: 未知机构
- **作者**: Feiyan Zhou, Luyuan Wang, Shoufa Chen, Zhe Wang, Zhiheng Liu 等
- **arXiv**: [2605.18749](https://arxiv.org/abs/2605.18749)
- **代码**: 暂无
- **分类**: cs.SD, cs.CV
- **核心创新**: 挑战 latent space 音频生成范式，直接在原始波形空间通过 flow matching 的 x-prediction 生成高保真音频。波形 patchify 为 2D token 网格+振幅提升对齐信号尺度，利用 500 万视频-文本-音频三元组从零学习声学模式，性能匹配/超越 latent-based 方法。

### 12🌟 Vision-OPD: Learning to See Fine Details for Multimodal LLMs via On-Policy Self-Distillation
- **机构**: CAS (Le Sun)
- **作者**: Qianhao Yuan, Jie Lou, Xing Yu, Hongyu Lin, Le Sun
- **arXiv**: [2605.18740](https://arxiv.org/abs/2605.18740)
- **代码**: 暂无
- **分类**: cs.CV, cs.AI, cs.CL
- **核心创新**: 发现 MLLM 存在区域到全局感知差距（同一模型在裁剪区域上回答细粒度问题比全图更准），提出 Vision-OPD 自蒸馏框架：裁剪条件教师策略→全图条件学生策略，通过 on-policy rollout 的 token 级分布对齐转移区域感知优势，无需外部教师/标注/推理工具。

---

## 🔥 GitHub Trending AI 项目

| # | 项目 | Stars | 描述 |
|---|------|-------|------|
| 1 | [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) | ⭐ 111.1k | LLM inference in C/C++ |
| 2 | [microsoft/ai-agents-for-beginners](https://github.com/microsoft/ai-agents-for-beginners) | ⭐ 63.5k | 12 Lessons to Get Started Building AI Agents |
| 3 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | ⭐ 37.3k | LLM 驱动 A/H/美股智能分析+推送 |
| 4 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | ⭐ 36.8k | CLI-Anything: Making ALL Software Agent-Native |
| 5 | [humanlayer/12-factor-agents](https://github.com/humanlayer/12-factor-agents) | ⭐ 20.7k | LLM-powered 生产级 Agent 设计原则 |
| 6 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | ⭐ 17.7k | Personal AI super intelligence, Rust |
| 7 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | ⭐ 24.5k | Agent Skills for research/science/engineering |
| 8 | [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) | ⭐ 15.4k | Stealth Chromium, passes all bot detection |
| 9 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) | ⭐ 12.1k | Claude Code 学术研究技能链 |
| 10 | [NVlabs/Sana](https://github.com/NVlabs/Sana) | ⭐ 6.6k | Efficient High-Resolution Image Synthesis |

---

## 📊 今日趋势总结

- **Agent 基础设施化**成为共识：Code as Agent Harness 综述将代码定位为 Agent 运行基座，CLI-Anything 将任意软件 Agent 化，12-factor-agents 提出 Agent 生产设计原则
- **RL 对齐创新**：GPRL 用广义偏好模型统一在线 RL 和偏好优化，SafeDiffusion-R1 用 CLIP steering reward 实现扩散模型安全对齐
- **长视频生成**基础设施快速演进：LongLive-2.0 NVFP4 精度在 Blackwell 上实现极致效率
- **Agent 视频编辑**成为新范式：Aurora 用 VLM Agent 统一处理文本/视觉欠指定问题
- **事实回忆 Scaling Law**首次建立：参数量×主题频率双变量 sigmoid 模型解释 60%+ 方差
