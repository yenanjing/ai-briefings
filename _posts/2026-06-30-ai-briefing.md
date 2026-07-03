---
layout: default
title: "AI Research Briefing - 2026-06-30"
date: 2026-06-30 17:45:00 +08:00
---

# AI Research Briefing - 2026-06-30

> 自动生成于 2026-06-30 17:45 CST
>
> arXiv 批次：2026-06-29 提交（25 篇候选，精选 12 篇）
>
> 在线版：https://yenanjing.github.io/ai-briefings/2026/06/30/ai-briefing.html

## 📚 论文精选（12 篇）

### 1. 9.5🌟 Agents-A1: Scaling the Horizon, Not the Parameters
- **机构**: 上海人工智能实验室 (Shanghai AI Lab)
- **作者**: Lei Bai, Bowen Zhou, Dahua Lin 等 49 人
- **arXiv**: [2606.30616](https://arxiv.org/abs/2606.30616)
- **分类**: cs.CL
- **核心创新**: 35B MoE Agent 通过"agent-horizon scaling"（长轨迹 45K token + 异构能力）实现万亿参数级性能。SEAL-0 (56.4)、IFBench (80.6)、HiPhO (46.4) 等多个长程任务榜单对标 Kimi-K2.6/DeepSeek-V4-pro。

### 2. 9.0🌟 VLK: Humanoid Loco-Manipulation from Synthetic Interactions in Reconstructed Scenes
- **作者**: Yen-Jen Wang, Pieter Abbeel, Karen Liu, Guanya Shi, Angjoo Kanazawa, Koushil Sreenath 等
- **arXiv**: [2606.30645](https://arxiv.org/abs/2606.30645)
- **代码**: [vision-language-kinematics.github.io](https://vision-language-kinematics.github.io/)
- **分类**: cs.RO
- **核心创新**: 用 3D Gaussian Splatting 重建室内场景 + 合成 48K 视觉-语言-运动学轨迹训练 VLK 策略，Unitree G1 实机 sim-to-real 验证导航和物体搬运。

### 3. 8.5🌟 LeVo 2: Stable and Melodious Song Generation via Hierarchical Representation Modeling
- **机构**: 腾讯 AI Lab
- **作者**: Shun Lei, Dong Yu, Zhiyong Wu 等
- **arXiv**: [2606.30642](https://arxiv.org/abs/2606.30642)
- **分类**: cs.SD, cs.AI
- **核心创新**: 混合 LLM-Diffusion 框架，LeLM 层次建模（语义规划 + 轨道细化）+ 美学引导训练（SFT/DPO/Online-DPO），全时长歌曲生成接近商用系统。

### 4. 8.3🌟 C²R: Cross-sample Consistency Regularization Mitigates Feature Splitting and Absorption in SAEs
- **作者**: Haoran Jin, Xiting Wang, Shijie Ren, Hong Xie, Defu Lian
- **arXiv**: [2606.30609](https://arxiv.org/abs/2606.30609)
- **代码**: [github.com/hr-jin/Cross-sample-Consistency-Regularization](https://github.com/hr-jin/Cross-sample-Consistency-Regularization)
- **分类**: cs.LG, cs.AI
- **核心创新**: 针对 SAE 大字典下的"特征分裂/吸收"问题，提出跨样本一致性正则化，惩罚方向相似潜在共激活，保持重建保真度的同时提升可解释性。

### 5. 8.2🌟 HOPformer / EPIC-Contact: In-the-wild Egocentric 3D Hand-Object Pose Estimation
- **作者**: Siddhant Bansal, Zhifan Zhu, Shashank Tripathi, Michael J. Black, Dima Damen
- **arXiv**: [2606.30598](https://arxiv.org/abs/2606.30598)
- **代码**: [sid2697.github.io/epic-contact](https://sid2697.github.io/epic-contact)
- **分类**: cs.CV
- **核心创新**: 端到端 transformer 单次前向预测双手-物体 3D 位姿，ARCTIC 82.4% 成功率 (+6.2 pts)。新发布 EPIC-Contact 数据集（2.3K clips, 62.3K frames）含密集双向接触对应。

### 6. 8.0🌟 Goku: Million-Scale Universal Dataset for Instruction-Based Video Editing
- **机构**: 中国科学技术大学 / 快手
- **作者**: Sen Liang, Zhibo Chen 等
- **arXiv**: [2606.30599](https://arxiv.org/abs/2606.30599)
- **分类**: cs.CV
- **核心创新**: 200 万视频编辑对数据集，从单任务外观编辑扩展到多任务/结构操控（主体运动控制）。提出 Goku-Edit 双分支架构（mask 分支控结构 + 主分支渲染外观），Goku-Bench 1000 测试用例 + 7 个新指标，相对开源模型 +8%。

### 7. 7.8🌟 DOPD: Dual On-policy Distillation
- **机构**: 阿里达摩院
- **作者**: Xinlei Yu, Shuicheng Yan 等
- **arXiv**: [2606.30626](https://arxiv.org/abs/2606.30626)
- **分类**: cs.AI
- **核心创新**: 提出"privilege illusion"概念，揭示特权信息输入导致的能力差距 vs 信息不对称差距混淆。优势感知的双蒸馏范式，token 级别动态路由特权教师 vs 特权学生监督信号。

### 8. 7.6🌟 WorldEvolver: Self-Evolving World Models for LLM Agent Planning
- **作者**: Xuan Zhang, Wenxuan Zhang, See-Kiong Ng, Yang Deng
- **arXiv**: [2606.30639](https://arxiv.org/abs/2606.30639)
- **分类**: cs.AI, cs.CL
- **核心创新**: 部署期自演化世界模型，下游 agent 与所有参数冻结。集成情景记忆 + 语义记忆 + 选择性预测三个模块，ALFWorld/Word2World 上 SOTA。

### 9. 7.5🌟 MESA: Prioritizing Vulnerable Communication Channels for Securing Multi-Agent Systems
- **作者**: Kunyang Li, Patrick McDaniel (Wisconsin)
- **arXiv**: [2606.30602](https://arxiv.org/abs/2606.30602)
- **分类**: cs.CR, cs.AI
- **核心创新**: 无标签 MAS 边级安全优先级框架，6 个图论指标 + 2 个动态探针（ablation/masking），监控 Top 10% edges 拦截 3× 攻击。

### 10. 7.4🌟 SPARK: Sequential Planning via Anchored Robotic Keypoints
- **作者**: Bryce Grant, Peng Wang 等 (Case Western)
- **arXiv**: [2606.30613](https://arxiv.org/abs/2606.30613)
- **代码**: [cwru-aism.github.io/spark-page](https://cwru-aism.github.io/spark-page/)
- **分类**: cs.RO
- **核心创新**: 无训练神经符号机器人操控系统，类型化行为树 + 多 prompt 检测 + 恢复循环。LIBERO-PRO 43.7% (2× VLA)，9 个任务 20 次试验平均 68%。

### 11. 7.3🌟 GROW²: Grounding Which and Where for Robot Tool Use
- **机构**: NUS
- **作者**: Yuhong Deng, Yuyao Liu, David Hsu
- **arXiv**: [2606.30632](https://arxiv.org/abs/2606.30632)
- **分类**: cs.RO, cs.AI, cs.CV
- **核心创新**: 开放世界 affordance grounding 框架，语义层（VLM 选工具/部件）+ 几何层（视觉基础模型定位 3D 区域）分层处理，零样本泛化到开放类目物体。

### 12. 7.2🌟 UnfoldArt: Zero-Shot Recovery of Full Articulated 3D Objects from Text or Image
- **机构**: TUM
- **作者**: Mohamed el amine boudjoghra, Ivan Laptev, Angela Dai
- **arXiv**: [2606.30608](https://arxiv.org/abs/2606.30608)
- **分类**: cs.CV
- **核心创新**: 首次 debate-driven agentic 3D 重建方法，高层/低层 agent 围绕全局-局部分歧展开两轮结构化辩论，video generative prior 驱动部件运动以暴露遮挡几何。

## 🚀 GitHub Trending AI 项目（按今日新增 Star）

1. **msitarzewski/agency-agents** — 119.7k⭐ (1,425 today) — 一整套 AI Agency 模板（前端/Reddit/创意等专用 agent）
2. **xbtlin/ai-berkshire** — 7.2k⭐ (1,386 today) — AI 时代伯克希尔价值投资框架，4 大师方法论 + 多 Agent 对抗分析
3. **browser-use/video-use** — 12.2k⭐ (967 today) — 用 coding agent 编辑视频
4. **HKUDS/Vibe-Trading** — 15.5k⭐ (839 today) — 个人交易 Agent
5. **altic-dev/FluidVoice** — 4.6k⭐ (830 today) — macOS 离线语音转文字
6. **commaai/openpilot** — 62.9k⭐ (458 today) — 300+ 车型自动驾驶 OS
7. **cupy/cupy** — 11.9k⭐ (352 today) — GPU 版 NumPy/SciPy
8. **0xNyk/council-of-high-intelligence** — 2.2k⭐ (331 today) — 18 个 AI 人格跨 LLM 多轮协商
9. **refactoringhq/tolaria** — 17.8k⭐ (280 today) — 桌面 markdown 知识库管理
10. **Unclecheng-li/VulnClaw** — 1.3k⭐ (129 today) — AI Agent + MCP 渗透测试工具链
