---
layout: default
title: "AI研究简报 2026-03-31"
date: 2026-03-31
---

# 🤖 AI 研究简报

> **时间范围**: 2026-03-31 → 2026-03-31（arXiv 最新批次：2026-03-30 提交）| **论文**: 15 篇 | **GitHub**: 8 个
> 🌐 [在线版](https://yenanjing.github.io/ai-briefings/2026-03-31)

---

## 📑 本期速览

> [!summary] 本期要点
> - 🔥 最高分论文：Adaptive Block-Scaled Data Types（MIT / NVIDIA — LLM 量化新格式）
> - 🌟 重点领域：LLM 量化与推理 / VLA 机器人 / 具身智能 / 图像生成 / AI Agent
> - 📈 GitHub 最热：[hacksider/Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam)（⭐ 86,460）

---

## 📚 arXiv 精选论文

> 筛选范围：`cs.AI` · `cs.LG` · `cs.CL` · `cs.CV` · `cs.RO` · `cs.NE` · `stat.ML`
> 排序：推荐度（高 → 低）

---

### 8🌟 Adaptive Block-Scaled Data Types
- **机构**: Massachusetts Institute of Technology / NVIDIA
- **作者**: Jack Cook, Hyemin S. Lee, Kathryn Le, Junxian Guo, Giovanni Traverso, Anantha P. Chandrakasan, Song Han
- **arXiv**: [2603.28765](https://arxiv.org/abs/2603.28765)
- **代码**: 暂无开源代码
- **分类**: `cs.CL`
- **核心创新**: 针对 NVFP4 量化格式的误差分布缺陷，提出自适应块缩放数据类型（ABSD），动态调整每个块的缩放因子以更好地匹配激活分布，在 LLM 量化中显著优于现有 4-bit 格式。Song Han 是 MIT 高效 AI 领域顶尖学者，NVIDIA 提供硬件侧支持，工程落地价值极高。
- **评分理由**: MIT + NVIDIA 顶级联合团队，Song Han 高 h-index 学者；4-bit 量化是 LLM 推理工程核心，直接影响部署效率。

---

### 8🌟 Pandora: Articulated 3D Scene Graphs from Egocentric Vision
- **机构**: MIT LIDS（信息与决策系统实验室）/ Meta Reality Labs
- **作者**: Alan Yu, Yun Chang, Christopher Xie, Luca Carlone
- **arXiv**: [2603.28732](https://arxiv.org/abs/2603.28732)
- **代码**: 暂无开源代码
- **分类**: `cs.RO`
- **核心创新**: 提出从第一视角视觉构建关节化 3D 场景图的框架 Pandora，能够以机器人自己的视角感知并构建包含物体关节状态的语义地图，显著推进具身智能的环境理解能力。MIT LIDS 在机器人感知与规划方面为顶尖团队，Meta Reality Labs 提供工业验证。
- **评分理由**: MIT + Meta 联合，具身智能核心方向，场景图对机器人操控/导航有极高价值。

---

### 8🌟 Rethinking Language Model Scaling under Transferable Hypersphere Optimization
- **机构**: Microsoft Research
- **作者**: Liliang Ren, Yang Liu, Yelong Shen, Weizhu Chen
- **arXiv**: [2603.28743](https://arxiv.org/abs/2603.28743)
- **代码**: [github.com/microsoft/ArchScale](https://github.com/microsoft/ArchScale)
- **分类**: `cs.LG`
- **核心创新**: 提出超球面优化（Hypersphere Optimization）框架重新审视 LLM 扩展律，证明现有超参数迁移律在该参数化下可以更准确地预测最优学习率和批次大小，为大规模训练提供更精准的扩展理论基础。
- **评分理由**: Microsoft Research 顶级团队，Weizhu Chen 在 LLM 训练优化领域影响力极高；扩展律是当前 LLM 研究最核心议题之一。

---

### 8🌟 Gen-Searcher: Reinforcing Agentic Search for Image Generation
- **机构**: MMLab, 香港中文大学（CUHK）/ UCLA / UC Berkeley
- **作者**: Kaituo Feng, Manyuan Zhang, Shuang Chen, Yunlong Lin, Kaixuan Fan, Yilei Jiang, Hongyu Li, Dian Zheng, Chenyang Wang, Xiangyu Yue
- **arXiv**: [2603.28767](https://arxiv.org/abs/2603.28767)
- **代码**: [github.com/tulerfeng/Gen-Searcher](https://github.com/tulerfeng/Gen-Searcher)
- **分类**: `cs.CV`
- **核心创新**: 提出强化学习驱动的 Agentic 搜索框架，让图像生成模型能够主动检索最新外部知识，突破生成模型"冻结知识"的根本限制，使其能正确处理知识密集型或需实时信息的场景。Xiangyu Yue（MMLab 背景）为领域活跃学者。
- **评分理由**: 将 RAG 思路引入图像生成是重要创新方向；有开源代码加分；Xiangyu Yue 知名研究者。

---

### 7🌟 SHOW3D: Capturing Scenes of 3D Hands and Objects in the Wild
- **机构**: Meta Reality Labs / Yale University
- **作者**: Patrick Rim, Kevin Harris, Braden Copple, Shangchen Han, Xu Xie, Ivan Shugurov, Sizhe An, He Wen, Alex Wong, Tomas Hodan, Kun He
- **arXiv**: [2603.28760](https://arxiv.org/abs/2603.28760)
- **代码**: 暂无开源代码
- **分类**: `cs.CV` · `cs.RO`
- **核心创新**: 构建大规模野外手-物交互 3D 数据集与捕获系统，突破现有数据集仅限受控实验室环境的局限，为手-物操控理解提供真实场景基础数据，推动具身智能感知能力。
- **评分理由**: Meta Reality Labs 主导，数据集工作为社区基础设施，具身智能手部交互方向重要贡献。

---

### 7🌟 SOLE-R1: Video-Language Reasoning as the Sole Reward for On-Robot Reinforcement Learning
- **机构**: 未知机构（Brown University 等推测）
- **作者**: Philip Schroeder, Thomas Weng, Karl Schmeckpeper, Eric Rosen, Stephen Hart, Ondrej Biza
- **arXiv**: [2603.28730](https://arxiv.org/abs/2603.28730)
- **代码**: 暂无开源代码
- **分类**: `cs.RO`
- **核心创新**: 仅以视频-语言模型（VLM）的推理输出作为奖励信号，驱动机器人在线强化学习，无需人工奖励函数设计，实现端到端的机器人学习自动化。验证了 VLM 推理能力可直接转化为高质量机器人学习奖励。
- **评分理由**: VLM 即奖励函数是当前机器人学习的热点思路，创新性强，工程落地价值大。

---

### 7🌟 Dynamic Dual-Granularity Skill Bank for Agentic RL
- **机构**: 中国科学院自动化研究所 / 鹏城实验室 / 中山大学
- **作者**: Songjun Tu, Chengdong Xu, Qichao Zhang, Yaocheng Zhang, Xiangyuan Lan, Linjing Li, Dongbin Zhao
- **arXiv**: [2603.28716](https://arxiv.org/abs/2603.28716)
- **代码**: [github.com/TU2021/D2Skill-AgenticRL](https://github.com/TU2021/D2Skill-AgenticRL)
- **分类**: `cs.AI`
- **核心创新**: 提出双粒度技能库（D2Skill），同时在轨迹级和动作级提取可复用技能，通过动态检索-复用机制大幅提升 Agentic RL 的样本效率和泛化能力，解决了现有技能方法粒度单一的问题。
- **评分理由**: 中国科学院 + 鹏城实验室顶级国内机构；Agentic RL 是当前 AI Agent 研究核心方向，双粒度设计创新。

---

### 7🌟 On-the-fly Repulsion in the Contextual Space for Rich Diversity in Diffusion Transformers
- **机构**: Tel Aviv University / Snap Research
- **作者**: Omer Dahary, Benaya Koren, Daniel Garibi, Daniel Cohen-Or
- **arXiv**: [2603.28762](https://arxiv.org/abs/2603.28762)
- **代码**: 暂无开源代码
- **分类**: `cs.CV` · `cs.AI` · `cs.LG`
- **核心创新**: 针对文本到图像扩散模型"典型性偏差"（生成结果同质化）问题，提出在上下文空间实时排斥（On-the-fly Repulsion）机制，同一 prompt 的多次生成结果多样性大幅提升，无需修改模型权重。Daniel Cohen-Or 是计算机视觉领域国际知名学者。
- **评分理由**: Tel Aviv + Snap 联合，Cohen-Or 高 h-index 学者；图像多样性生成是创意应用核心需求，方法轻量无需重训练。

---

### 7🌟 FocusVLA: Focused Visual Utilization for Vision-Language-Action Models
- **机构**: 哈尔滨工业大学（深圳）/ DaiMon Robotics / 南京大学 / 中国人民大学
- **作者**: Yichi Zhang, Weihao Yuan, Yizhuo Zhang, Xidong Zhang, Jia Wan
- **arXiv**: [2603.28740](https://arxiv.org/abs/2603.28740)
- **代码**: 暂无开源代码
- **分类**: `cs.RO`
- **核心创新**: 发现当前自回归 VLA 模型未能充分利用视觉信息的问题，提出聚焦视觉利用机制（Focused Visual Utilization），通过注意力引导让模型优先处理任务相关视觉区域，在多个机器人操控基准上取得显著提升。
- **评分理由**: VLA 是具身智能前沿，国内顶级高校联合工业团队；视觉利用效率是 VLA 的根本瓶颈之一。

---

### 7🌟 HandX: Scaling Bimanual Motion and Interaction Generation
- **机构**: University of Illinois Urbana-Champaign / Snap Inc.
- **作者**: Zimu Zhang, Yucheng Zhang, Xiyan Xu, Ziyin Wang, Sirui Xu, Kai Zhou, Bing Zhou, Chuan Guo, Jian Wang, Yu-Xiong Wang, Liang-Yan Gui
- **arXiv**: [2603.28766](https://arxiv.org/abs/2603.28766)
- **代码**: 暂无开源代码
- **分类**: `cs.CV`
- **核心创新**: 提出大规模双手动作与交互生成框架，专注于手指细粒度动作、接触时序和双手协同等现有全身模型忽视的关键细节，构建高保真双手序列数据集并训练生成模型，为人机交互和具身智能提供重要基础。
- **评分理由**: UIUC + Snap 学术工业联合，Yu-Xiong Wang 活跃学者；双手交互是具身智能/AR 方向重要缺口。

---

### 6🌟 Stepwise Credit Assignment for GRPO on Flow-Matching Models
- **机构**: Carnegie Mellon University / Adobe Research
- **作者**: Yash Savani, Branislav Kveton, Yuchen Liu, Yilin Wang, Jing Shi, Subhojyoti Mukherjee, Nikos Vlassis, Krishna Kumar Singh
- **arXiv**: [2603.28718](https://arxiv.org/abs/2603.28718)
- **代码**: 暂无开源代码
- **分类**: `cs.LG`
- **核心创新**: 针对 Flow-GRPO 均匀信用分配（忽略时序贡献差异）问题，提出逐步信用分配方法，基于各时间步对最终输出的实际贡献进行差异化权重分配，提升流匹配模型的强化学习训练效率与效果。
- **评分理由**: CMU + Adobe Research 联合；将 GRPO 引入流匹配是当前扩散/生成模型 RLHF 的前沿方向。

---

### 6🌟 Stop Probing, Start Coding: Why Linear Probes and Sparse Autoencoders Fail at Compositional Generalisation
- **机构**: Mila - Québec AI Institute / Université de Montréal
- **作者**: Vitória Barin Pacela, Shruti Joshi, Isabela Camacho, Simon Lacoste-Julien, David Klindt
- **arXiv**: [2603.28744](https://arxiv.org/abs/2603.28744)
- **代码**: 暂无开源代码
- **分类**: `cs.LG`
- **核心创新**: 系统性证明线性探针和稀疏自编码器（SAE）在组合泛化任务上的根本缺陷——它们无法捕获神经网络中非线性组合的语义结构，对可解释性研究社区的方法论有重要警示意义。Simon Lacoste-Julien 为 Mila 知名学者。
- **评分理由**: Mila 顶级可解释性团队；对主流可解释性工具（探针/SAE）的批判性分析影响范围广，方法论贡献重要。

---

### 6🌟 EpiScreen: Early Epilepsy Detection from Electronic Health Records with Large Language Models
- **机构**: University of Minnesota（计算健康科学部 / 理工学院 / 神经科）
- **作者**: Shuang Zhou, Kai Yu, Zaifu Zhan, Huixue Zhou, Min Zeng, Feng Xie, Zhiyi Sha, Rui Zhang
- **arXiv**: [2603.28698](https://arxiv.org/abs/2603.28698)
- **代码**: 暂无开源代码
- **分类**: `cs.CL`
- **核心创新**: 利用 LLM 从电子健康记录（EHR）中早期检测癫痫，解决癫痫与非癫痫性发作（PNES）相似临床表现导致的误诊问题，在真实 EHR 数据上验证了 LLM 在医疗 NLP 中的实用价值。
- **评分理由**: 医疗 AI + LLM 的落地应用，临床价值明确；EHR 处理是 NLP 重要应用方向。

---

### 6🌟 AdaptToken: Entropy-based Adaptive Token Selection for MLLM Long Video Understanding
- **机构**: Microsoft Spatial AI Lab / EPFL / ETH Zurich
- **作者**: Haozhe Qi, Kevin Qu, Mahdi Rad, Rui Wang, Alexander Mathis, Marc Pollefeys
- **arXiv**: [2603.28696](https://arxiv.org/abs/2603.28696)
- **代码**: [haozheqi.github.io/adapt-token](https://haozheqi.github.io/adapt-token)（项目页）
- **分类**: `cs.CV`
- **核心创新**: 提出基于熵的自适应 Token 选择策略（AdaptToken），根据帧间信息熵动态选择关键视觉 token，在保持视频理解准确率的同时大幅降低多模态 LLM 的内存消耗和计算量，有效突破长视频理解瓶颈。
- **评分理由**: ETH Zurich / Marc Pollefeys 在 3D 视觉和多模态领域国际顶尖；长视频理解是当前 MLLM 最重要的扩展方向之一。

---

### 6🌟 SonoWorld: From One Image to a 3D Audio-Visual Scene
- **机构**: University of Maryland, College Park
- **作者**: Derong Jin, Xiyi Chen, Ming C. Lin, Ruohan Gao
- **arXiv**: [2603.28757](https://arxiv.org/abs/2603.28757)
- **代码**: 暂无开源代码
- **分类**: `cs.CV`
- **核心创新**: 提出 Image2AVScene 任务框架及 SonoWorld 系统，从单张图像生成完整 3D 音视觉场景——全景图外绘、3D 导航场景提升、空间音频生成一体化，填补了 3D 沉浸式场景生成中音频维度的空白。
- **评分理由**: UMD Ming C. Lin 计算机图形学领域顶尖学者；音视觉 3D 场景生成是元宇宙/AR/VR 的重要基础，创新任务定义有价值。

---

## 🔥 GitHub Trending

> 排序：Star 总数（高 → 低）｜ 已过滤非AI项目 ｜ 已去重

| 热度 | 项目 | 语言 | 简介 |
|------|------|------|------|
| ⭐ 86,460 | [hacksider/Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam) | Python | 实时人脸替换与一键式视频深度伪造技术 |
| ⭐ 64,592 | [OpenBB-finance/OpenBB](https://github.com/OpenBB-finance/OpenBB) | Python | 面向分析师、量化与 AI Agent 的金融数据平台 |
| ⭐ 30,902 | [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) | Python | 微软出品开源前沿语音 AI 技术 |
| ⭐ 26,440 | [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) | HTML | Claude Code 最佳实践指南 |
| ⭐ 18,828 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | Python | NousResearch 出品的自适应成长型 AI Agent |
| ⭐ 10,215 | [luongnv89/claude-howto](https://github.com/luongnv89/claude-howto) | Python | Claude Code 可视化示例指南（含高级 Agent 模板） |

---

## 🏷️ 关键词索引

**模型与架构**
[[VLA模型]] [[流匹配]] [[扩散Transformer]] [[超球面优化]] [[块缩放量化]] [[稀疏自编码器]]

**研究方向**
[[LLM量化]] [[具身智能]] [[双手交互生成]] [[机器人学习]] [[图像生成]] [[长视频理解]] [[医疗AI]] [[可解释性]]

**关键技术**
[[Agentic搜索]] [[强化学习奖励]] [[双粒度技能库]] [[熵自适应Token]] [[3D场景图]] [[音视觉生成]]

**机构**
[[MIT]] [[Microsoft]] [[中国科学院]] [[Meta Reality Labs]] [[ETH Zurich]] [[EPFL]] [[Tel Aviv University]] [[Mila]] [[UIUC]] [[香港中文大学CUHK]] [[UCLA]] [[UC Berkeley]] [[University of Minnesota]]

---

#AI简报 #2026年 #03月 #arxiv #github-trending
