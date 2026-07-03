---
layout: default
title: "AI Research Briefing - 2026-06-29"
date: 2026-06-29 10:55:00 +08:00
---

# AI Research Briefing - 2026-06-29

> 自动生成于 2026-06-29 10:55 CST

## 📚 论文精选（12 篇）

### 8.0🌟 Paper Assistant Tool: Agentic AI for Scientific Review
- **作者**: Rajesh Jayaram, Drew Tyler, David Woodruff, Corinna Cortes, Yossi Matias, Vahab Mirrokni 等
- **arXiv**: [2606.28277](https://arxiv.org/abs/2606.28277)
- **分类**: cs.LG
- **核心创新**: Google DeepMind 推出 PAT 工具用于深度科学评审，利用推理缩放技术在 SPOT 基准上数学错误检测提升 34%，已在 STOC/ICML 作为投稿前工具部署。

### 7.9🌟 SimFoundry: Video-to-Sim Scene Generation for Robot Policy Learning
- **作者**: Nadun Ranawaka, Josiah Wong, Wei-Lin Pai, Danfei Xu, Li Fei-Fei, Yuke Zhu 等
- **arXiv**: [2606.28276](https://arxiv.org/abs/2606.28276)
- **分类**: cs.RO
- **核心创新**: NVIDIA/Stanford/CMU 联合，从视频自动生成模拟场景，支持物体/场景/任务编辑生成"数字表亲"，零样本迁移相关性达 0.911，跨 7 个操作任务平均提升 21-40%。

### 7.8🌟 PerceptionRubrics: Calibrating Multimodal Evaluation to Human Perception
- **作者**: Yana Wei, Hongbo Peng, Yanning Lai, Xiangyu Zhang, Daxin Jiang, Vishal M. Patel 等
- **arXiv**: [2606.28322](https://arxiv.org/abs/2606.28322)
- **分类**: cs.CV
- **核心创新**: ICML 2026 接收，提出基于标准的多模态评估框架，1038 张密集图像配 12000+ 细粒度标准，采用门控评分机制揭示开放源与专有前沿 8% 感知差距。

### 7.7🌟 Vision-Default, Prior-Override: Causal Mechanisms in VLMs
- **作者**: Niclas Lietzow, Danielle Bitterman, Carsten Eickhoff, William Rudman, Michal Golovanevsky
- **arXiv**: [2606.28273](https://arxiv.org/abs/2606.28273)
- **分类**: cs.CL
- **核心创新**: 首次揭示 VLM 感知-知识冲突的因果机制，发现仅 2.5-4.8% 注意力头负责先验定锚，可分解为路由头和写入头，跨模型家族一致性强。

### 7.6🌟 StructSplat: Generalizable 3D Gaussian Splatting from Uncalibrated Views
- **作者**: Jia-Chen Zhao, Beiqi Chen, Xinyang Chen, Liqiang Nie
- **arXiv**: [2606.28321](https://arxiv.org/abs/2606.28321)
- **分类**: cs.CV
- **核心创新**: 无需标定图像的前馈 3DGS 框架，采用结构化表示分离几何/语义/纹理，DL3DV 上 PSNR 达 28.045（超 AnySplat 5.67dB），跨数据集泛化 +1.7~1.9dB。
- **代码**: [github.com/J-C-Zhao/StructSplat](https://github.com/J-C-Zhao/StructSplat)

### 7.6🌟 Uni-Mo: Infinite Expressive Quadrupedal Motion via Video Priors
- **作者**: Youzhi Liu, Li Gao, Yifei Qian
- **arXiv**: [2606.28237](https://arxiv.org/abs/2606.28237)
- **分类**: cs.RO
- **核心创新**: 全自动生成四足机器人运动生成，LLM 提议动作提示 + 视频扩散模型合成 + 3D 轨迹提取，开源 7488 个语言标注动作（18.5 小时），96.7% 部署成功率。
- **代码**: [github.com/GaoLii/Quad-Imaginarium](https://github.com/GaoLii/Quad-Imaginarium)

### 7.5🌟 DexCompose: Reusing Dexterous Policies for Multi-Task Manipulation
- **作者**: Dihong Huang, Zhenyu Wei, Zhuxiu Xu, Yunchao Yao, Sikai Li, Mingyu Ding
- **arXiv**: [2606.28323](https://arxiv.org/abs/2606.28323)
- **分类**: cs.RO
- **核心创新**: 角色感知残差组合框架，通过显式手指级动作所有权复用预训练灵巧策略，16 个复合任务平均成功率 77.4%，解决策略间破坏性干扰问题。
- **代码**: [devon018.github.io/DexCompose-Webpage](https://devon018.github.io/DexCompose-Webpage/)

### 7.5🌟 WARP-RM: Warp-Augmented Relative Progress Reward Model
- **作者**: Justin Yu, Andrew Goldberg, Mac Schwager, Ken Goldberg, Philipp Wu 等
- **arXiv**: [2606.28320](https://arxiv.org/abs/2606.28320)
- **分类**: cs.RO
- **核心创新**: 全自监督时间扭曲增强相对进度奖励模型，从成功演示学习密集帧级进度信号，WARP-BC 在 T 恤折叠任务上吞吐量提升 18×（19/20 vs 2/20）。

### 7.4🌟 RSICCLLM: Multimodal LLM for Remote Sensing Image Change Captioning
- **作者**: Yelin Wang, Zijia Song, Shuo Ye, Yong Xu, Zitong Yu
- **arXiv**: [2606.28266](https://arxiv.org/abs/2606.28266)
- **分类**: cs.CV
- **核心创新**: ECCV 2026 接收，首个遥感图像变化描述 LLM 后训练框架，7B 参数超越更大模型，双负偏好优化（DNPO）构建互补负样本，代码数据集开源。
- **代码**: [github.com/keaill/RSICCLLM](https://github.com/keaill/RSICCLLM)

### 7.3🌟 Agent-Native Immune System (ANIS): Architecture & Taxonomy
- **作者**: Bo Shen, Lifeng Chang, Tianyuan Wei, Feng Shi 等
- **arXiv**: [2606.28270](https://arxiv.org/abs/2606.28270)
- **分类**: cs.AI
- **核心创新**: 首个生物启发的 Agent 内源防御架构，六层免疫塔（L0-L5）含屏障免疫层，区分非参数疫苗和参数疫苗，提出持续免疫学习使疫苗动态适应新型威胁。

### 7.3🌟 Proper Positive-Only Learning: PAC Learning Theory Breakthrough
- **作者**: Shai Ben-David, Farnam Mansouri, Anay Mehrotra, Manolis Zampetakis
- **arXiv**: [2606.28309](https://arxiv.org/abs/2606.28309)
- **分类**: stat.ML
- **核心创新**: 首次完全刻画 proper 正样本 PAC 学习的充要条件：有限 VC 维度 + 均匀外部可分性，揭示 proper/improper、随机化/确定性学习的分离，引入新的组合维度。

### 7.2🌟 HPRO: Hierarchical Progressive Reward Optimization for Emotional TTS
- **作者**: Sihang Nie, Xiaofen Xing, Rui Xing, Xiangmin Xu
- **arXiv**: [2606.28249](https://arxiv.org/abs/2606.28249)
- **分类**: cs.CL
- **核心创新**: 情感 TTS 层级偏好优化框架，HD-Emo 编解码器将内容和风格偏好分离到不同 token，从句子级到帧级渐进对齐，解决内容-情感梯度冲突。
- **代码**: [xxh333.github.io/hpro-demo](https://xxh333.github.io/hpro-demo/)

---

## 🔥 GitHub Trending (AI 相关)

| 项目 | Stars | 今日新增 | 描述 |
|------|-------|----------|------|
| DeusData/codebase-memory-mcp | 19.9k | 2,190 | 高性能代码智能 MCP 服务器，158 种语言 |
| xbtlin/ai-berkshire | 5.5k | 1,445 | AI 价值投资框架，多 Agent 研究 |
| HKUDS/Vibe-Trading | 14.4k | 492 | 个人交易 Agent |
| opendatalab/MinerU | 71.7k | 380 | 文档转 LLM 格式，Agent 工作流 |
| Robbyant/lingbot-map | 8.3k | 372 | 前馈 3D 场景重建基础模型 |
| altic-dev/FluidVoice | 3.8k | 365 | macOS 离线语音识别 |
| commaai/openpilot | 62.5k | 266 | 自动驾驶系统 |
| browser-use/video-use | 11.2k | 196 | 用编程 Agent 编辑视频 |

---

*Generated by AI Research Briefing Automation*
