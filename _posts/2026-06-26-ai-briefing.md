---
layout: default
title: "AI Research Briefing - 2026-06-26"
date: 2026-06-26 10:55:00 +0800
---

# AI Research Briefing - 2026-06-26

**论文来源**: arXiv API (25 篇候选，精选 12 篇)  
**GitHub Trending**: 10 个 AI 相关项目

---

## 📚 论文精选 (12 篇)

### 8.0🌟 Autoregressive Boltzmann Generators
- **作者**: Danyal Rehman, Charlie B. Tan, Yoshua Bengio, Avishek Joey Bose, Alexander Tong
- **arXiv**: [2606.27361](https://arxiv.org/abs/2606.27361)
- **代码**: [github.com/danyalrehman/autobg](https://github.com/danyalrehman/autobg)
- **分类**: cs.LG, cs.AI
- **核心创新**: 提出自回归 Boltzmann Generator (ArBG) 框架，突破传统基于流的 Boltzmann Generator 在分子系统采样中的表达能力限制。引入 Robin 模型（1.32 亿参数），在 8-residue 系统上将零样本能量误差降低超 60%，由 Yoshua Bengio 共同作者。

### 7.8🌟 Scalable Behavior Cloning with Open Data, Training, and Evaluation
- **作者**: Arthur Allshire, Himanshu Gaurav Singh, Ritvik Singh, Adam Rashid, Hongsuk Choi, David McAllister, Justin Yu, Yiyuan Chen, Huang Huang, Pieter Abbeel
- **arXiv**: [2606.27375](https://arxiv.org/abs/2606.27375)
- **分类**: cs.RO
- **核心创新**: 发布 ABC-130K 数据集（3,500 小时遥操作数据，195 个任务），目前最大的开源机器人遥操作数据集。全栈开源包括硬件设置、训练基础设施和仿真流程，支持 DiT 和 VLA 模型训练，由 Pieter Abbeel 共同作者。

### 7.7🌟 Reinforcement Learning without Ground-Truth Solutions can Improve LLMs
- **作者**: Yingyu Lin, Qiyue Gao, Nikki Lijing Kuang, Xunpeng Huang, Kun Zhou, Tongtong Liang, Zhewei Yao, Yi-An Ma, Yuxiong He
- **arXiv**: [2606.27369](https://arxiv.org/abs/2606.27369)
- **分类**: cs.LG
- **核心创新**: 提出 RiVER 框架，在无标准答案的评分优化任务上训练 LLM，使用执行反馈作为连续监督。解决尺度主导和频率主导问题，Qwen3-8B 和 GLM-Z1-9B 在 ALE 评级上分别提升 8.9% 和 9.4%，且效果可迁移到精确解基准。

### 7.6🌟 Paying More Attention to Visual Tokens in Self-Evolving Large Multimodal Models
- **作者**: Shravan Venkatraman, Ritesh Thawkar, Omkar Thawakar, Rao Muhammad Anwer, Hisham Cholakkal, Salman Khan, Fahad Khan
- **arXiv**: [2606.27373](https://arxiv.org/abs/2606.27373)
- **代码**: [mbzuai-oryx.github.io/VISE](https://mbzuai-oryx.github.io/VISE)
- **分类**: cs.CV
- **核心创新**: 提出 VISE 框架解决自进化多模态模型的视觉欠条件化问题。通过几何不变性和语义不变性两种奖励直接正则化视觉条件策略。在 Qwen3-VL-2B 上 COCO CIDEr 提升 +16.85，TextCaps +19.66，物体幻觉减少 5.0 Chair-I 点。

### 7.5🌟 DanceOPD: On-Policy Generative Field Distillation
- **作者**: Wei Zhou, Xiongwei Zhu, Zelin Xu, Bo Dong, Lixue Gong, Yongyuan Liang, Meng Chu, Leigang Qu, Lingdong Kong, Wei Liu
- **arXiv**: [2606.27377](https://arxiv.org/abs/2606.27377)
- **分类**: cs.CV, cs.CL, cs.LG
- **核心创新**: 针对 Flow Matching 模型多能力组合冲突问题，提出 DanceOPD 框架。将每个能力定义为流状态空间上的速度场，学生模型从自身 rollout 状态查询各能力场进行蒸馏。在 T2I、编辑、CFG 吸收等任务上验证有效。

### 7.4🌟 PhysiFormer: Learning to Simulate Mechanics in World Space
- **作者**: Yiming Chen, Yushi Lan, Andrea Vedaldi
- **arXiv**: [2606.27364](https://arxiv.org/abs/2606.27364)
- **代码**: [yimingc9.github.io/physiformer](https://yimingc9.github.io/physiformer)
- **分类**: cs.CV
- **核心创新**: 提出 PhysiFormer 扩散 Transformer，直接在世界坐标系预测 3D 物体顶点轨迹。无需显式刚性约束或因果归纳偏置，通过单一去噪扩散过程实现物理合理运动。支持刚性和弹性力学，可泛化到未见真实几何和更大物体数量。

### 7.3🌟 Ask, Solve, Generate: Self-Evolving Unified Multimodal Understanding and Generation
- **作者**: Ritesh Thawkar, Shravan Venkatraman, Omkar Thawakar, Abdelrahman Shaker, Fahad Khan, Hisham Cholakkal, Salman Khan, Rao Muhammad Anwer
- **arXiv**: [2606.27376](https://arxiv.org/abs/2606.27376)
- **分类**: cs.CV
- **核心创新**: 无需人工标注或外部奖励模型的多模态自进化训练框架。三角色设计（提议者、求解者、生成器），引入基于 token 预测不确定性的连续难度信号 STE。在 BLIP3o、BAGEL、VARGPT 三种架构上验证，MMMU 提升 3.5%，GenEval 从 82% 到 85%。

### 7.2🌟 VibeAct: Vibration to Actions for Contact-Rich Reactive Robot Dexterity
- **作者**: Yuemin Mao, Uksang Yoo, Jean Oh, Jonathan Francis, Jeffrey Ichnowski
- **arXiv**: [2606.27344](https://arxiv.org/abs/2606.27344)
- **代码**: [vibeact.github.io](https://vibeact.github.io/)
- **分类**: cs.RO
- **核心创新**: 利用压电麦克风实现高带宽振动感知机器人灵巧操作。通过数字孪生自动标注接触和打滑，训练触觉估计器从真实波形预测接触状态。在抓取、手中重定位和插入任务上超越本体感知+点云基线，成功迁移到真实机器人平台。

### 7.1🌟 RoPEMover: Depth-Aware Object Relocation via Positional Embeddings
- **作者**: Ipek Oztas, Duygu Ceylan, Aybars Bugra Aksoy, Aysegul Dundar
- **arXiv**: [2606.27332](https://arxiv.org/abs/2606.27332)
- **分类**: cs.CV
- **核心创新**: 利用扩散 Transformer 的 RoPE 位置编码实现深度感知物体运动。将 2D RoPE 扩展为深度感知公式，将 6D Plucker 坐标注入自注意力的查询和键。仅增加不到 0.1% 参数，零初始化，支持大位移保持物体身份和场景一致性更新。

### 7.0🌟 Hallucination in World Models is Predictable and Preventable
- **作者**: Nicklas Hansen, Xiaolong Wang
- **arXiv**: [2606.27326](https://arxiv.org/abs/2606.27326)
- **代码**: [nicklashansen.com/mmbench2](https://www.nicklashansen.com/mmbench2)
- **分类**: cs.LG, cs.CV, cs.RO
- **核心创新**: 发布 MMBench2 数据集（427 小时、210 个任务），训练 3.5 亿参数世界模型。识别三种幻觉模式（感知、动作边缘化、场景发散），开发覆盖率感知采样技术和好奇心奖励数据收集方法。仅需 50 条真实轨迹即可高效微调适应未见环境。

### 6.9🌟 Empowering GUI Agents via Autonomous Experience Exploration
- **作者**: Tianyi Men, Zhuoran Jin, Pengfei Cao, Yubo Chen, Kang Liu, Jun Zhao
- **arXiv**: [2606.27330](https://arxiv.org/abs/2606.27330)
- **分类**: cs.CL, cs.AI, cs.CV, cs.LG
- **核心创新**: 提出 PEEU 方法通过自主经验探索和事后经验利用提升小型 MLLM 的 GUI 规划能力。引入 TDHAF 框架研究组合泛化三层粒度。7B 模型达到 30.6% 准确率，超越更大的 Qwen2.5-VL-32B 模型。

### 6.8🌟 World Action Models Enable Continual Imitation Learning
- **作者**: Manish Kumar Govind, Dominick Reilly, Smit Patel, Hieu Le, Srijan Das
- **arXiv**: [2606.27374](https://arxiv.org/abs/2606.27374)
- **分类**: cs.RO, cs.CV
- **核心创新**: 提出 REGEN（递归生成重放）持续模仿学习框架，利用世界动作模型合成伪重放轨迹。无需存储原始人类演示即可实现持续学习，相对顺序微调减少灾难性遗忘 50%，接近需要真实重放数据的上界方法。

---

## 🔥 GitHub Trending (AI 相关)

| 项目 | ⭐ Stars | 今日 | 描述 |
|------|---------|-----|------|
| [garrytan/gstack](https://github.com/garrytan/gstack) | 115.9k | 767 | Garry Tan 的 Claude Code 工具栈，23 个工具覆盖多角色 |
| [opendatalab/MinerU](https://github.com/opendatalab/MinerU) | 69.7k | 644 | PDF/Office 文档转 LLM-ready markdown/JSON |
| [apple/container](https://github.com/apple/container) | 43.3k | 1,351 | macOS Linux 容器工具，Apple Silicon 优化 |
| [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) | 60.7k | 287 | Claude Code 最佳实践指南 |
| [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 22.3k | 3,434 | 开源 Agent 视频制作系统 |
| [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | 21.3k | 571 | 817 个结构化网络安全技能 |
| [JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template) | 20.6k | 1,024 | 一条命令克隆任意网站 |
| [alibaba/page-agent](https://github.com/alibaba/page-agent) | 19.9k | 163 | 页面内 GUI Agent |
| [google-labs-code/design.md](https://github.com/google-labs-code/design.md) | 19.5k | 1,475 | DESIGN.md 格式规范 |
| [NanmiCoder/MediaCrawler](https://github.com/NanmiCoder/MediaCrawler) | 52.9k | 398 | 多平台社交媒体爬虫 |

---

## 📊 统计

- **论文总数**: 12 篇精选（来自 25 篇候选）
- **GitHub AI 项目**: 10 个
- **亮点方向**: 
  - 自回归 Boltzmann Generator (Bengio)
  - 机器人行为克隆 (Pieter Abbeel)
  - 无监督 LLM RL (RiVER)
  - 多模态自进化 (VISE)
  - 世界模型幻觉研究 (MMBench2)
