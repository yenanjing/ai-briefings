---
layout: default
title: "AI Research Briefing - 2026-06-15"
date: 2026-06-15
---

# AI 研究简报 - 2026-06-15（周一）

## 论文精选（12 篇）

### 8.0🌟 Gaze Heads: How VLMs Look at What They Describe
- **作者**: Rohit Gandikota; David Bau
- **arXiv**: [2606.14703v1](https://arxiv.org/abs/2606.14703v1)
- **分类**: cs.CV, cs.AI
- **核心创新**: 发现 VLM 中存在"注视头"（Gaze Heads）——语言模型骨干中的少量注意力头，其注意力追踪模型正在描述的图像区域。使用漫画条作为受控测试床，通过简单相关性分数定位这些头。揭示了 VLM 内部视觉-语言关联的神经机制。

### 7.9🌟 ClinHallu: A Benchmark for Diagnosing Stage-Wise Hallucinations in Medical MLLM Reasoning
- **机构**: 阿里巴巴达摩院（摘要含 github.com/alibaba-damo-academy）
- **作者**: Sicheng Yang; Hangjie Yuan; Wenjun Zhang; Jinwang Wang; Yichen Qian; Weihua Chen
- **arXiv**: [2606.14697v1](https://arxiv.org/abs/2606.14697v1)
- **代码**: [github.com/alibaba-damo-academy/ClinHallu](https://github.com/alibaba-damo-academy/ClinHallu)
- **分类**: cs.CV, cs.AI
- **核心创新**: 首个医疗 MLLM 推理过程中幻觉来源诊断基准。发现幻觉来源因样本而异：视觉误识别、医学知识错误回忆、推理整合缺陷。提供分阶段幻觉定位能力，对临床 AI 安全评估有实用价值。

### 7.8🌟 RATS! Patches Talk Through Registers: Emergent Parts in Register Attention Transformers
- **作者**: Timing Yang; Predrag Neskovic; Jansen Seheult; Wenchao Han; Anand Bhattad; Alan Yuille
- **arXiv**: [2606.14701v1](https://arxiv.org/abs/2606.14701v1)
- **分类**: cs.CV, cs.AI
- **核心创新**: 提出 RATS（Register Attention Transformers），将分类 token 分解为 N 个可学习的寄存器 token，实现 patch 信息的 L→N→N→L 路由。在自监督视觉模型中发现组合部件结构的自发涌现，类似人类识别鸟的头、翅膀、爪子等可复用部件。

### 7.7🌟 RepFusion: Leveraging Multimodal Priors for Denoising in Representation Space
- **作者**: Xichen Pan; Aashu Singh; Satya Narayan Shukla; Xiangjun Fan; Shlok Kumar Mishra; Saining Xie
- **arXiv**: [2606.14700v1](https://arxiv.org/abs/2606.14700v1)
- **分类**: cs.CV, cs.AI
- **核心创新**: 利用表示自编码器（RAE）将生成目标转向语义结构化视觉表示，利用预训练多模态 LLM 的 MLP 投影器进行潜空间去噪。将 LLM 先验从文本编码扩展到扩散模型去噪过程，实现文本到图像生成的质量提升。

### 7.6🌟 OmniVideo-100K: A Dataset for Audio-Visual Reasoning through Structured Scripts and Evidence Chains
- **作者**: Xinyue Cai; Chaoyou Fu; Yi-Fan Zhang; Ran He; Caifeng Shan
- **arXiv**: [2606.14702v1](https://arxiv.org/abs/2606.14702v1)
- **分类**: cs.CV, cs.AI
- **核心创新**: 构建 10 万级音视频推理数据集，引入结构化脚本和证据链。解决现有"视频-字幕-QA"范式中音频-视觉源关联断裂、跨片段描述不一致的问题。为长文本理解与音视频 QA 联合训练提供高质量数据资源。

### 7.5🌟 Instruct-Particulate: Scaling Feed-Forward 3D Object Articulation with Kinematic Control
- **作者**: Ruining Li; Yuxin Yao; Matt Zhou; Chuanxia Zheng; Christian Rupprecht; Joan Lasenby
- **arXiv**: [2606.14699v1](https://arxiv.org/abs/2606.14699v1)
- **分类**: cs.CV, cs.GR
- **核心创新**: 3D 物体关节运动前馈预测模型，输入 3D 网格和目标运动学规范（部件描述、连接性、关节类型），预测可动画结构。解决标注数据稀缺问题，为游戏、动画、机器人仿真提供数据合成工具。

### 7.4🌟 AdaSR: Adaptive Streaming Reasoning with Hierarchical Relative Policy Optimization
- **作者**: Junlong Tong; Wenqi Xu; Yingqi Fan; Anhao Zhao; Xuan Lu; Yang Tan
- **arXiv**: [2606.14694v1](https://arxiv.org/abs/2606.14694v1)
- **代码**: [github.com/EIT-NLP/StreamingLLM](https://github.com/EIT-NLP/StreamingLLM)
- **分类**: cs.CL, cs.AI
- **核心创新**: 自适应流式推理框架，使用层级相对策略优化（HRPO）实现"边读边想"。解决传统"先读后想"范式无法处理音频/视频流的局限，在部分观测下持续推理、更新、响应。有开源代码。

### 7.3🌟 CORA: Analyzing and bridging thinking-answer gap in Multimodal RLVR via Consistency-Oriented Reasoning Alignment
- **作者**: Jiayue Cao; Zhicong Lu; Xuehan Sun; Wei Jia; Hongling Zheng; Changyuan Tian
- **arXiv**: [2606.14691v1](https://arxiv.org/abs/2606.14691v1)
- **分类**: cs.CV, cs.AI
- **核心创新**: 针对多模态 RLVR 中推理过程与最终答案的语义不一致问题，提出一致性导向推理对齐（CORA）。深入分析视觉推理中"思考-答案"间隙的成因和解决方案，提升多模态推理的可靠性。

### 7.2🌟 AgentSpec: Understanding Embodied Agent Scaffolds Through Controlled Composition
- **作者**: Jixuan Chen; Jianzhi Shen; Haoqiang Kang; Zhi Hong; Qingyi Jiang; Soham Bose
- **arXiv**: [2606.14674v1](https://arxiv.org/abs/2606.14674v1)
- **分类**: cs.AI, cs.RO
- **核心创新**: 模块化具身 Agent 规范框架，将 Agent 系统分解为推理、记忆、反思、动作执行、学习等组件。通过受控组合实验隔离组件贡献、比较设计替代方案、理解模块交互如何塑造 Agent 行为，提供 Agent 架构设计方法论。

### 7.1🌟 Memento: Reconstruct to Remember for Consistent Long Video Generation
- **作者**: Xuan Wei; Longbin Ji; Guan Wang; Xiangrui Liu; Zhenyu Zhang; Shuohuan Wang
- **arXiv**: [2606.14667v1](https://arxiv.org/abs/2606.14667v1)
- **分类**: cs.CV
- **核心创新**: 长视频生成一致性框架，通过"重建以记忆"机制验证历史记忆是否保留身份关键的主体证据。解决长序列生成中主体被稀释、覆盖或遗忘的问题，提升长视频生成的主体一致性。

### 7.0🌟 Persona-Pruner: Sculpting Lightweight Models for Role-Playing
- **作者**: Jinsu Kim; Jihoon Tack; Noah Lee; Jongheon Jeong
- **arXiv**: [2606.14695v1](https://arxiv.org/abs/2606.14695v1)
- **代码**: [github.com/jsu-kim/Persona-Pruner](https://github.com/jsu-kim/Persona-Pruner)
- **分类**: cs.CL
- **核心创新**: 质疑为单一角色分配完整通用模型的必要性，提出角色扮演模型轻量化方法。针对 NPC 生态系统（大量角色同时交互）的计算效率问题，通过结构化剪枝实现角色模型压缩，有开源代码。

### 6.9🌟 HPSv3++: Scaling Reward Models Across the Full Spectrum of Diffusion Model Capabilities
- **作者**: Yijun Liu; Jie Huang; Zeyue Xue; Yuming Li; Ruizhe He; Haoran Li
- **arXiv**: [2606.14657v1](https://arxiv.org/abs/2606.14657v1)
- **代码**: [github.com/PlantPotatoOnMoon/HPSv3-PlusPlus](https://github.com/PlantPotatoOnMoon/HPSv3-PlusPlus)
- **分类**: cs.CV
- **核心创新**: 扩展 HPSv3 奖励模型框架以适配不同能力水平的扩散模型。解决传统奖励模型仅在早期 T2I 模型标注数据上训练、无法适应模型能力和 RL 迭代带来的质量判别偏移问题，有开源代码。

## GitHub Trending（AI 相关）

| 项目 | Stars | 今日增长 | 描述 |
|------|-------|----------|------|
| NVIDIA/SkillSpector | ~5,431 | - | AI Agent skill 安全扫描器，检测漏洞和恶意模式 |
| shiyu-coder/Kronos | - | - | AI 相关项目 |
| andrewyng/aisuite | - | - | AI 工具集 |
