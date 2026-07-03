---
layout: default
title: "AI Research Briefing - 2026-05-28"
date: 2026-05-28T11:00:00+08:00
---

## 📄 精选论文（12 篇）

### 1🌟 OSP-Next: Efficient High-Quality Video Generation with Sparse Sequence Parallelism, HiF8 Quantization, and Reinforcement Learning
- **机构**: Peking University；Nanyang Technological University, Singapore；Rabbitpre AI
- **作者**: Ge, He, Zhang, Lin, Zhu, Cheng, Yuan
- **arXiv**: [2605.28691](https://arxiv.org/abs/2605.28691)
- **代码**: [GitHub](https://github.com/PKU-YuanGroup/OSP-Next)
- **分类**: cs.CV
- **评分**: 8/10 🌟🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 提出端到端视频生成优化框架，结合稀疏序列并行（减少显存占用）、HiF8 浮点8量化和高保真 RL 奖励微调三大技术，首次在视频生成中实现推理效率与生成质量的双重提升，为大规模视频生成模型的部署提供了可行路径。

### 2🌟 DREAM-R: Multimodal Speculative Reasoning with RL-Based Refined Drafting, Precise Verification, and Fully Parallel Execution
- **机构**: New York University；University of Pennsylvania；Cerebras Systems
- **作者**: Hu, Liu, Yin, Xia, Bao, Sather, Thangarasa, Zhang
- **arXiv**: [2605.28678](https://arxiv.org/abs/2605.28678)
- **代码**: [GitHub](https://github.com/HuYunhai-Alex/DREAM-R)
- **分类**: cs.AI
- **评分**: 7.5/10 🌟🌟🌟🌟🌟🌟🌟⭐
- **核心创新**: 将投机推理（speculative decoding）扩展到多模态推理场景，用 RL 训练草稿模型生成更高质量的推理路径，配合精确验证机制和全并行执行，显著降低多模态推理延迟。投机推理+RL 的组合在多模态领域属首次探索。

### 3🌟 Mechanistically Interpreting the Role of Sample Difficulty in RLVR for LLMs
- **机构**: Beijing Jiaotong University；AntGroup；Northwestern Polytechnical University；University of Leeds；University of Southampton
- **作者**: Cheng, Zhang, Gao, Xing, Wang, Zhu
- **arXiv**: [2605.28388](https://arxiv.org/abs/2605.28388)
- **代码**: 暂无
- **分类**: cs.AI
- **评分**: 7.5/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 从机制可解释性角度分析 RLVR（Reinforcement Learning from Verifier Rewards）中样本难度的影响，揭示了困难样本和简单样本在训练动力学中的不同角色，为 RLVR 数据筛选提供了理论指导。该工作弥合了经验观察与理论理解之间的鸿沟。

### 4🌟 Meta-Attention: Bayesian Per-Token Routing for Efficient Transformer Inference
- **机构**: Knowledge Lab AG
- **作者**: Ferrari
- **arXiv**: [2605.28384](https://arxiv.org/abs/2605.28384)
- **代码**: 暂无
- **分类**: cs.LG
- **评分**: 7/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 提出基于贝叶斯推断的 token 级注意力路由机制，每个 token 动态选择 attending 的 head 子集，实现自适应稀疏注意力。方法无需额外训练开销，在保持全模型精度的同时显著降低推理 FLOPs。

### 5🌟 Agent Explorative Policy Optimization for Multimodal Agentic Reasoning
- **机构**: NVIDIA；KAIST
- **作者**: Kang, Diao, Hachiuma, Hwang, Molchanov, Wang, Lee
- **arXiv**: [2605.28774](https://arxiv.org/abs/2605.28774)
- **代码**: [项目页](https://byungkwanlee.github.io/AXPO-page/)
- **分类**: cs.CL
- **评分**: 7/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 提出 Agent 探索性策略优化（AEPO），专门针对多模态 Agentic 推理场景，通过显式鼓励 Agent 探索多样化的推理路径和工具使用策略来提升复杂任务中的推理质量，而非仅依赖被动反馈。

### 6🌟 CIRF: Tokenizing Chain-of-Thoughts into Reusable Functional Units for Efficient Latent Reasoning in Large Language Models
- **机构**: Boston University；Hankuk University of Foreign Studies
- **作者**: Lee, Shen, Park, Yang, Park
- **arXiv**: [2605.28292](https://arxiv.org/abs/2605.28292)
- **代码**: 暂无
- **分类**: cs.CL
- **评分**: 7/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 将 Chain-of-Thought 推理过程 tokenize 为可复用的「功能单元」，存储在潜在空间中供后续推理复用。类似推理层面的「函数抽象」，避免每次都从头生成完整推理链，显著提升推理效率。

### 7🌟 Gamma-World: Generative Multi-Agent World Modeling Beyond Two Players
- **机构**: NVIDIA；Tsinghua University；University of Toronto；Vector Institute
- **作者**: Liu, He, Shen, Cao, Fidler, Duan, Gao, Gilitschenski et al.
- **arXiv**: [2605.28816](https://arxiv.org/abs/2605.28816)
- **代码**: [项目页](https://research.nvidia.com/labs/sil/projects/gamma-world)
- **分类**: cs.CV
- **评分**: 7/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 将生成式世界模型从传统双人对抗扩展到多 Agent 场景，支持三个以上智能体同时交互建模。通过 Gamma 分布建模多智能体联合动作空间，为多 Agent 规划和仿真提供了新的生成式建模范式。

### 8🌟 LACUNA: Safe Agents as Recursive Program Holes
- **机构**: EPFL
- **作者**: Zhao, Xu, Bračevac, Pham, Wu, Odersky
- **arXiv**: [2605.28617](https://arxiv.org/abs/2605.28617)
- **代码**: 暂无
- **分类**: cs.AI
- **评分**: 7/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 提出将 Agent 安全约束建模为「递归程序洞」（灵感来自编程语言的 staged metaprogramming），Agent 的每步行动都是一个待填充的程序洞，安全检查在编译期而非运行时完成。Odersky（Scala 作者）参与，将 PL 安全理论引入 Agent 安全。

### 9🌟 Thinking as Compression: Your Reasoning Model is Secretly a Context Compressor
- **机构**: Baidu Inc.；Xi’an Jiaotong University；City University of Hong Kong；Queen Mary University of London
- **作者**: Ma, Liu, Li, Liang, Wang, Zhang, Chen, Zhang et al.
- **arXiv**: [2605.28713](https://arxiv.org/abs/2605.28713)
- **代码**: 暂无
- **分类**: cs.AI
- **评分**: 7/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 通过理论和实验证明推理模型（如 o1/o3）的核心能力本质上是上下文压缩：长推理链实际上是在对问题空间进行高效的压缩表示。该发现统一了推理、压缩和信息论三个领域的视角，为理解推理模型的内部机制提供了简洁框架。

### 10🌟 Skill0.5: Joint Skill Internalization and Utilization for Out-of-Distribution Generalization in Agentic Reinforcement Learning
- **机构**: East China Normal University；Meituan Longcat Team
- **作者**: Zhu, Yu, Zhao, Han, Gu, Cai, Li, Qian
- **arXiv**: [2605.28424](https://arxiv.org/abs/2605.28424)
- **代码**: [GitHub](https://github.com/JasonZhujp/Skill0_5)
- **分类**: cs.CL
- **评分**: 7/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 提出技能「半内化」机制（Skill0.5），Agent 不是完全将技能固化到策略中（0.0）也不是完全从外部调用（1.0），而是在训练中联合学习技能的内部化和外部调用策略，显著提升 Agent 在分布外任务中的泛化能力。

### 11🌟 Transformers Provably Learn to Internalize Chain-of-Thought
- **机构**: UC Berkeley；Princeton University
- **作者**: Huang, Zhu, Wang, Jiao, Russell, Sojoudi, Mei
- **arXiv**: [2605.28600](https://arxiv.org/abs/2605.28600)
- **代码**: 暂无
- **分类**: cs.LG
- **评分**: 7/10 🌟🌟🌟🌟🌟🌟🌟
- **核心创新**: 首次给出严格数学证明：Transformer 在足够数据下会自动学会将 Chain-of-Thought 推理步骤内化到其隐表示中。Stuart Russell 参与指导，证明使用了 PAC-Bayes 框架，回答了「为什么 CoT 有效」这一核心理论问题。

### 12🌟 Soft-SVeRL: Self-Verified Reinforcement Learning with Soft Rewards
- **机构**: Cohere Labs；Cohere
- **作者**: Dash, Clavier, Dang, Galle, Fadaee, Üstün, Ermis
- **arXiv**: [2605.28561](https://arxiv.org/abs/2605.28561)
- **代码**: 暂无
- **分类**: cs.CL
- **评分**: 6.5/10 🌟🌟🌟🌟🌟🌟⭐
- **核心创新**: 提出将硬验证奖励替换为软概率奖励的 RL 方法，模型不再需要完全正确的验证结果才获得奖励，而是根据部分正确的程度获得梯度信号，使训练更稳定、探索更充分，在数学推理任务上取得显著提升。

---

## 🔥 GitHub Trending AI 项目

| # | 项目 | 描述 | ⭐ Stars | 语言 |
|---|------|------|----------|------|
| 1 | [obra/superpowers](https://github.com/obra/superpowers) | Agent 技能框架与软件开发方法论 | 209,798 | Shell |
| 2 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent 性能优化系统：技能/记忆/安全一体化 | 196,208 | JavaScript |
| 3 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | AI 大模型一键生成高清短视频 | 62,867 | Python |
| 4 | [Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) | 代码转交互式知识图谱，支持 Claude/Codex/Cursor | 40,454 | TypeScript |
| 5 | [shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) | 金融市场语言基础模型 | 26,936 | Python |
| 6 | [p-e-w/heretic](https://github.com/p-e-w/heretic) | LLM 全自动审查移除工具 | 22,078 | Python |
| 7 | [twentyhq/twenty](https://github.com/twentyhq/twenty) | 开源 AI 原生 CRM（Salesforce 替代） | 47,404 | TypeScript |
| 8 | [moeru-ai/airi](https://github.com/moeru-ai/airi) | 自托管 Grok 伴侣，实时语音+Minecraft/异星工厂 | 40,280 | TypeScript |

---

## 📊 今日概览

- **论文总数**: 200 篇候选（cs.AI/LG/CL/CV），精选 12 篇
- **GitHub 项目**: 8 个 AI 相关 Trending 项目
- **热门方向**: Agent 推理与策略优化（AEPO/CIRF/Skill0.5）、RLVR 机制解释、推理模型压缩理论、多 Agent 世界模型、视频生成效率优化
- **亮点**: Thinking as Compression 统一推理与信息论视角、Transformers 内化 CoT 严格证明（Berkeley/Russell）、LACUNA 将 PL 安全理论引入 Agent（EPFL/Odersky）

---

*本文由 AI 自动生成，仅供研究参考。2026-05-28 20:20 已按 PDF 首页校验并补全论文机构/项目链接，同时复核标题与 arXiv 链接映射。*

