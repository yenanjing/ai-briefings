---
layout: default
title: "AI 研究简报 2026-04-07"
date: 2026-04-07T21:00:00+08:00
paper_count: 30
repo_count: 9
---

## 📊 速览

| 指标 | 数值 |
|------|------|
| 📄 论文数 | 30 篇 |
| 🏷️ 分类覆盖 | cs.CV, cs.CL, cs.LG, cs.AI, cs.RO, cs.NE, stat.ML 等 |
| ⭐ 最高评分 | 8🌟 |
| 🔥 GitHub 项目 | 9 个 |
| 📅 数据范围 | 2026-04-06 ~ 2026-04-07 |

---

## 📄 今日论文 TOP 30

### 8🌟 Vero: An Open RL Recipe for General Visual Reasoning
- **机构**: Princeton University (Danqi Chen Lab)
- **作者**: Gabriel Sarch, Linrong Cai, Qunzhong Wang, Haoyang Wu, Danqi Chen, Zhuang Liu
- **arXiv**: [2604.04917](https://arxiv.org/abs/2604.04917)
- **代码**: [项目主页](https://vero-reasoning.github.io/) — 全部数据、代码和模型已发布
- **分类**: cs.CV, cs.AI, cs.CL
- **核心创新**: 提出完全开放的 VLM 强化学习训练方案 Vero-600K（60 万样本，来自 59 个数据集），通过任务路由奖励处理异构答案格式。从 Qwen3-VL-8B-Instruct 出发，在 30 个基准中 23 个超越了 Qwen3-VL-8B-Thinking，无需额外专有思维数据。+1🌟 开源
- **评分理由**: Princeton 名校+Danqi Chen 知名学者(30%)，完全开源的 RL 训练配方具有高创新性(40%)，覆盖六大视觉推理任务类别影响面广(20%)，实验全面严谨(10%)

### 8🌟 QED-Nano: Teaching a Tiny Model to Prove Hard Theorems
- **机构**: LM-Provers (多位合作者)
- **作者**: Yuxiao Qu, Amrith Setlur, Jasper Dekoninck, Edward Beeching, Jia Li, Ian Wu, Lewis Tunstall, Aviral Kumar
- **arXiv**: [2604.04898](https://arxiv.org/abs/2604.04898)
- **代码**: 完整 QED-Nano 流水线已发布（含模型、数据集、训练和评估代码）
- **分类**: cs.AI, cs.CL, cs.LG
- **核心创新**: 仅用 4B 参数模型通过三阶段后训练（SFT → RL → 推理缓存扩展 RL）在奥赛级数学定理证明上达到接近 Gemini 3 Pro 的水平，远超 Nomos-1 和 GPT-OSS-120B 等大模型。推理缓存机制将长证明分解为迭代总结-优化循环。+1🌟 开源
- **评分理由**: 小模型达到大模型水平的高创新性(40%)，多位知名研究者合作(30%)，开源完整流程(含+1🌟)，对数学推理社区影响重大(20%)

### 8🌟 TriAttention: Efficient Long Reasoning with Trigonometric KV Compression
- **机构**: 未知机构（含 Stanford Song Han 团队关联）
- **作者**: Weian Mao, Xi Lin, Wei Huang, Yuxin Xie, Tianfu Fu, Bohan Zhuang, Song Han, Yukang Chen
- **arXiv**: [2604.04921](https://arxiv.org/abs/2604.04921)
- **代码**: [https://github.com/WeianMao/triattention](https://github.com/WeianMao/triattention)
- **分类**: cs.CL, cs.CV
- **核心创新**: 发现 pre-RoPE 空间中 Q/K 向量围绕固定非零中心高度集中的现象（Q/K concentration），利用三角级数估计 key 重要性，实现 10.7x KV 内存压缩且在 32K token 生成上匹配 Full Attention 推理精度。+1🌟 开源
- **评分理由**: Song Han（MIT/Stanford）知名学者(30%)，三角函数 KV 压缩方法新颖且效果显著(40%)，对长推理效率优化影响广泛(20%)，实验充分(10%)

### 7🌟 Early Stopping for Large Reasoning Models via Confidence Dynamics
- **机构**: Stanford University (Soheil Feizi Lab)
- **作者**: Parsa Hosseini, Sumit Nawathe, Mahdi Salmani, Meisam Razaviyayn, Soheil Feizi
- **arXiv**: [2604.04930](https://arxiv.org/abs/2604.04930)
- **代码**: 暂无
- **分类**: cs.CL, cs.AI, cs.LG
- **核心创新**: 提出 CoDE-Stop 方法，利用推理过程中间答案的置信度动态特性来决定何时终止推理。观察到正确推理轨迹往往早期就达到高置信度，而错误轨迹倾向于产生冗长低效的推理。无需额外训练即可集成到现有模型，减少 25-50% token 使用量。
- **评分理由**: Stanford 知名团队(30%)，推理效率优化是当前热点(40%)，跨模型验证充分(20%)，方法简洁优雅(10%)

### 7🌟 LoMa: Local Feature Matching Revisited
- **机构**: Lund University / Chalmers University of Technology（瑞典）
- **作者**: David Nordström, Johan Edstedt, Georg Bökman, Jonathan Astermark, Anders Heyden, Viktor Larsson, Mårten Wadenbäck, Michael Felsberg, Fredrik Kahl
- **arXiv**: [2604.04931](https://arxiv.org/abs/2604.04931)
- **代码**: [https://github.com/davnords/LoMa](https://github.com/davnords/LoMa)
- **分类**: cs.CV
- **核心创新**: 从数据驱动视角重新审视局部特征匹配，结合大规模多样化数据混合、现代训练配方和扩展的模型容量。在多个基准上全面超越 SOTA，包括 HardMatch (+18.6 mAA)、WxBS (+29.5 mAA)、InLoc (+21.4) 等。同时发布高难度数据集 HardMatch。+1🌟 开源
- **评分理由**: 多项大幅超越 SOTA 的结果(40%)，瑞典 CV 强校(30%)，新数据集 HardMatch 有价值(20%)，代码开源(含+1🌟)

### 7🌟 Vanast: Virtual Try-On with Human Image Animation via Synthetic Triplet Supervision
- **机构**: Seoul National University (Hanbyul Joo Lab)
- **作者**: Hyunsoo Cha, Wonjung Woo, Byungjun Kim, Hanbyul Joo
- **arXiv**: [2604.04934](https://arxiv.org/abs/2604.04934)
- **代码**: [项目主页](https://hyunsoocha.github.io/vanast/)
- **分类**: cs.CV
- **核心创新**: 统一虚拟试穿和姿态驱动的人体动画为单步框架，通过大规模三元组监督解决身份漂移、服装扭曲和前后不一致问题。提出 Dual Module 架构用于视频扩散 Transformer 以稳定训练。被 CVPR 2026 接收。
- **评分理由**: CVPR 2026 接收(40%)，首尔大学 Hanbyul Joo 知名学者(30%)，统一框架思路新颖(20%)，完整度高(10%)

### 7🌟 A Frame is Worth One Token: Efficient Generative World Modeling with Delta Tokens
- **机构**: TU Delft / University of Texas at Austin (Liang-Chieh Chen)
- **作者**: Tommie Kerssies, Gabriele Berton, Ju He, Qihang Yu, Wufei Ma, Daan de Geus, Gijs Dubbelman, Liang-Chieh Chen
- **arXiv**: [2604.04913](https://arxiv.org/abs/2604.04913)
- **代码**: [https://deltatok.github.io](https://deltatok.github.io)
- **分类**: cs.CV
- **核心创新**: 提出 DeltaTok tokenizer 将 VFM 特征帧间差异编码为单个连续 delta token，实现 1024x 的 token 压缩。DeltaWorld 在此基础上实现高效生成式世界模型，参数量减少 35x，FLOPs 减少 2000x，同时在密集预测任务上更接近真实结果。
- **评分理由**: 世界模型是当前热点(40%)，参数/计算量大幅降低(30%)，Liang-Chieh Chen 知名学者(20%)，思路创新(10%)

### 7🌟 How AI Aggregation Affects Knowledge
- **机构**: MIT (Daron Acemoglu)
- **作者**: Daron Acemoglu, Tianyi Lin, Asuman Ozdaglar, James Siderius
- **arXiv**: [2604.04906](https://arxiv.org/abs/2604.04906)
- **代码**: 暂无
- **分类**: econ.TH, cs.AI, cs.CY, cs.SI
- **核心创新**: 诺贝尔经济学奖得主 Daron Acemoglu 从理论角度研究 AI 聚合对社会学习的影响，扩展 DeGroot 模型引入 AI 聚合器。证明更新速度过快时不存在能稳健改善学习的权重，而局部聚合器在所有环境中都能改善学习。
- **评分理由**: Daron Acemoglu 诺贝尔奖级学者(30%)，AI 对知识影响的深刻理论分析(40%)，跨学科影响面广(20%)，证明严谨(10%)

### 7🌟 FileGram: Grounding Agent Personalization in File-System Behavioral Traces
- **机构**: Nanyang Technological University (Ziwei Liu Lab)
- **作者**: Shuai Liu, Shulin Tian, Kairui Hu, Yuhao Dong, Zhe Yang, Bo Li, Jingkang Yang, Chen Change Loy, Ziwei Liu
- **arXiv**: [2604.04901](https://arxiv.org/abs/2604.04901)
- **代码**: 框架已开源
- **分类**: cs.CV, cs.AI
- **核心创新**: 提出基于文件系统行为轨迹的 Agent 个性化框架，包含 FileGramEngine（可扩展的个性化数据引擎）、FileGramBench（诊断基准）和 FileGramOS（自底向上的记忆架构）。将用户画像从原子操作构建为过程性、语义性和情景性记忆通道。+1🌟 开源
- **评分理由**: NTU Ziwei Liu 知名学者(30%)，Agent 记忆系统是前沿方向(40%)，框架设计完整(20%)，开源(含+1🌟)

### 6🌟 Muon Dynamics as a Spectral Wasserstein Flow
- **机构**: École Normale Supérieure, Paris (Gabriel Peyré)
- **作者**: Gabriel Peyré
- **arXiv**: [2604.04891](https://arxiv.org/abs/2604.04891)
- **代码**: 暂无
- **分类**: math.OC, cs.AI, stat.ML
- **核心创新**: 在均值场框架下研究谱归一化优化规则族，引入 Spectral Wasserstein 距离族，建立 Muon 优化器的几何基础。证明了谱 Wasserstein 梯度流的等价性，获得测地凸性结果。
- **评分理由**: Gabriel Peyré 优化理论领域权威学者(30%)，Muon 优化器理论分析高创新(40%)，理论深度显著(20%)，完整度极高(10%)

### 6🌟 Your Pre-trained Diffusion Model Secretly Knows Restoration
- **机构**: Johns Hopkins University (Vishal M. Patel Lab)
- **作者**: Sudarshan Rajagopalan, Vishal M. Patel
- **arXiv**: [2604.04924](https://arxiv.org/abs/2604.04924)
- **代码**: [项目主页](https://sudraj2002.github.io/yptpage/)
- **分类**: cs.CV, cs.AI
- **核心创新**: 发现预训练扩散模型内在具有图像恢复能力，只需在文本编码器输出处学习 prompt embedding 即可解锁。提出扩散桥公式对齐训练和推理动态，在 WAN 和 FLUX 模型上实现高性能恢复。
- **评分理由**: JHU Vishal Patel 知名学者(30%)，扩散模型隐藏能力发现颇具创新(40%)，免微调方案实用性强(20%)

### 6🌟 SpatialEdit: Benchmarking Fine-Grained Image Spatial Editing
- **机构**: The University of Hong Kong / Microsoft (Nan Duan)
- **作者**: Yicheng Xiao, Wenhu Zhang, Lin Song, Yukang Chen, Wenbo Li, et al.
- **arXiv**: [2604.04911](https://arxiv.org/abs/2604.04911)
- **代码**: [https://github.com/EasonXiao-888/SpatialEdit](https://github.com/EasonXiao-888/SpatialEdit)
- **分类**: cs.CV
- **核心创新**: 提出 SpatialEdit-Bench 基准和 50 万合成的 SpatialEdit-500k 数据集，联合评估感知合理性和几何保真度。开发 SpatialEdit-16B 基线模型。+1🌟 开源
- **评分理由**: HKU + Microsoft Nan Duan 合作(30%)，大规模数据集+大模型+基准三位一体(40%)，代码开源(含+1🌟)

### 6🌟 Synthetic Sandbox for Training Machine Learning Engineering Agents
- **机构**: City University of Hong Kong (Hong Yan)
- **作者**: Yuhang Zhou, Lizhu Zhang, Yifan Wu, Jiayu Liu, Xiangjun Fan, Zhuokai Zhao, Hong Yan
- **arXiv**: [2604.04872](https://arxiv.org/abs/2604.04872)
- **代码**: 暂无
- **分类**: cs.CL, cs.LG
- **核心创新**: 提出 SandMLE 多 Agent 框架，从少量种子任务生成多样可验证的合成 MLE 环境，每个任务仅配 50-200 样本。将执行时间降低 13 倍以上，首次在 MLE 领域实现大规模在线 RL。
- **评分理由**: ML 工程 Agent 训练方案新颖(40%)，13x 效率提升意义重大(30%)，Agent 训练是热点(20%)

### 6🌟 MemMachine: A Ground-Truth-Preserving Memory System for Personalized AI Agents
- **机构**: 未知机构（Charles Fan 等）
- **作者**: Shu Wang, Edwin Yu, Oscar Love, Tom Zhang, Tom Wong, Steve Scargall, Charles Fan
- **arXiv**: [2604.04853](https://arxiv.org/abs/2604.04853)
- **代码**: 已开源
- **分类**: cs.AI
- **核心创新**: 提出保留全量对话片段的记忆系统，整合短期、长期情景和个人档案记忆。相比 Mem0 减少 ~80% 输入 token。+1🌟 开源
- **评分理由**: Agent 记忆系统方向重要(40%)，性能指标突出(30%)，80% token 节省(20%)，开源(含+1🌟)

### 6🌟 Rethinking Model Efficiency: Multi-Agent Inference with Large Models
- **机构**: 未知机构
- **作者**: Sixun Dong, Juhua Hu, Steven Li, Wei Wen, Qi Qian
- **arXiv**: [2604.04929](https://arxiv.org/abs/2604.04929)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 发现大模型可以用更少输出 token 达到更好性能，提出多 Agent 推理框架，让大模型生成短回答但从小模型转移关键推理 token。
- **评分理由**: 多 Agent 推理效率优化思路新颖(40%)，颠覆性的大模型使用范式(30%)，实用性强(20%)

### 6🌟 SkillX: Automatically Constructing Skill Knowledge Bases for Agents
- **机构**: Zhejiang University (Peng Zhang)
- **作者**: Chenxi Wang, Zhuoyun Yu, Xin Xie, Wuguannan Yao, et al.
- **arXiv**: [2604.04804](https://arxiv.org/abs/2604.04804)
- **代码**: 即将发布 [https://github.com/zjunlp/SkillX](https://github.com/zjunlp/SkillX)
- **分类**: cs.CL, cs.AI, cs.IR, cs.LG, cs.MA
- **核心创新**: 提出 SkillX 全自动框架构建可复用的 Agent 技能知识库，包含三层技能设计和迭代改进。在 AppWorld、BFCL-v3、τ²-Bench 上验证了可迁移性。
- **评分理由**: 浙大 NLP 组实力强(30%)，Agent 技能自动化构建方向前沿(40%)，多基准验证(20%)，即将开源(含+1🌟)

### 6🌟 DIRECT: Video Mashup Creation via Hierarchical Multi-Agent Planning
- **机构**: 未知机构
- **作者**: Ke Li, Maoliang Li, Jialiang Chen, Jiayu Chen, Zihao Zheng, Shaoqi Wang, Xiang Chen
- **arXiv**: [2604.04875](https://arxiv.org/abs/2604.04875)
- **代码**: [https://github.com/AK-DREAM/DIRECT](https://github.com/AK-DREAM/DIRECT)
- **分类**: cs.CV, cs.AI, cs.MM
- **核心创新**: 将视频混剪创作形式化为多模态一致性满足问题，提出层级多 Agent 框架 DIRECT（编剧→导演→编辑三级级联）。+1🌟 开源
- **评分理由**: 视频 AI 生成热点方向(40%)，多 Agent 层级设计思路好(30%)，基准+代码开源(含+1🌟)

### 6🌟 Beyond the Final Actor: Modeling Creator and Editor Roles for LLM Text Detection
- **机构**: Chinese Academy of Sciences (Juan Cao)
- **作者**: Yang Li, Qiang Sheng, Zhengjia Wang, Yehan Yang, Danding Wang, Juan Cao
- **arXiv**: [2604.04932](https://arxiv.org/abs/2604.04932)
- **代码**: 暂无
- **分类**: cs.CL
- **核心创新**: 提出 RACE 方法进行细粒度 LLM 文本检测（四分类设定），利用修辞结构理论构建逻辑图表征创作者基础。提供政策对齐的 LLM 监管方案。
- **评分理由**: 中科院 Juan Cao 团队(30%)，四分类细粒度检测思路创新(40%)，社会意义大(20%)

### 6🌟 E-VLA: Event-Augmented Vision-Language-Action Model
- **机构**: 未知机构（Kaiwei Wang 等）
- **作者**: Jiajun Zhai, Hao Shi, Shangwei Guo, Kailun Yang, Kaiwei Wang
- **arXiv**: [2604.04834](https://arxiv.org/abs/2604.04834)
- **代码**: [https://github.com/JJayzee/E-VLA](https://github.com/JJayzee/E-VLA)
- **分类**: cs.CV, cs.MM, cs.RO
- **核心创新**: 将事件相机直接集成到 VLA 模型中，在极暗和运动模糊场景下显著提升操作鲁棒性。在 20 lux 下 Pick-Place 成功率从 0% 提升到 90%。+1🌟 开源
- **评分理由**: 事件相机+VLA 结合思路新颖(40%)，实际场景效果显著(30%)，开源数据集和代码(含+1🌟)

### 5🌟 Are Latent Reasoning Models Easily Interpretable?
- **机构**: 未知机构
- **作者**: Connor Dilgren, Sarah Wiegreffe
- **arXiv**: [2604.04902](https://arxiv.org/abs/2604.04902)
- **代码**: 暂无
- **分类**: cs.LG
- **核心创新**: 系统调查 LRM 可解释性，发现隐式推理 token 往往不必要，且可解码出 65-93% 的正确推理轨迹。可解释性本身是预测正确性的信号。
- **评分理由**: LRM 可解释性分析对领域理解有重要价值(40%)，发现令人意外(30%)，但分析为主(20%)

### 5🌟 Fully Procedural Synthetic Data from Simple Rules for Multi-View Stereo
- **机构**: Princeton University (Jia Deng Lab)
- **作者**: Zeyu Ma, Alexander Raistrick, Jia Deng
- **arXiv**: [2604.04925](https://arxiv.org/abs/2604.04925)
- **代码**: [https://github.com/princeton-vl/SimpleProc](https://github.com/princeton-vl/SimpleProc)
- **分类**: cs.CV
- **核心创新**: SimpleProc 用极少规则生成全程序化 MVS 训练数据。352K 图片可媲美 692K 手工数据训练的模型。+1🌟 开源
- **评分理由**: Princeton Jia Deng(30%)，极简规则生成高质量数据(40%)，但 MVS 偏垂直领域(20%)

### 5🌟 HorizonWeaver: Generalizable Multi-Level Semantic Editing for Driving Scenes
- **机构**: 未知机构
- **作者**: Mauricio Soroco, Francesco Pittaluga, et al.
- **arXiv**: [2604.04887](https://arxiv.org/abs/2604.04887)
- **代码**: [项目主页](https://msoroco.github.io/horizonweaver/)
- **分类**: cs.CV
- **核心创新**: 驾驶场景多粒度语义编辑框架，255K 配对数据集，+46.4% 用户偏好。
- **评分理由**: 驾驶场景编辑实用性强(40%)，大规模数据集(30%)，自动驾驶方向(20%)

### 5🌟 PointTPA: Dynamic Network Parameter Adaptation for 3D Scene Understanding
- **机构**: Huazhong University of Science and Technology (Xiang Bai)
- **作者**: Siyuan Liu, Chaoqun Zheng, Xin Zhou, Tianrui Feng, Dingkang Liang, Xiang Bai
- **arXiv**: [2604.04933](https://arxiv.org/abs/2604.04933)
- **代码**: [https://github.com/H-EmbodVis/PointTPA](https://github.com/H-EmbodVis/PointTPA)
- **分类**: cs.CV
- **核心创新**: 测试时参数自适应框架，仅增加不到 2% 参数量，ScanNet 验证集达到 78.4% mIoU。+1🌟 开源
- **评分理由**: HUST Xiang Bai 知名学者(30%)，测试时自适应思路好(40%)，3D 场景理解偏垂直(20%)

### 5🌟 ANX: Protocol-First Design for AI Agent Interaction
- **机构**: 个人作者 (Xu Mingze)
- **作者**: Xu Mingze
- **arXiv**: [2604.04820](https://arxiv.org/abs/2604.04820)
- **代码**: 暂无
- **分类**: cs.AI, cs.CL
- **核心创新**: Agent 原生协议 ANX 和 3EX 解耦架构，相比 MCP 减少 47-56% token，执行时间缩短 58%。
- **评分理由**: Agent 交互协议设计是热点(40%)，效率提升显著(30%)，但单一作者(20%)

### 5🌟 Rethinking Exploration in RLVR: AsymGRPO
- **机构**: 未知机构
- **作者**: Hengrui Gu, Xiaotian Han, Yujing Bian, Kaixiong Zhou
- **arXiv**: [2604.04894](https://arxiv.org/abs/2604.04894)
- **代码**: 暂无
- **分类**: cs.CL, cs.AI, cs.LG
- **核心创新**: 将策略熵分解为"信息熵"和"虚假熵"，提出 AsymGRPO 框架对正负 rollout 分别调制。
- **评分理由**: RLVR 探索机制的理论分析有深度(40%)，熵分解视角新颖(30%)，但实验规模有限(20%)

### 5🌟 LiveFact: A Dynamic, Time-Aware Benchmark for Fake News Detection
- **机构**: 未知机构
- **作者**: Cheng Xu, Changhong Jin, Yingjie Niu, et al.
- **arXiv**: [2604.04815](https://arxiv.org/abs/2604.04815)
- **代码**: 暂无
- **分类**: cs.CL, cs.AI
- **核心创新**: 动态时间感知的虚假新闻检测基准 LiveFact，测试 22 个 LLM，发现开源 MoE 模型已匹配或超越专有模型。
- **评分理由**: 动态基准对评估污染问题有意义(40%)，22 个模型的大规模评测(30%)，但方法创新有限(20%)

### 4🌟 Free-Range Gaussians: Non-Grid-Aligned Generative 3D Gaussian Reconstruction
- **机构**: 多机构合作
- **作者**: Ahan Shabanov, Peter Hedman, Ethan Weber, et al.
- **arXiv**: [2604.04874](https://arxiv.org/abs/2604.04874)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 非像素、非体素对齐的 3D 高斯重建方法，通过 flow matching 预测高斯参数，仅需 4 张图片即可重建。
- **评分理由**: 3D Gaussian 领域持续创新(40%)，多机构合作(30%)，4 图重建令人印象深刻(20%)

### 4🌟 Beyond Global Scores: Fine-Grained Token Grounding for LVLM Hallucination Detection
- **机构**: 多机构合作
- **作者**: Tuan Dung Nguyen, Minh Khoi Ho, Qi Chen, Yutong Xie, et al.
- **arXiv**: [2604.04863](https://arxiv.org/abs/2604.04863)
- **代码**: 暂无
- **分类**: cs.CV
- **核心创新**: 发现幻觉 token 的两个特征，开发 patch 级幻觉检测方法，token 级检测准确率达 90%。
- **评分理由**: LVLM 幻觉检测机制分析有价值(40%)，90% 检测准确率(30%)，但实用落地尚待验证(20%)

### 4🌟 Agentic Federated Learning: The Future of Distributed Training
- **机构**: University of Campinas（巴西）
- **作者**: Rafael O. Jarczewski, Gabriel U. Talasso, Leandro Villas, Allan M. de Souza
- **arXiv**: [2604.04895](https://arxiv.org/abs/2604.04895)
- **代码**: 暂无
- **分类**: cs.MA, cs.AI
- **核心创新**: 提出 Agentic-FL 范式，让 LM Agent 承担联邦学习中的自主编排角色。
- **评分理由**: Agent + 联邦学习交叉有创意(40%)，但主要是概念框架(30%)，缺乏大规模实验(20%)

---

## 🔥 GitHub Trending AI 项目

| # | 项目 | Stars | 今日 | 描述 |
|---|------|-------|------|------|
| 1 | [GitNexus](https://github.com/abhigyanpatwari/GitNexus) | 24,088 | +1,174 | 客户端知识图谱引擎，浏览器运行，支持 Graph RAG |
| 2 | [qmd](https://github.com/tobi/qmd) | 19,219 | +859 | 迷你 CLI 搜索引擎，完全本地运行 |
| 3 | [google-ai-edge/gallery](https://github.com/google-ai-edge/gallery) | 18,397 | +899 | Google 端侧 ML/GenAI 用例展示 |
| 4 | [DeepTutor](https://github.com/hkuds/DeepTutor) | 11,706 | +164 | Agent 原生个性化学习助手 |
| 5 | [RedditVideoMakerBot](https://github.com/Elebumm/RedditVideoMakerBot) | 9,755 | +656 | 一键创建 Reddit 视频 |
| 6 | [PersonaPlex](https://github.com/NVIDIA/PersonaPlex) | 7,677 | +663 | NVIDIA PersonaPlex |
| 7 | [andrej-karpathy-skills](https://github.com/forrestchang/andrej-karpathy-skills) | 7,755 | +42 | Andrej Karpathy Skills |
| 8 | [litert-lm](https://github.com/google-ai-edge/litert-lm) | 2,325 | +522 | Google LiteRT LLM 运行时 |
| 9 | [SEOMachine](https://github.com/thecraigewitt/SEOMachine) | 3,600 | +213 | Claude Code SEO 内容工作区 |

---

## 🏷️ 关键词索引

| 关键词 | 相关论文/项目 |
|--------|-------------|
| **RL / 强化学习** | Vero, QED-Nano, AsymGRPO, Agentic-FL |
| **KV Cache / 推理效率** | TriAttention, CoDE-Stop, Multi-Agent Inference |
| **世界模型** | DeltaWorld |
| **3D 重建** | LoMa, Free-Range Gaussians, PointTPA, SimpleProc |
| **Agent / 记忆** | FileGram, MemMachine, SkillX, ANX, DIRECT, SandMLE |
| **视频生成/编辑** | Vanast, DIRECT, HorizonWeaver |
| **图像恢复/编辑** | Diffusion Restoration, SpatialEdit |
| **幻觉检测** | Token Grounding, Plausibility |
| **数学推理** | QED-Nano |
| **视觉推理** | Vero, DDP |
| **端侧 AI** | Google AI Edge, E-VLA, ClickAIXR |
| **AI 安全** | Kolmogorov Safety, PCSA |

---

> 📅 本简报由 AI 自动生成 | 数据来源: arXiv API, GitHub Trending
