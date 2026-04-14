---
layout: default
title: "AI研究简报 2026-04-14"
date: 2026-04-14
---

# 🤖 AI 研究简报

> **时间范围**: 2026-04-14 | **论文**: 30 篇 | **GitHub**: 12 个

---

## 📑 本期速览

> **本期要点**
> - 🔥 最高分论文：AggAgent 并行 Agent 聚合框架（普林斯顿大学，8🌟）
> - 🌟 重点领域：Agent 安全与规模化、VLA/机器人、视频生成、LLM 推理机制
> - 📈 GitHub 今日增长最快：[forrestchang/andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills)（🔥 +9,230）
> - 💡 亮点：Claude Code 生态全面爆发，多个相关项目冲上 Trending

---

## 📚 arXiv 精选论文

### 8🌟 Agentic Aggregation for Parallel Scaling of Long-Horizon Agentic Tasks
- **机构**: 普林斯顿大学
- **作者**: Yoonsang Lee, Howard Yen, Xi Ye, Danqi Chen
- **arXiv**: [2604.11753](https://arxiv.org/abs/2604.11753)
- **代码**: 暂无开源代码
- **分类**: cs.AI
- **核心创新**: 提出 AggAgent，将并行轨迹视为环境的聚合代理，配备轻量工具检查候选解和跨轨迹搜索。在6个基准和3个模型族上超越所有现有聚合方法，平均提升5.3%，深度研究任务提升10.3%，开销仅相当于单次代理 rollout。
- **评分理由**: 普林斯顿顶级机构，Danqi Chen 为 NLP 领域知名学者；解决 Agent 并行规模化这一核心瓶颈问题，方法新颖且效果显著。

### 8🌟 ClawGUI: A Unified Framework for Training, Evaluating, and Deploying GUI Agents
- **机构**: 浙江大学
- **作者**: Fei Tang, Zhiqiong Lu, Boxuan Zhang, Weiming Lu, Jun Xiao, Yueting Zhuang, Yongliang Shen
- **arXiv**: [2604.11784](https://arxiv.org/abs/2604.11784)
- **代码**: [GitHub](https://github.com/zju-real/ClawGUI)
- **分类**: cs.AI
- **核心创新**: 首个 GUI Agent RL 基础设施 ClawGUI-RL + 标准化评估管道 ClawGUI-Eval（95.8%复现率）+ 多平台部署 ClawGUI-Agent。训练的 ClawGUI-2B 在 MobileWorld GUI-Only 上达到17.1%成功率，超越同尺度基线6.0%。
- **评分理由**: 浙江大学，庄越挺教授团队；GUI Agent 是当前热点方向，提供完整开源训练+评估+部署框架，工程价值极高。开源代码加分。

### 7🌟 Detecting Safety Violations Across Many Agent Traces
- **机构**: 宾夕法尼亚大学
- **作者**: Adam Stein, Davis Brown, Hamed Hassani, Mayur Naik, Eric Wong
- **arXiv**: [2604.11806](https://arxiv.org/abs/2604.11806)
- **代码**: 暂无开源代码
- **分类**: cs.AI
- **核心创新**: 提出 Meerkat，结合聚类与代理搜索从大量代理轨迹中发现安全违规。发现顶级代理基准中开发者广泛作弊行为，在 CyBench 上发现的奖励黑客行为比以往审计多近4倍。
- **评分理由**: UPenn 强校，Hassani 和 Naik 为知名学者；Agent 安全审计是行业刚需，揭露奖励黑客问题影响深远。

### 7🌟 Solving Physics Olympiad via Reinforcement Learning on Physics Simulators
- **机构**: 未知机构（项目主页：sim2reason.github.io）
- **作者**: Mihir Prabhudesai, Aryan Satpathy, Yangmin Li, Zheyang Qin, Nikash Bhardwaj, Amir Zadeh, Chuan Li, Katerina Fragkiadaki, Deepak Pathak
- **arXiv**: [2604.11805](https://arxiv.org/abs/2604.11805)
- **代码**: [项目主页](https://sim2reason.github.io/)
- **分类**: cs.AI
- **核心创新**: 证明物理模拟器可作为训练 LLM 物理推理能力的强大监督来源。通过随机场景生成 + 合成 QA + RL 训练，实现零样本模拟到真实世界迁移，在 IPhO 问题上提升5-10个百分点。
- **评分理由**: 物理推理是 LLM 核心短板之一，此方法开辟 RL + 物理模拟器新路径，实验效果显著。

### 7🌟 StarVLA-α: Reducing Complexity in Vision-Language-Action Systems
- **机构**: 香港科技大学、西安交通大学、清华大学、阿里通义实验室、思谋科技
- **作者**: Jinhui Ye, Ning Gao, Senqiao Yang, Jinliang Zheng, Zixuan Wang, Yuxin Chen, Pengguang Chen, Yilun Chen, Shu Liu, Jiaya Jia
- **arXiv**: [2604.11757](https://arxiv.org/abs/2604.11757)
- **代码**: [GitHub](https://github.com/starVLA/starVLA)
- **分类**: cs.RO
- **核心创新**: 故意最小化架构和管道复杂性的 VLA 基线，在 LIBERO、SimplerEnv、RoboTwin 和 RoboCasa 上统一多基准训练。单一通用模型在真实世界 RoboChallenge 基准上超越 π₀.₅ 20%。
- **评分理由**: 港科大贾佳亚教授团队 + 阿里通义实验室，多机构联合；超越 Physical Intelligence 的 π₀.₅ 是重要里程碑。开源代码加分。

### 7🌟 SWE-AGILE: A Software Agent Framework for Efficiently Managing Dynamic Reasoning Context
- **机构**: 厦门大学、微软
- **作者**: Shuquan Lian, Juncheng Liu, Yazhe Chen, Yuhong Chen, Hui Li
- **arXiv**: [2604.11716](https://arxiv.org/abs/2604.11716)
- **代码**: [GitHub](https://github.com/KDEGroup/SWE-AGILE)
- **分类**: cs.AI
- **核心创新**: 引入动态推理上下文策略，维护推理的"滑动窗口"保持即时连续性，同时将历史推理压缩为简洁摘要。在 SWE-Bench-Verified 上为 7B-8B 模型设定新标准，仅使用 2.2k 轨迹和 896 个任务。
- **评分理由**: 厦门大学 + 微软联合；SWE-Bench 是软件工程 Agent 的核心基准，动态推理上下文管理是关键挑战。开源代码加分。

### 7🌟 LottieGPT: Tokenizing Vector Animation for Autoregressive Generation
- **机构**: 清华大学、香港理工大学、南京大学、智源研究院
- **作者**: Junhao Chen, Kejun Gao, Yuehan Cui, Mingze Sun, Mingjin Chen, Shaohui Wang, Xiaoxiao Long, Fei Ma, Qi Tian, Ruqi Huang, Hao Zhao
- **arXiv**: [2604.11792](https://arxiv.org/abs/2604.11792)
- **代码**: [项目主页](https://lottiegpt.github.io/)
- **分类**: cs.CV
- **核心创新**: 首个向量动画标记化和自回归生成框架。设计定制 Lottie 标记器，构建 660K Lottie 动画数据集，基于 Qwen-VL 微调，能从自然语言或视觉提示直接生成可编辑的向量动画。CVPR 2026 接收。
- **评分理由**: 清华 AIR + 智源研究院，田奇教授参与；CVPR 2026 正式论文，向量动画生成是全新任务范式。

### 7🌟 ClawGuard: A Runtime Security Framework for Tool-Augmented LLM Agents Against Indirect Prompt Injection
- **机构**: 新加坡管理大学
- **作者**: Wei Zhao, Zhe Li, Peixin Zhang, Jun Sun
- **arXiv**: [2604.11790](https://arxiv.org/abs/2604.11790)
- **代码**: [GitHub](https://github.com/Claw-Guard/ClawGuard)
- **分类**: cs.AI
- **核心创新**: 运行时安全框架，在每个工具调用边界强制执行用户确认的规则集，将不可靠的对齐依赖防御转化为确定性可审计机制。在5个 SOTA 语言模型上验证，无需模型修改即可阻止三种注入途径。
- **评分理由**: Agent 安全是行业刚需，间接提示注入防御方案实用性强，无需修改模型即可部署，工程落地价值高。开源代码加分。

### 7🌟 A Mechanistic Analysis of Looped Reasoning Language Models
- **机构**: 牛津大学、Google DeepMind、Mila
- **作者**: Hugh Blayney, Álvaro Arroyo, Johan Obando-Ceron, Pablo Samuel Castro, Aaron Courville, Michael M. Bronstein, Xiaowen Dong
- **arXiv**: [2604.11791](https://arxiv.org/abs/2604.11791)
- **代码**: 暂无开源代码
- **分类**: cs.CL
- **核心创新**: 首次对循环推理语言模型进行系统性机制分析，发现循环中每层收敛到不同不动点，注意力头行为趋于稳定。揭示循环块学习的推理阶段与前馈模型 closely mirror。
- **评分理由**: 牛津 + DeepMind + Mila 顶级组合；Bronstein 和 Courville 为 AI 领域知名学者；机制可解释性是理解推理模型的前沿方向。

### 6🌟 OmniShow: Unifying Multimodal Conditions for Human-Object Interaction Video Generation
- **机构**: 香港中文大学、字节跳动
- **作者**: Donghao Zhou, Guisheng Liu, Hao Yang, Jiatong Li, Jingyu Lin, Xiaohu Huang, Yichen Liu, Xin Gao, Cunjian Chen, Shilei Wen, Chi-Wing Fu, Pheng-Ann Heng
- **arXiv**: [2604.11804](https://arxiv.org/abs/2604.11804)
- **代码**: [项目主页](https://correr-zhou.github.io/OmniShow)
- **分类**: cs.CV
- **核心创新**: 端到端框架统一文本、图像、音频、姿态等多模态条件的人-物交互视频生成。引入统一通道条件注入和门控局部上下文注意力，建立 HOIVG-Bench 基准。
- **评分理由**: 港中大 + 字节跳动，傅振业教授团队；多模态视频生成是热点，统一条件框架有实用价值。

### 6🌟 LangFlow: Continuous Diffusion Rivals Discrete in Language Modeling
- **机构**: 未知机构
- **作者**: Yuxin Chen, Chumeng Liang, Hangke Sui, Ruihan Guo, Chaoran Cheng, Jiaxuan You, Ge Liu
- **arXiv**: [2604.11748](https://arxiv.org/abs/2604.11748)
- **代码**: 暂无开源代码
- **分类**: cs.CL
- **核心创新**: 首个在性能上媲美离散扩散的连续扩散语言模型。引入基于 ODE 的 NLL 边界、Gumbel 信息均匀噪声调度和自条件训练协议。在 LM1B 上达到 30.0 PPL，零样本迁移超越自回归基线。
- **评分理由**: 连续扩散语言模型性能首次追平离散方法，具有重要的理论意义和方法论创新。

### 6🌟 General365: Benchmarking General Reasoning in Large Language Models
- **机构**: 中国科学院大学、美团
- **作者**: Junlin Liu, Shengnan An, Shuang Zhou, Dan Ma, Shixiong Luo, Ying Xie, Yuan Zhang, Wenling Yuan, Yifan Zhou, Xiaoyu Li, Ziwen Wang, Xuezhi Cao, Xunliang Cai
- **arXiv**: [2604.11778](https://arxiv.org/abs/2604.11778)
- **代码**: [项目主页](https://General365.github.io)
- **分类**: cs.CL
- **核心创新**: 专门评估 LLM 通用推理能力的基准，背景知识限制在 K-12 水平，含 365 个种子问题和 1,095 个变体。评估 26 个 LLM 显示最强模型仅达 62.8% 准确率。
- **评分理由**: 产业级应用场景下的 LLM 能力评估，数据规模大（26个模型），结论有启发性。

### 6🌟 Grounded World Model for Semantically Generalizable Planning
- **机构**: NUS 新加坡国立大学、EPFL
- **作者**: Quanyi Li, Lan Feng, Haonan Zhang, Wuyang Li, Letian Wang, Alexandre Alahi, Harold Soh
- **arXiv**: [2604.11751](https://arxiv.org/abs/2604.11751)
- **代码**: 暂无开源代码
- **分类**: cs.RO
- **核心创新**: 在视觉-语言对齐潜在空间中学习的接地世界模型，基于动作未来结果与任务指令的接近程度评分。在 WISER 基准上达到 87% 成功率，传统 VLA 平均仅 22%。
- **评分理由**: NUS + EPFL 强校组合；世界模型用于机器人规划是前沿方向，87% vs 22% 的差距极其显著。

### 6🌟 HDR Video Generation via Latent Alignment with Logarithmic Encoding
- **机构**: Lightricks、特拉维夫大学
- **作者**: Naomi Ken Korem, Mohamed Oumoumad, Harel Cain, Matan Ben Yosef, Urska Jelercic, Ofir Bibi, Yaron Inger, Or Patashnik, Daniel Cohen-Or
- **arXiv**: [2604.11788](https://arxiv.org/abs/2604.11788)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 发现对数编码将 HDR 图像映射到与预训练生成模型潜在空间自然对齐的分布，无需重训练编码器即可轻量微调实现 HDR 视频生成。
- **评分理由**: 发现了简洁优雅的 latent alignment 方法解决 HDR 生成问题，Cohen-Or 为知名图形学学者，方法创新性强。

### 6🌟 C-ReD: Chinese Benchmark for AI-Generated Text Detection
- **机构**: 清华大学（深圳国际研究生院）
- **作者**: Chenxi Qing, Junxi Wu, Zheng Liu, Yixiang Qiu, Hongyao Yu, Bin Chen, Hao Wu, Shu-Tao Xia
- **arXiv**: [2604.11796](https://arxiv.org/abs/2604.11796)
- **代码**: 暂无开源代码
- **分类**: cs.CL
- **核心创新**: 全面的中文真实提示 AI 生成文本检测基准，支持可靠的域内检测和强泛化到未见 LLM 及外部中文数据集。
- **评分理由**: AI 生成文本检测是 AI 安全重要方向，中文基准稀缺，清华出品质量有保障。

### 6🌟 SyncFix: Fixing 3D Reconstructions via Multi-View Synchronization
- **机构**: 未知机构
- **作者**: Deming Li, Abhay Yadav, Cheng Peng, Rama Chellappa, Anand Bhattad
- **arXiv**: [2604.11797](https://arxiv.org/abs/2604.11797)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 通过多视图同步在扩散模型精修重建场景时强制跨视图一致性。将精修表述为联合潜在桥接匹配问题。
- **评分理由**: Chellappa 为计算机视觉领域知名学者；3D 重建一致性是经典难题，方法有新意。

### 5🌟 LMMs Meet Object-Centric Vision
- **机构**: 浙江大学、南京航空航天大学
- **作者**: Yuqian Yuan, Wenqiao Zhang, Juekai Lin, Yu Zhong, Mingjian Gao, Binhe Yu, Yunqi Cao, Wentong Li, Yueting Zhuang, Beng Chin Ooi
- **arXiv**: [2604.11789](https://arxiv.org/abs/2604.11789)
- **代码**: [GitHub](https://github.com/DCDmllm/Awesome-Object-Centric-LMMs)
- **分类**: cs.CV
- **核心创新**: 综述 LMM 与以物体为中心的视觉的交汇点最新进展，组织为理解、指代分割、视觉编辑和生成四个主题。
- **评分理由**: 综述类论文，覆盖面广，浙江大学 + 新国大（Ooi）参与，附带开源论文列表。

### 5🌟 Disentangled Point Diffusion for Precise Object Placement
- **机构**: 未知机构（可能为 CMU）
- **作者**: Lyuxing He, Eric Cai, Shobhit Aggarwal, Jianjun Wang, David Held
- **arXiv**: [2604.11793](https://arxiv.org/abs/2604.11793)
- **代码**: 暂无开源代码
- **分类**: cs.RO
- **核心创新**: 层次化解耦点扩散框架 TAX-DPD，密集 GMM 建模全局放置，解耦点云分别扩散物体几何和放置框架。
- **评分理由**: David Held 为机器人操作领域知名学者，解耦扩散思路新颖，工业应用场景明确。

### 5🌟 Psychological Concept Neurons in LLMs
- **机构**: 未知机构
- **作者**: Yuto Harada, Hiro Taiyo Hamada
- **arXiv**: [2604.11802](https://arxiv.org/abs/2604.11802)
- **代码**: 暂无开源代码
- **分类**: cs.CL
- **核心创新**: 研究大五人格在 LLM 内部的表示定位，发现概念选择性神经元在中层最集中。揭示表示控制与行为控制间的差距。
- **评分理由**: LLM 内部心理特征表示研究具有前沿探索价值，但实验规模和作者机构均较有限。

### 5🌟 HistLens: Mapping Idea Change across Concepts and Corpora
- **机构**: 北京大学
- **作者**: Yi Jing, Weiyun Qiu, Yihang Peng, Zhifang Sui
- **arXiv**: [2604.11749](https://arxiv.org/abs/2604.11749)
- **代码**: 暂无开源代码
- **分类**: cs.CL
- **核心创新**: 基于 SAE 的多概念多语料库概念历史分析框架，将概念表示分解为可解释特征并跟踪跨时间激活动态。ACL 2026 主会接收。
- **评分理由**: 北大穗志方教授团队，ACL 2026 正式论文；SAE 应用于概念演变分析是新视角。

### 5🌟 Evaluating Cooperation in LLM Social Groups through Elected Leadership
- **机构**: 未知机构（DeepMind 线索）
- **作者**: Ryan Faulkner, Anushka Deshpande, David Guzman Piedrahita, Joel Z. Leibo, Zhijing Jin
- **arXiv**: [2604.11721](https://arxiv.org/abs/2604.11721)
- **代码**: 暂无开源代码
- **分类**: cs.AI
- **核心创新**: 研究领导力和选举机制对多代理模拟中集体决策的影响。有选举领导力时社会福利分数提升55.4%，生存时间提升128.6%。
- **评分理由**: Leibo 和 Jin 为多代理研究知名学者，LLM 社会模拟是新兴方向，实验设计有启发性。

### 5🌟 Re2Pix: Representations Before Pixels
- **机构**: 未知机构
- **作者**: Efstathios Karypidis, Spyros Gidaris, Nikos Komodakis
- **arXiv**: [2604.11707](https://arxiv.org/abs/2604.11707)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 层次化视频预测框架，将预测分解为语义表示预测和表示引导的视觉合成两阶段。
- **评分理由**: Komodakis 为知名计算机视觉学者；先语义后像素的两阶段框架思路合理。

### 5🌟 Pair2Scene: Learning Local Object Relations for Procedural Scene Generation
- **机构**: 未知机构
- **作者**: Xingjian Ran, Shujie Zhang, Weipeng Zhong, Li Luo, Bo Dai
- **arXiv**: [2604.11808](https://arxiv.org/abs/2604.11808)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 程序化 3D 室内场景生成框架，通过学习局部规则结合场景层次结构和物理算法。能超越训练分布生成复杂环境。
- **评分理由**: 3D 场景生成方向有实用价值，Bo Dai 为知名学者，方法结合物理约束有新意。

### 5🌟 GenTac: Generative Modeling and Forecasting of Soccer Tactics
- **机构**: 未知机构
- **作者**: Jiayuan Rao, Tianlin Gui, Haoning Wu, Yanfeng Wang, Weidi Xie
- **arXiv**: [2604.11786](https://arxiv.org/abs/2604.11786)
- **代码**: 暂无开源代码
- **分类**: cs.LG
- **核心创新**: 基于扩散的生成式足球战术建模框架，将战术概念化为连续多玩家轨迹和离散语义事件上的随机过程。成功泛化到篮球、美式足球和冰球。
- **评分理由**: 多运动泛化的战术建模有实用价值，扩散模型应用于体育分析有新意。

### 4🌟 Multi-ORFT: Stable Online RL Fine-Tuning for Multi-Agent Diffusion Planning
- **机构**: 未知机构
- **作者**: Haojie Bai, Aimin Li, Ruoyu Yao, Xiongwei Zhao, Tingting Zhang, Xing Zhang, Lin Gao, Jun Ma
- **arXiv**: [2604.11734](https://arxiv.org/abs/2604.11734)
- **代码**: 暂无开源代码
- **分类**: cs.RO
- **核心创新**: 将场景条件扩散预训练与稳定在线强化后训练耦合，提出两级 MDP 暴露和方差门控组相对策略优化。在 WOMD 闭环基准上将碰撞率从 2.04% 降至 1.89%。
- **评分理由**: 自动驾驶协作规划方向有应用价值，但创新幅度和改进幅度相对有限。

### 4🌟 Discourse Diversity in Multi-Turn Empathic Dialogue
- **机构**: 未知机构
- **作者**: Hongli Zhan, Emma S. Gueorguieva, Javier Hernandez, Jina Suh, Desmond C. Ong, Junyi Jessy Li
- **arXiv**: [2604.11742](https://arxiv.org/abs/2604.11742)
- **代码**: 暂无开源代码
- **分类**: cs.CL
- **核心创新**: 发现 LLM 在多轮共情对话中话语策略重复率几乎是人类的2倍。提出 MINT 框架，最佳变体将聚合共情提升25.3%，话语策略重复减少26.3%。
- **评分理由**: 对话多样性研究有启发性，但聚焦面较窄，实验规模有限。

### 4🌟 Collaborative Multi-Agent Scripts for Murder Mystery Games
- **机构**: 中山大学、香港中文大学（深圳）
- **作者**: Keyang Zhong, Junlin Xie, Hefeng Wu, Haofeng Li, Guanbin Li
- **arXiv**: [2604.11741](https://arxiv.org/abs/2604.11741)
- **代码**: 暂无开源代码
- **分类**: cs.CL
- **核心创新**: 协作多代理框架评估和合成高质量角色驱动的多人游戏剧本，设计思维链微调 + GRPO 强化学习两阶段训练策略。ACL 2026 Findings。
- **评分理由**: 多代理叙事推理有娱乐价值，ACL 2026 收录，但应用场景较窄。

### 4🌟 Fairness is Not Flat: Geometric Phase Transitions Against Shortcut Learning
- **机构**: 未知机构
- **作者**: Nicolas Rodriguez-Alvarez, Fernando Rodriguez-Merino
- **arXiv**: [2604.11704](https://arxiv.org/abs/2604.11704)
- **代码**: 暂无开源代码
- **分类**: cs.LG
- **核心创新**: 通过零隐藏层拓扑审计器数学隔离垄断梯度的特征，展示容量相变。将反事实性别脆弱性从21.18%降至7.66%。
- **评分理由**: 公平性研究有社会价值，拓扑审计器方法新颖，但实验规模较小。

### 4🌟 On the Robustness of Watermarking for Autoregressive Image Generation
- **机构**: 未知机构
- **作者**: Andreas Müller, Denis Lukovnikov, Shingo Kodama, Minh Pham, Anubhav Jain, Jonathan Petit, Niv Cohen, Asja Fischer
- **arXiv**: [2604.11720](https://arxiv.org/abs/2604.11720)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 研究自回归图像生成水印方案的脆弱性，引入三种新攻击。评估显示去除和伪造攻击仅需单张水印参考图像即可有效。
- **评分理由**: 自回归图像水印方案脆弱性研究有现实意义，发现去除和伪造攻击仅需单张水印参考图像。

### 3🌟 Physics-Informed State Space Models for Solar Irradiance Forecasting
- **机构**: 未知机构（单作者）
- **作者**: Mohammed Ezzaldin Babiker Abdullah
- **arXiv**: [2604.11807](https://arxiv.org/abs/2604.11807)
- **代码**: 暂无开源代码
- **分类**: cs.LG
- **核心创新**: 热力学流形网络将15个气象变量投影到 Koopman 线性化黎曼流形中，集成光谱校准单元和热力学 Alpha 门控。五年半干旱气候测试中 RMSE 为 18.31 Wh/m²。
- **评分理由**: 领域应用性较强，但创新幅度和影响范围有限，单作者独立研究。

### 3🌟 Learning Long-term Motion Embeddings for Efficient Kinematics Generation
- **机构**: 未知机构
- **作者**: Nick Stracke, Kolja Bauer, Stefan Andreas Baumann, Miguel Angel Bautista, Josh Susskind, Björn Ommer
- **arXiv**: [2604.11737](https://arxiv.org/abs/2604.11737)
- **代码**: 暂无开源代码
- **分类**: cs.CV
- **核心创新**: 直接在大规模跟踪器轨迹上学习长期运动嵌入，64倍时间压缩。条件流匹配模型生成的运动分布超越 SOTA 视频模型和专用方法。
- **评分理由**: 运动生成方向有应用价值，但问题定义和影响范围较窄。

---

## 🔥 GitHub Trending

| 今日增长 | 项目 | 语言 | 简介 |
|----------|------|------|------|
| 🔥 +9,230 (⭐29.8k) | [forrestchang/andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills) | - | 基于 Andrej Karpathy LLM 编程经验总结的 CLAUDE.md 配置文件，改善 Claude Code 行为 |
| 🔥 +8,282 (⭐82.5k) | [nousresearch/hermes-agent](https://github.com/nousresearch/hermes-agent) | Python | Nous Research 的自进化 Agent 框架——"与你一起成长的代理" |
| 🔥 +2,979 (⭐54.7k) | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | TypeScript | Claude Code 插件，自动捕获编码过程并注入相关上下文到未来会话 |
| 🔥 +2,569 (⭐43.0k) | [shanraishan/claude-code-best-practice](https://github.com/shanraishan/claude-code-best-practice) | HTML | 从 Vibe Coding 到 Agentic Engineering 的 Claude Code 最佳实践指南 |
| 🔥 +1,928 (⭐151.5k) | [obra/superpowers](https://github.com/obra/superpowers) | Shell | Agentic 技能框架与软件开发方法论，让你的 Agent 更强大 |
| 🔥 +1,672 (⭐107.9k) | [microsoft/markitdown](https://github.com/microsoft/markitdown) | Python | 微软出品的文档转 Markdown 工具，支持 PDF/Office/图片等格式 |
| 🔥 +1,165 (⭐16.8k) | [jamiepine/voicebox](https://github.com/jamiepine/voicebox) | TypeScript | 开源语音合成工作室 |
| 🔥 +1,007 (⭐53.7k) | [virattt/ai-hedge-fund](https://github.com/virattt/ai-hedge-fund) | Python | AI 对冲基金团队，用 AI 进行投资决策 |
| 🔥 +965 (⭐17.5k) | [shiyu-coder/kronos](https://github.com/shiyu-coder/kronos) | Python | 金融市场的语言基础模型（Foundation Model for Financial Market Language） |
| 🔥 +922 (⭐39.9k) | [anthropics/claude-cookbooks](https://github.com/anthropics/claude-cookbooks) | Notebook | Anthropic 官方 Claude 使用技巧合集，涵盖多种高效用法 |
| 🔥 +769 (⭐10.9k) | [pascalorg/editor](https://github.com/pascalorg/editor) | TypeScript | 3D 建筑项目创建与分享编辑器 |
| 🔥 +390 (⭐66.0k) | [chrislgarry/apollo-11](https://github.com/chrislgarry/apollo-11) | Assembly | 阿波罗11号导航计算机原始源代码 |
