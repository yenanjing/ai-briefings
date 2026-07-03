---
layout: default
title: "AI Research Briefing - 2026-06-11"
date: 2026-06-11
---

# AI 研究简报 - 2026-06-11

## 今日亮点

- **Ambient Diffusion Policy** (MIT CSAIL) — 噪声依赖轴限制次优数据贡献，机器人模仿学习新范式
- **DIRECT** (Stanford) — 具身规划器动态计算分配路由，场景上下文感知推理
- **FACTR 2** (CMU) — commodity 机器人臂无专用传感器外部力感知，NEXT 估计

---

## 论文精选（12 篇）

### 7.9🌟 Ambient Diffusion Policy: Imitation Learning from Suboptimal Data in Robotics
- **作者**: Adam Wei, Nicholas Pfaff, Thomas Cohn, Arif Kerem Dayı, Constantinos Daskalakis, Giannis Daras, Russ Tedrake
- **arXiv**: [2606.12365v1](https://arxiv.org/abs/2606.12365v1)
- **分类**: cs.RO, cs.AI
- **核心创新**: 提出从机器人学次优数据进行模仿学习的简单而有原则的方法。通过引入噪声依赖的数据使用新轴来限制次优数据的贡献，解决传统模仿学习中次优演示污染策略的问题。MIT CSAIL Tedrake/Daras 团队出品。

### 7.8🌟 DIRECT: When and Where Should You Allocate Test-Time Compute in Embodied Planners?
- **作者**: Jadelynn Dao, Milan Ganai, Yasmina Abukhadra, Ajay Sridhar, Mozhgan Nasr Azadani, Katie Luo, Clark Barrett, Jiajun Wu, Chelsea Finn, Marco Pavone
- **arXiv**: [2606.12402v1](https://arxiv.org/abs/2606.12402v1)
- **分类**: cs.RO, cs.AI, cs.CV
- **核心创新**: 介绍 DIRECT 路由框架，使用多模态场景上下文为每个提示动态分配计算资源，改进固定模型选择的成功-成本帕累托前沿。Stanford Finn/Finn/Pavone 团队。

### 7.7🌟 FACTR 2: Learning External Force Sensing for Commodity Robot Arms Improves Policy Learning
- **作者**: Steven Oh, Jason Jingzhou Liu, Tony Tao, Philip Han, Kenneth Shaw, Satoshi Funabashi, Ruslan Salakhutdinov, Deepak Pathak
- **arXiv**: [2606.12406v1](https://arxiv.org/abs/2606.12406v1)
- **分类**: cs.RO, cs.AI, cs.LG, eess.SY
- **核心创新**: 提出 Neural External Torque Estimation (NEXT)，一种数据驱动方法，无需任何专用力传感器即可估计外部关节扭矩，为 commodity 机器人臂提供接触丰富的操作能力。CMU Pathak/Salakhutdinov 团队。

### 7.5🌟 World Pilot: Steering Vision-Language-Action Models with World-Action Priors
- **作者**: Zefu Lin, Rongxu Cui, Junjia Xu, Xiaojuan Jin, Wenling Li, Lue Fan, Zhaoxiang Zhang
- **arXiv**: [2606.12403v1](https://arxiv.org/abs/2606.12403v1)
- **分类**: cs.RO
- **核心创新**: 提出 World Pilot VLA 框架，通过 World-Action Model (WAM) 的先验来增强策略。通过潜在转向和动作转向两个互补路径将先验路由到决策链中。

### 7.4🌟 UniIntervene: Agentic Intervention for Efficient Real-World Reinforcement Learning
- **作者**: Haoyuan Deng, Yitong Gao, Yudong Lin, Haichao Liu, Zhenyu Wu, Ziwei Wang
- **arXiv**: [2606.12372v1](https://arxiv.org/abs/2606.12372v1)
- **分类**: cs.RO, cs.LG
- **核心创新**: 代理干预模型，检测非生产性探索并自主恢复策略。通过未来条件的动作值估计和时间值风险评论家，提升真实世界强化学习效率。

### 7.4🌟 APT: Action Expert Pretraining Improves Instruction Generalization of Vision-Language-Action Policies
- **作者**: Kechun Xu, Zhenjie Zhu, Anzhe Chen, Rong Xiong, Yue Wang
- **arXiv**: [2606.12366v1](https://arxiv.org/abs/2606.12366v1)
- **分类**: cs.RO
- **核心创新**: 两阶段训练方法，强调动作专家预训练。从贝叶斯角度将策略分解为语言无关的 Vision-Action (VA) 先验和语言条件的 VLA 似然。HKUST 团队。

### 7.3🌟 Breaking Entropy Bounds: Accelerating RL Training via MTP with Rejection Sampling
- **作者**: Yucheng Li, Huiqiang Jiang, Yang Xu, Jianxin Yang, Yi Zhang, Yizhong Cao, Yuhao Shen, Fan Zhou, Rui Men, Jianwei Zhang, An Yang, Bowen Yu, Bo Zheng, Fei Huang, Junyang Lin, Dayiheng Liu, Jingren Zhou
- **arXiv**: [2606.12371v1](https://arxiv.org/abs/2606.12371v1)
- **分类**: cs.LG, cs.CL
- **核心创新**: Bebop 对 LLM 后训练中 MTP 进行系统研究，揭示 MTP 接受率从根本上受模型熵波动限制，提出使用概率拒绝采样来缓解。微软 Jingren Zhou 团队。

### 7.2🌟 Verifiable Environments Are LEGO Bricks: Recursive Composition for Reasoning Generalization
- **作者**: Hao Xiang, Qiaoyu Tang, Le Yu, Yaojie Lu, Xianpei Han, Ben He, Le Sun, Bowen Yu, Peng Wang, Hongyu Lin, Dayiheng Liu
- **arXiv**: [2606.12373v1](https://arxiv.org/abs/2606.12373v1)
- **分类**: cs.CL
- **核心创新**: RACES 框架，将可验证环境概念化为可递归组装的可组合构建块，通过递归自动化组合实现推理泛化。人大团队。

### 7.1🌟 Which Models Are Our Models Built On? Auditing Invisible Dependencies in Modern LLMs
- **作者**: Sanjay Adhikesaven, Haoxiang Sun, Sewon Min
- **arXiv**: [2606.12385v1](https://arxiv.org/abs/2606.12385v1)
- **分类**: cs.CL
- **核心创新**: ModSleuth 代理系统，从公开工件中递归重建 LLM 依赖图，揭示现代 LLM 开发复杂生态系统中的多跳许可义务和其他问题。Berkeley Sewon Min 团队。

### 7.0🌟 Redesign Mixture-of-Experts Routers with Manifold Power Iteration
- **作者**: Songhao Wu, Ang Lv, Ruobing Xie, Yankai Lin
- **arXiv**: [2606.12397v1](https://arxiv.org/abs/2606.12397v1)
- **分类**: cs.LG, cs.AI, cs.CL
- **核心创新**: 用 Manifold Power Iteration (MPI) 重新设计 MoE 路由器，将每个路由行与相关专家的主奇异方向对齐，提升路由决策质量。清华 Lin/Xie 团队。

### 6.9🌟 ATLAS: Active Theory Learning for Automated Science
- **作者**: Noémi Éltető, Nathaniel D. Daw, Kimberly L. Stachenfeld, Kevin J. Miller
- **arXiv**: [2606.12386v1](https://arxiv.org/abs/2606.12386v1)
- **分类**: cs.LG, cs.AI
- **核心创新**: ATLAS 主动学习框架，用于数据驱动发现可解释行为模型。在强化学习代理的行为恢复问题上测试，Princeton/Flatiron Stachenfeld 团队。

### 6.8🌟 SPEA2⁺: Improved Density Estimation in SPEA2 with Provable Runtime Guarantees
- **作者**: Duc-Cuong Dang, Andre Opris, Dirk Sudholt
- **arXiv**: [2606.12382v1](https://arxiv.org/abs/2606.12382v1)
- **分类**: cs.NE, cs.AI
- **核心创新**: 首次对 SPEA2 进行运行时分析，分析处理支配解的算法组件。提出改进变体 SPEA2⁺，考虑所有成对距离，提供可证明的运行时保证。Sheffield Sudholt 团队。

---

## GitHub Trending（AI 相关）

| 项目 | ⭐ Stars | 语言 | 说明 |
|------|---------|------|------|
| x1xhlol/system-prompts-and-models-of-ai-tools | 139,654 | - | AI 工具系统提示词与模型集合 |
| obra/superpowers | 224,048 | Shell | 代理技能框架和软件开发方法论 |
| harry0703/MoneyPrinterTurbo | 85,475 | Python | AI 大模型一键生成高清短视频 |
| ruvnet/RuView | 73,037 | Rust | WiFi 信号转空间智能/生命体征监测 |
| addyosmani/agent-skills | 52,885 | Shell | AI 编码代理生产级工程技能 |
| luongnv89/claude-howto | 36,711 | Python | Claude Code 可视化示例驱动指南 |
| mvanhorn/last30days-skill | 39,361 | Python | 跨 Reddit/X/YouTube/HN 研究综合 |
| roboflow/supervision | 43,717 | Python | 可重用计算机视觉工具库 |
| apple/container | 30,389 | Swift | Mac 上 Linux 容器工具 |
| phuryn/pm-skills | 15,577 | - | 100+ 代理技能/命令/插件 |

---

## 今日总结

机器人学方向论文集中爆发：MIT CSAIL 的 Ambient Diffusion Policy、Stanford 的 DIRECT、CMU 的 FACTR 2、HKUST 的 APT 等，覆盖模仿学习、具身规划、力感知、VLA 策略等方向。LLM 后训练方面，微软的 Bebop 研究 MTP 拒绝采样加速，人大提出可验证环境递归组合。Agent 框架在 GitHub Trending 持续霸榜。

---

*生成时间: 2026-06-11 15:47 CST*
