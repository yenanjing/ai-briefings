---
layout: default
title: "AI研究简报 2026-04-03"
date: 2026-04-03
---

> **时间范围**: 2026-04-03 → 2026-04-03 | **论文**: 20 篇 | **GitHub**: 2 个
> 🌐 [在线版](https://yenanjing.github.io/ai-briefings/2026-04-03)

---

## 📑 本期速览

> [!summary] 本期要点
> - 🔥 最高分论文：Generative World Renderer（Meta Reality Labs）
> - 🌟 重点领域：计算机视觉 / 多模态 / 大语言模型 / 强化学习
> - 📈 GitHub 最热：system_prompts_leaks（⭐ 36,520）

---

## 📚 arXiv 精选论文

### 8🌟 Generative World Renderer
- **机构**: Meta Reality Labs
- **作者**: Zheng-Hui Huang, Zhixiang Wang, Jiaming Tan, Ruihan Yu, Yidan Zhang, Bo Zheng, Yu-Lun Liu, Yung-Yu Chuang, Kaipeng Zhang
- **arXiv**: [2604.02329](https://arxiv.org/abs/2604.02329)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 从 AAA 游戏构建大规模动态数据集，包含 400 万帧同步 RGB 和 G-buffer 通道，用于世界模型训练。
- **评分理由**: Meta 出品，数据集规模庞大（4M 帧），对世界模型研究有重要价值，创新点明显。

---

### 8🌟 Large-scale Codec Avatars: The Unreasonable Effectiveness of Large-scale Avatar Pretraining
- **机构**: Meta Reality Labs
- **作者**: Junxuan Li, Rawal Khirodkar, Chengan He, Zhongshi Jiang, Giljoo Nam 等
- **arXiv**: [2604.02320](https://arxiv.org/abs/2604.02320)
- **代码**: 暂无开源代码
- **分类**: cs.CV, cs.GR
- **核心创新**: 使用 100 万野外视频进行预训练/后训练范式，学习广泛先验，然后在高质量精选数据上后训练。
- **评分理由**: Meta 顶级团队，大规模预训练范式（1M 视频），高保真 3D 头像模型，工程价值高。

---

### 7🌟 Omni123: Exploring 3D Native Foundation Models with Limited 3D Data by Unifying Text to 2D and 3D Generation
- **机构**: 未知机构
- **作者**: Chongjie Ye, Cheng Cao, Chuanyu Pan, Yiming Hao, Yihao Zhi, Yuanming Hu, Xiaoguang Han
- **arXiv**: [2604.02289](https://arxiv.org/abs/2604.02289)
- **代码**: 暂无开源代码
- **分类**: cs.CV, cs.AI
- **核心创新**: 在单一自回归框架内统一文本到 2D 和 3D 生成的 3D 原生基础模型，用有限 3D 数据实现 3D 生成。
- **评分理由**: 统一 2D/3D 生成的新范式，方法新颖，解决 3D 数据稀缺问题，跨领域影响较大。

---

### 7🌟 ActionParty: Multi-Subject Action Binding in Generative Video Games
- **机构**: 未知机构
- **作者**: Alexander Pondaven, Ziyi Wu, Igor Gilitschenski, Philip Torr, Sergey Tulyakov, Fabio Pizzati, Aliaksandr Siarohin
- **arXiv**: [2604.02330](https://arxiv.org/abs/2604.02330)
- **代码**: 暂无开源代码
- **分类**: cs.CV, cs.AI, cs.LG
- **核心创新**: 引入主体状态令牌控制视频扩散模型中的多个智能体，实现能同时控制多达七名玩家的系统。
- **评分理由**: 多智能体视频生成的首创，创新点突出，对游戏/视频生成领域影响显著。

---

### 7🌟 STOP: Steerable Visual Representations
- **机构**: 未知机构
- **作者**: Jona Ruthardt, Manu Gaur, Deva Ramanan, Makarand Tapaswi, Yuki M. Asano
- **arXiv**: [2604.02327](https://arxiv.org/abs/2604.02327)
- **代码**: 暂无开源代码
- **分类**: cs.CV, cs.AI
- **核心创新**: 可操控的视觉表示，通过轻量级交叉注意力早期融合，用自然语言控制全局和局部特征。
- **评分理由**: 视觉表示的新范式，可控性强，对视觉理解和生成有重要价值。

---

### 7🌟 Batched Contextual Reinforcement: A Task-Scaling Law for Efficient Reasoning
- **机构**: 未知机构
- **作者**: Bangji Yang, Hongbo Ma, Jiajun Fan, Ge Liu
- **arXiv**: [2604.02322](https://arxiv.org/abs/2604.02322)
- **代码**: 暂无开源代码
- **分类**: cs.LG, cs.AI, cs.CL
- **核心创新**: 训练模型同时解决 N 个问题，实现高效推理，在数学基准上减少 token 使用同时保持或提高准确率。
- **评分理由**: 任务扩展定律的新发现，效率提升明显，对大模型推理有实际应用价值。

---

### 6🌟 SKILL0: In-Context Agentic Reinforcement Learning for Skill Internalization
- **机构**: 未知机构
- **作者**: Zhengxi Lu, Zhiyuan Yao, Jinyang Wu, Chengcheng Han, Qi Gu, Xunliang Cai, Weiming Lu, Jun Xiao, Yueting Zhuang, Yongliang Shen
- **arXiv**: [2604.02268](https://arxiv.org/abs/2604.02268)
- **代码**: 暂无开源代码
- **分类**: cs.LG
- **核心创新**: 探索技能是否可以内化到模型参数中，实现零样本自主行为而无需运行时技能检索。
- **评分理由**: 技能内化的新思路，对 Agent 能力构建有理论价值，实验设计合理。

---

### 6🌟 Grounded Token Initialization for New Vocabulary in LMs for Generative Recommendation
- **机构**: 未知机构
- **作者**: Daiwei Chen, Zhoutong Fu, Chengming Jiang, Haichao Zhang, Ran Zhou, Tan Wang 等
- **arXiv**: [2604.02324](https://arxiv.org/abs/2604.02324)
- **代码**: 暂无开源代码
- **分类**: cs.CL, cs.AI, cs.LG
- **核心创新**: 分析新词汇令牌的平均初始化策略（会导致退化子空间），提出 GTI 对新令牌进行语言学接地。
- **评分理由**: 对词汇初始化问题的深入分析，提出系统性解决方案，对生成式推荐和大模型训练有意义。

---

### 6🌟 EventHub: Data Factory for Generalizable Event-Based Stereo Networks without Active Sensors
- **机构**: 未知机构
- **作者**: Luca Bartolomei, Fabio Tosi, Matteo Poggi, Stefano Mattoccia, Guillermo Gallego
- **arXiv**: [2604.02331](https://arxiv.org/abs/2604.02331)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 事件相机的无源传感器深度立体网络训练框架，使用标准彩色图像代替昂贵的主动传感器标注。
- **评分理由**: 解决事件相机标注成本问题，方法实用，对事件相机应用有推动作用。

---

### 6🌟 VOID: Video Object and Interaction Deletion
- **机构**: 未知机构
- **作者**: Saman Motamed, William Harvey, Benjamin Klein, Luc Van Gool, Zhuoning Yuan, Ta-Ying Cheng
- **arXiv**: [2604.02296](https://arxiv.org/abs/2604.02296)
- **代码**: 暂无开源代码
- **分类**: cs.CV, cs.AI
- **核心创新**: 视频对象移除框架，需要修改下游物理交互以实现物理合理的填充。
- **评分理由**: 视频编辑的新方向，考虑物理交互的影响，思路独特，工程实现复杂度高。

---

### 6🌟 Unifying Group-Relative and Self-Distillation Policy Optimization via Sample Routing
- **机构**: 未知机构
- **作者**: Gengsheng Li, Tianyu Yang, Junfeng Fang, Mingyang Song, Mao Zheng, Haiyun Guo, Dan Zhang, Jinqiao Wang, Tat-Seng Chua
- **arXiv**: [2604.02288](https://arxiv.org/abs/2604.02288)
- **代码**: 暂无开源代码
- **分类**: cs.LG, cs.AI
- **核心创新**: SRPO 将正确样本路由到 GRPO 的奖励对齐强化，失败样本路由到 SDPO 的目标 logit 级校正。
- **评分理由**: 统一两种策略优化方法，样本路由思想新颖，对强化学习算法设计有贡献。

---

### 6🌟 MetaNav: Stop Wandering - Efficient Vision-Language Navigation via Metacognitive Reasoning
- **机构**: 未知机构
- **作者**: Xueying Li, Feng Lyu, Hao Wu, Mingliu Liu, Jia-Nan Liu, Guozi Liu
- **arXiv**: [2604.02318](https://arxiv.org/abs/2604.02318)
- **代码**: 暂无开源代码
- **分类**: cs.RO, cs.CV
- **核心创新**: 元认知导航智能体，整合空间记忆、历史感知规划和反思纠正，实现高效视觉语言导航。
- **评分理由**: 元认知在导航中的应用，方法完整，对具身智能有意义。

---

### 5🌟 A Simple Baseline for Streaming Video Understanding
- **机构**: 南洋理工大学
- **作者**: Yujiao Shen, Shulin Tian, Jingkang Yang, Ziwei Liu
- **arXiv**: [2604.02317](https://arxiv.org/abs/2604.02317)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 用滑动窗口基线喂给最近 N 帧到现成 VLM，已匹配或超越发布的流式模型。
- **评分理由**: 简单有效的方法，挑战现有流式模型趋势，但创新性有限。

---

### 5🌟 No Single Best Model for Diversity: Learning a Router for Sample Diversity
- **机构**: 华盛顿大学
- **作者**: Yuhan Liu, Fangyuan Xu, Vishakh Padmakumar, Daphne Ippolito, Eunsol Choi
- **arXiv**: [2604.02319](https://arxiv.org/abs/2604.02319)
- **代码**: 暂无开源代码
- **分类**: cs.CL
- **核心创新**: 引入多样性覆盖率指标和路由器，为每个查询预测最佳模型以生成全面的开放响应。
- **评分理由**: 多样性度量的新思路，路由方法实用，但影响力有限。

---

### 5🌟 Beyond Referring Expressions: Scenario Comprehension Visual Grounding
- **机构**: 弗吉尼亚大学
- **作者**: Ruozhen He, Nisarg A. Shah, Qihua Dong, Zilin Xiao, Jaywon Koo, Vicente Ordonez
- **arXiv**: [2604.02323](https://arxiv.org/abs/2604.02323)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: RSC 基准用于基于场景的视觉定位，目标需从角色、意图和关系上下文推断而非显式命名。
- **评分理由**: 新的定位任务定义，更贴近真实场景，但方法相对传统。

---

### 5🌟 Crystalite: A Lightweight Transformer for Efficient Crystal Modeling
- **机构**: 未知机构
- **作者**: Tin Hadži Veljković, Joshua Rosenthal, Ivor Lončarič, Jan-Willem van de Meent
- **arXiv**: [2604.02270](https://arxiv.org/abs/2604.02270)
- **代码**: 暂无开源代码
- **分类**: cs.LG, cs.AI
- **核心创新**: 带原子令牌化和几何增强模块的扩散 Transformer 晶体建模。
- **评分理由**: 面向晶体建模的专用 Transformer，方法合理，但影响范围较为局限。

---

### 5🌟 The Self Driving Portfolio: Agentic Architecture for Institutional Asset Management
- **机构**: 未知机构
- **作者**: Andrew Ang, Nazym Azimbayev, Andrey Kim
- **arXiv**: [2604.02279](https://arxiv.org/abs/2604.02279)
- **代码**: 暂无开源代码
- **分类**: cs.AI, cs.MA
- **核心创新**: 代理战略资产配置流水线，约 50 个专业智能体产生资本市场假设，构建组合。
- **评分理由**: 大规模 Agent 架构在金融领域的应用，设计有趣，但创新性和严谨性一般。

---

### 5🌟 De Jure: Iterative LLM Self-Refinement for Structured Extraction of Regulatory Rules
- **机构**: 未知机构
- **作者**: Keerat Guliani, Deepkamal Gill, David Landsman, Nima Eshraghi, Krishna Kumar, Lovedeep Gondara
- **arXiv**: [2604.02276](https://arxiv.org/abs/2604.02276)
- **代码**: 暂无开源代码
- **分类**: cs.AI, cs.CL, cs.LG
- **核心创新**: 全自动化、领域无关的法规规则结构化提取流水线，无需人类标注。
- **评分理由**: 实用性强的 NLP 应用，方法完整，但创新性有限。

---

### 5🌟 Answering the Wrong Question: Reasoning Trace Inversion for Abstention in LLMs
- **机构**: 未知机构
- **作者**: Abinathab Gourabathina, Inkit Padhi, Manish Nagireddy, Subhajit Chaudhury, Prasanna Sattigeri
- **arXiv**: [2604.02230](https://arxiv.org/abs/2604.02230)
- **代码**: 暂无开源代码
- **分类**: cs.AI
- **核心创新**: 将导致拒答失败的幻觉重新解释为 LLM 回答错误问题而非问题本身，提出推理痕迹反转方法。
- **评分理由**: 对 LLM 拒答问题的新视角，理论分析有价值，但实际应用效果待验证。

---

### 4🌟 Topological Effects in Neural Network Field Theory
- **机构**: 未知机构
- **作者**: Christian Ferko, James Halverson, Vishnu Jejjala, Brandon Robinson
- **arXiv**: [2604.02313](https://arxiv.org/abs/2604.02313)
- **代码**: 暂无开源代码
- **分类**: hep-th, cs.LG
- **核心创新**: 扩展神经网络场理论到拓扑设置，恢复 Berezinskii-Kosterlitz-Thouless 转变并验证玻色弦理论的 T-对偶。
- **评分理由**: 理论物理方向的工作，与实际 AI 应用距离较远，影响力相对局限。

---

## 🔥 GitHub Trending

| 热度 | 项目 | 语言 | 简介 |
|------|------|------|------|
| ⭐ 36,520 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | - | 提取自 ChatGPT (GPT-5.4, 5.3)、Claude (Opus 4.6, Sonnet 4.6)、Gemini 等模型系统提示词，定期更新 |
| ⭐ 12,023 | [Yeachan-Heo/oh-my-codex](https://github.com/Yeachan-Heo/oh-my-codex) | TypeScript | OmX - 为代码添加钩子、代理团队、HUD 等扩展功能 |

---

## 🏷️ 关键词索引

#world-model #multimodal #video-generation #3d-generation #foundation-model #avatar-pretraining #event-camera #vision-language #reinforcement-learning #skill-internalization #token-initialization #agentic-ai #video-editing

---

#AI简报 #2026年 #04月 #arxiv #github-trending
