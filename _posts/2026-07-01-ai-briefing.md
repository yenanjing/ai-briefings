---
layout: default
title: "AI 研究简报 2026-07-01"
date: 2026-07-01 10:55:00 +0800
---

# AI 研究简报 2026-07-01

> 自动生成于 2026-07-01 10:55 CST
> 论文来源：arXiv API（25 篇候选，精选 12 篇）

---

## 📚 论文精选（12 篇）

### 8.5🌟 SkillComposer: Structured Skill Composition for LLM Agents
- **作者**: Xinyu Zhao, Zhen Tan, Vaishnav Tadiparthi, Nakul Agarwal, Kwonjoon Lee, Ehsan Moradi Pari, Hossein Nourkhiz Mahjoub, Tianlong Chen
- **arXiv**: [2606.32025](https://arxiv.org/abs/2606.32025)
- **分类**: cs.CL
- **核心创新**: 将 LLM Agent 技能组合形式化为结构化联合决策问题（选择哪些技能、多少个、什么顺序），提出 SkillComposer 使用约束自回归解码器一次性预测技能序列。在 GPT-5.2-Codex 和 Gemini-3-Pro-Preview 上实测，相比无技能基线 pass rate 提升 +23.1pp 和 +18.2pp，接近黄金技能检索上界。

### 8.3🌟 AdaJEPA: An Adaptive Latent World Model
- **作者**: Ying Wang, Oumayma Bounou, **Yann LeCun**, Mengye Ren
- **arXiv**: [2606.32026](https://arxiv.org/abs/2606.32026)
- **分类**: cs.LG, cs.AI
- **核心创新**: LeCun 团队提出自适应潜在世界模型 AdaJEPA，在模型预测控制的闭环中进行测试时适应：每次执行动作后用真实状态转换作为自监督信号更新世界模型，仅需一个梯度步即可显著提升规划成功率。解决了世界模型在分布偏移下的失效问题。

### 8.2🌟 Freeform Preference Learning for Robotic Manipulation
- **作者**: Marcel Torne, Anubha Mahajan, Abhijnya Bhat, **Chelsea Finn**
- **arXiv**: [2606.32027](https://arxiv.org/abs/2606.32027)
- **分类**: cs.RO, cs.AI, cs.LG
- **核心创新**: Chelsea Finn 团队提出 FPL，让人类用自然语言定义偏好轴（速度、安全性、精度等），而非二元偏好。学习语言条件奖励模型，多轴偏好提升长周期操作任务性能 38 个百分点。支持测试时策略引导无需重训练。

### 8.0🌟 TRIAGE: Role-Typed Credit Assignment for Agentic Reinforcement Learning
- **作者**: Yuanda Xu, Zhengze Zhou, Hejian Sang, Xiaomin Li, Jiaxin Zhang, Xinchen Du, Zhipeng Wang, Alborz Geramifard
- **arXiv**: [2606.32017](https://arxiv.org/abs/2606.32017)
- **分类**: cs.LG, cs.AI
- **核心创新**: 提出角色化信用分配框架 TRIAGE，为 Agent RL 动作（搜索、点击、编辑等）添加语义角色轴。结构化 judge 将动作分为"决定性进展/有用探索/无进展基础设施/退化"四类，赋予有界过程奖励。在 ALFWorld/Search-QA/WebShop 上均优于 GRPO，减少 10-15% 无用动作。

### 7.8🌟 Reinforcement Learning with Metacognitive Feedback (RLMF)
- **作者**: Gabrielle Kaili-May Liu, Avi Caciularu, Gal Yona, Idan Szpektor, Arman Cohan
- **arXiv**: [2606.32032](https://arxiv.org/abs/2606.32032)
- **分类**: cs.CL, cs.AI
- **核心创新**: 将元认知（自我监控与调节）引入 LLM 训练。RLMF 基于模型自我判断质量优化偏好排序，超越标准 RL 最高 63%。应用于忠实校准（FC）任务，将内在不确定性对齐到自然语言表达。元认知数据选择比朴素主动学习更高效。

### 7.6🌟 QVal: Evaluating Dense Supervision Signals for Long-Horizon LLM Agents
- **作者**: Sergio Hernández-Gutiérrez, Matteo Merler, Ilze Amanda Auzina, Joschka Strüber, Ameya Prabhu, Matthias Bethge
- **arXiv**: [2606.32034](https://arxiv.org/abs/2606.32034)
- **分类**: cs.LG, cs.AI, cs.CL
- **核心创新**: 提出无训练测试床 QVal，直接评估密集监督信号质量——给定状态-动作对，衡量评分是否与强参考策略的 Q 值对齐。基准覆盖 21 种方法、4 个环境、7 个方法族、6 个开源模型，共 1200+ 评估实验。发现简单 prompting 基线常优于文献中的复杂方法，性能按方法族聚类。

### 7.5🌟 DVG-WM: Disentangled Video Generation for Embodied World Model
- **作者**: Ziyu Shan, Zhenyu Wu, Xiaofeng Wang, Zheng Zhu, Ziwei Wang
- **arXiv**: [2606.32028](https://arxiv.org/abs/2606.32028)
- **分类**: cs.RO
- **核心创新**: 解决视频世界模型的"纠缠"困境：动态建模需要低级时序推理，高分辨率合成需要高级语义。DVG-WM 显式解耦为动力学学习和视觉合成两阶段，使用 Flow Matching 映射动力学到视频潜在空间，加速 3.97×，同时保留接触丰富的细节。

### 7.4🌟 SpheRoPE: Zero-Shot Optimization-Free 360 Panorama Generation
- **作者**: Or Hirschorn, Aaron Olender, Eli Alshan, Ianir Ideses, Lior Fritz, Sagie Benaim
- **arXiv**: [2606.32033](https://arxiv.org/abs/2606.32033)
- **代码**: [项目页](https://orhir.github.io/SpheRoPE)
- **分类**: cs.CV
- **核心创新**: 零样本无训练无优化的 360 全景生成框架。Spherical RoPE 替换标准 RoPE：低频通道用 3D 笛卡尔坐标编码球面流形，高频通道用谐波量化强制精确周期性。配合语义畸变 CFG 显式引导几何，直接继承 Flux.1/Flux.2/LTX-Video 全部创意能力。

### 7.3🌟 Introspective Coupling: Self-Explanation Training Tracks Behavioral Change
- **作者**: Zifan Carl Guo, Laura Ruis, **Jacob Andreas**, Belinda Z. Li
- **arXiv**: [2606.32038](https://arxiv.org/abs/2606.32038)
- **分类**: cs.CL, cs.AI, cs.LG
- **核心创新**: 研究 LLM 训练生成解释时的自省耦合现象：使用早期 checkpoint 或行为相似模型的固定反事实解释训练，模型仍能产生比训练目标更忠实于自身行为的解释。揭示解释训练与行为漂移间的隐式追踪机制，为可扩展的后训练自省信号提供理论基础。

### 7.2🌟 CoMet: Context and Multiplicity Decomposition for Multimodal Uncertainty
- **作者**: Sanghyuk Chun, William Yang, Amaya Dharmasiri, Jisoo Kim, Youngjune Gwon, Hamed Zamani, Gunhee Kim, Guni Sharon, **Saining Xie**, Jiajun Wu, Yilin Shen, Yoav Goldberg
- **arXiv**: [2606.32012](https://arxiv.org/abs/2606.32012)
- **代码**: [GitHub](https://github.com/princetonvisualai/comet_uncertainty)
- **分类**: cs.CV
- **核心创新**: 普林斯顿视觉组提出多模态不确定性分解框架 CoMet，将不确定性分解为上下文和多重性两个维度。在视觉推理、多模态 QA 等任务上提供更细粒度的不确定性估计。开源实现。

### 7.1🌟 AxDafny: Agentic Verified Code Generation in Dafny
- **作者**: Benjamin Breen, Austin Letson, Borja Requena Pozo, Leopoldo Sarra
- **arXiv**: [2606.32007](https://arxiv.org/abs/2606.32007)
- **分类**: cs.AI
- **核心创新**: 研究 Agentic 代码生成在 Dafny 形式化验证中的应用。AxDafny 是验证器引导的修复框架，迭代生成实现、不变量、断言和终止参数。在 DafnyBench 上达到 92.7% 验证成功率，超过此前最强 proof-hint 基线 6.5 个百分点。验证成功与运行时测试衡量不同方面。

### 7.0🌟 Surrogate Fidelity: When Can Open LLMs Explain Closed Ones?
- **作者**: Philippe Chlenski, Zachariah Carmichael, Ayush Warikoo, Chia-Tse Shao, Yingxiao Ye, Aobo Yang, Vivek Miglani, Nehal Bandi
- **arXiv**: [2606.32008](https://arxiv.org/abs/2606.32008)
- **代码**: [GitHub facebookresearch/surrogate](https://github.com/facebookresearch/surrogate)
- **分类**: cs.LG
- **核心创新**: Facebook Research 评估开放 LLM 作为闭源 LLM 的代理保真度。在预测/归因/表示三个层面评估，覆盖 Llama/Qwen/GPT/Gemini 四个家族 11 个模型。发现预测保真度大幅高估归因保真度：预测一致的模型常对因果归因持不同意见。提出 access-validity inversion 现象。开源。

---

## 🐙 GitHub Trending（AI 相关，按今日新增 Star 排序）

| # | 项目 | 总 ⭐ | 今日 ⭐ | 描述 |
|---|------|------|---------|------|
| 1 | msitarzewski/agency-agents | 121,085 | 1,791 | 完整 AI 代理机构：前端、社区运营、创意注入、现实检验 |
| 2 | obra/superpowers | 242,624 | 890 | Agent Skills 框架 & 软件开发方法论 |
| 3 | xbtlin/ai-berkshire | 7,600 | 969 | AI 时代伯克希尔：Claude/Codex 价值投资框架 |
| 4 | diegosouzapw/OmniRoute | 8,643 | 387 | 免费 AI 网关：231+ 提供商，Claude/GPT/Gemini 一键接入 |
| 5 | usestrix/strix | 28,220 | 515 | 开源 AI 渗透测试工具 |
| 6 | ogulcancelik/herdr | 9,063 | 486 | 终端内 Agent 多路复用器 |
| 7 | altic-dev/FluidVoice | 4,967 | 588 | macOS 本地 STT + 自定义 AI 增强模型 |
| 8 | HKUDS/Vibe-Trading | 15,851 | 721 | 个人交易 Agent |

---

## 📊 统计

- **论文候选**: 25 篇（arXiv API submittedDate 降序）
- **精选论文**: 12 篇
- **GitHub AI 项目**: 8 个
- **在线简报**: [https://yenanjing.github.io/ai-briefings/2026/07/01/ai-briefing.html](https://yenanjing.github.io/ai-briefings/2026/07/01/ai-briefing.html)
