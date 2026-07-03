---
layout: default
title: "AI 研究简报 2026-04-24"
date: 2026-04-24
---

# AI 研究简报 2026-04-24

> 共收录 arXiv 论文 **25 篇**，精选评分 **12 篇**，GitHub Trending AI 项目 **10 个**

---

## 精选论文（按评分降序）

### 1🌟 Agentic World Modeling: Foundations, Capabilities, Laws, and Beyond
- **机构**: 未知机构
- **作者**: Meng Chu, Xuan Billy Zhang, Kevin Qinghong Lin, Lingdong Kong, Jize Zhang
- **arXiv**: [2604.22748](https://arxiv.org/abs/2604.22748)
- **代码**: 暂无
- **分类**: cs.AI
- **核心创新**: 提出 "levels × laws" 分类体系，将智能体世界模型能力分为三个层次（L1 预测器、L2 模拟器及更高层次），系统梳理了 Agentic World Modeling 的基础、能力与定律。为跨领域世界模型研究提供了统一的概念框架。

---

### 2🌟 Spend Less, Fit Better: Budget-Efficient Scaling Law Fitting via Active Experiment Selection
- **机构**: 未知机构
- **作者**: Sijie Li, Shanda Li, Haowei Lin, Weiwei Sun, Ameet Talwalkar
- **arXiv**: [2604.22753](https://arxiv.org/abs/2604.22753)
- **代码**: [https://github.com/PlanarG/active-sl](https://github.com/PlanarG/active-sl) 🌟
- **分类**: cs.LG
- **核心创新**: 将 Scaling Law 拟合建模为预算感知的序贯实验设计问题，提出基于不确定性的主动实验选择方法，在预算有限的情况下显著提升外推精度。有效降低百万美元级训练预算规划中的试验成本。

---

### 3🌟 Thinking Without Words: Efficient Latent Reasoning with Abstract Chain-of-Thought
- **机构**: IBM Research
- **作者**: Keshav Ramji, Tahira Naseem, Ramón Fernandez Astudillo
- **arXiv**: [2604.22709](https://arxiv.org/abs/2604.22709)
- **代码**: 暂无
- **分类**: cs.CL
- **核心创新**: 提出 Abstract Chain-of-Thought（ACoT），让语言模型在生成回答前先产生一段来自保留词表的短离散隐式推理序列，兼顾 CoT 的推理能力与更低的推理延迟。

---

### 4🌟 How Do AI Agents Spend Your Money? Analyzing and Predicting Token Consumption in Agentic Coding Tasks
- **机构**: University of Michigan / Salesforce
- **作者**: Longju Bai, Zhemin Huang, Xingyao Wang, Jiao Sun, Rada Mihalcea
- **arXiv**: [2604.22750](https://arxiv.org/abs/2604.22750)
- **代码**: 暂无
- **分类**: cs.CL
- **核心创新**: 首次系统研究 AI Agent 在编码任务中的 Token 消耗模式，分析 8 个前沿 LLM 在 SWE-bench Verified 上的轨迹，并评估模型自身预测 Token 用量的能力。

---

### 5🌟 BERAG: Bayesian Ensemble Retrieval-Augmented Generation for Knowledge-based Visual Question Answering
- **机构**: University of Cambridge
- **作者**: Jinghong Chen, Jingbiao Mei, Guangyu Yang, Bill Byrne
- **arXiv**: [2604.22678](https://arxiv.org/abs/2604.22678)
- **代码**: 暂无
- **分类**: cs.CL
- **核心创新**: 提出 BERAG，用贝叶斯集成替代拼接上下文的传统 RAG，解决"迷失于中间"效应和多模态长文本计算开销问题，在视觉问答任务上实现更好的文档归因与扩展性。

---

### 6🌟 Aligning Dense Retrievers with LLM Utility via Distillation
- **机构**: 未知机构
- **作者**: Rajinder Sandhu, Di Mu, Cheng Chang, Md Shahriar Tasjid, Himanshu Rai
- **arXiv**: [2604.22722](https://arxiv.org/abs/2604.22722)
- **代码**: 暂无
- **分类**: cs.IR
- **核心创新**: 提出 UAE（Utility-Aligned Embeddings）框架，将检索建模为分布匹配，通过蒸馏将 LLM 重排序的 Utility 知识迁移到双编码器，在低延迟下提升 RAG 召回精度。

---

### 7🌟 CRAFT: Clustered Regression for Adaptive Filtering of Training data
- **机构**: 未知机构
- **作者**: Parthasarathi Panda, Asheswari Swain, Subhrakanta Panda
- **arXiv**: [2604.22693](https://arxiv.org/abs/2604.22693)
- **代码**: 暂无
- **分类**: cs.CL
- **核心创新**: 提出 CRAFT，通过 k-means 聚类对训练数据进行双阶段筛选，在海量语料中高效挑选精细调优子集，向量化无关，适用于 Seq2Seq 微调场景。

---

### 8🌟 Can QPP Choose the Right Query Variant? Evaluating Query Variant Selection for RAG Pipelines
- **机构**: University of Waterloo / Google / UC Berkeley
- **作者**: Negar Arabzadeh, Andrew Drozdov, Michael Bendersky, Matei Zaharia
- **arXiv**: [2604.22661](https://arxiv.org/abs/2604.22661)
- **代码**: 暂无
- **分类**: cs.IR
- **核心创新**: 探索将查询性能预测（QPP）用于 RAG 管道的查询变体选择，在不运行完整管道的情况下识别最佳改写版本，降低 RAG 计算成本。

---

### 9🌟 Long-tail Internet photo reconstruction
- **机构**: Cornell University
- **作者**: Yuan Li, Yuanbo Xiangli, Hadar Averbuch-Elor, Noah Snavely, Ruojin Cai
- **arXiv**: [2604.22714](https://arxiv.org/abs/2604.22714)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 针对互联网照片长尾分布问题，通过从稠密重建场景采样稀疏子集模拟稀疏数据监督，推动 3D 基础模型在稀疏、噪声场景中的泛化。

---

### 10🌟 Representational Harms in LLM-Generated Narratives Against Global Majority Nationalities
- **机构**: MIT / Wellesley College
- **作者**: Ilana Nguyen, Harini Suresh, Thema Monroe-White, Evan Shieh
- **arXiv**: [2604.22749](https://arxiv.org/abs/2604.22749)
- **代码**: 暂无
- **分类**: cs.CL
- **核心创新**: 系统研究主流 LLM 如何在叙事性文本中表征全球多数族裔国籍身份，揭示针对非主导社群的代表性危害，为 LLM 公平性评估提供实证数据。

---

### 11🌟 Rethinking XAI Evaluation: A Human-Centered Audit of Shapley Benchmarks in High-Stakes Settings
- **机构**: Universidade do Porto / JPMorgan
- **作者**: Inês Oliveira e Silva, Sérgio Jesus, Iker Perez, Rita P. Ribeiro, Carlos Soares
- **arXiv**: [2604.22662](https://arxiv.org/abs/2604.22662)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 对 8 种 Shapley 变体在低延迟操作风险工作流中进行大规模实证评估，审计现有量化代理指标与人类实用性的对齐程度，揭示 XAI 评测框架的根本缺陷。

---

### 12🌟 SS3D: End2End Self-Supervised 3D from Web Videos
- **机构**: ENSTA Paris / Université Paris-Saclay
- **作者**: Marwane Hariat, Gianni Franchi, David Filliat, Antoine Manzanera
- **arXiv**: [2604.22686](https://arxiv.org/abs/2604.22686)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 提出 SS3D，基于 SfM 自监督从网络视频联合预测深度、自运动和内参，采用两阶段训练调度解决大规模无约束网络视频的自监督 3D 估计挑战。

---

## GitHub Trending AI 项目（2026-04-24）

| # | 项目 | 描述 | 今日 Stars |
|---|------|------|-----------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | Agent Skills for real engineers | 2,519 ⭐ |
| 2 | [Z4nzu/hackingtool](https://github.com/Z4nzu/hackingtool) | ALL IN ONE Hacking Tool For Hackers | 1,720 ⭐ |
| 3 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | Use claude-code for free in terminal/VSCode/Discord | 1,701 ⭐ |
| 4 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | Master programming by recreating favorite technologies | 1,075 ⭐ |
| 5 | [abhigyanpatwari/GitNexus](https://github.com/abhigyanpatwari/GitNexus) | Zero-Server Code Intelligence Engine with Graph RAG Agent | 700 ⭐ |
| 6 | [openclaw/openclaw](https://github.com/openclaw/openclaw) | Your own personal AI assistant. Any OS. Any Platform. | 627 ⭐ |
| 7 | [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) | Curated list of practical Codex skills | 517 ⭐ |
| 8 | [PostHog/posthog](https://github.com/PostHog/posthog) | All-in-one developer platform with AI product assistant | 337 ⭐ |
| 9 | [trycua/cua](https://github.com/trycua/cua) | Open-source infra for Computer-Use Agents | 182 ⭐ |
| 10 | [gastownhall/beads](https://github.com/gastownhall/beads) | A memory upgrade for your coding agent | 152 ⭐ |

---

## 今日速览

- **总论文数**: 25 篇（全部来自 2026-04-24）
- **精选评分**: 12 篇
- **有开源代码**: 1 篇（Spend Less, Fit Better）
- **热点方向**: Agentic AI、LLM 推理效率、RAG 优化、3D 视觉、XAI 评测
- **GitHub Trending**: Agent 工具链占主导，Computer-Use Agent 基础设施热度上升
