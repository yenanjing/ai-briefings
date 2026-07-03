---
layout: default
title: "AI Research Briefing - 2026-06-25"
date: 2026-06-25
---

# AI Research Briefing - 2026-06-25

> 自动生成于 2026-06-25 10:55 (CST)

## 论文精选（12 篇）

### 8🌟 OpenThoughts-Agent: Data Recipes for Agentic Models
- **作者**: Negin Raoof, Richard Zhuang 等 50 位作者
- **arXiv**: [2606.24855](https://arxiv.org/abs/2606.24855)
- **代码**: [openthoughts.ai](http://openthoughts.ai)
- **分类**: cs.AI
- **核心创新**: 50 作者团队完成 100+ 受控消融实验，系统研究 Agent 训练数据配方。基于 100K 样本微调 Qwen3-32B，在 7 个 Agent 基准上达 44.8% 平均准确率（超 Nemotron-Terminal 3.9 个百分点），展现强可扩展性。

### 7.8🌟 ReM-MoA: Reasoning Memory Sustains Mixture-of-Agents Scaling
- **作者**: Heng Ping, Arijit Bhattacharjee, Peiyu Zhang 等
- **arXiv**: [2606.24437](https://arxiv.org/abs/2606.24437)
- **分类**: cs.AI
- **核心创新**: 提出记忆增强 MoA 框架，通过排名推理记忆和多样化路由机制，解决深层 MoA 架构性能退化问题。在 5 个推理基准上随深度增加优势扩大，为可扩展多 Agent 推理奠定基础。

### 7.7🌟 SAFARI: Scaling Long Horizon Agentic Fault Attribution via Active Investigation
- **作者**: Chenyang Zhu, Jiayu Yao, Kushal Chawla 等
- **arXiv**: [2606.24626](https://arxiv.org/abs/2606.24626)
- **分类**: cs.AI
- **核心创新**: ICML 2026 Workshop。通过工具增强诊断循环替代线性上下文加载，解决长周期 Agent 故障归因。在 1M token 预算 Who&When 数据集超 SOTA 20%，即使超出原生上下文 5 倍仍保持 0.58 精确率。

### 7.6🌟 LemonHarness Technical Report
- **作者**: Kailong Ren, Fubo Sun, Jiachen Liu 等 21 位作者
- **arXiv**: [2606.24311](https://arxiv.org/abs/2606.24311)
- **分类**: cs.AI
- **核心创新**: 为长周期 Agent 建立显式执行边界，通过结构化工具接口管理文件写入、依赖安装等状态变更操作。Terminal-Bench 2.0 上 GPT-5.5 达 86.52% 准确率，引入时间感知执行机制优化探索/验证平衡。

### 7.5🌟 Governed Shared Memory for Multi-Agent LLM Systems
- **作者**: Yanki Margalit, Nurit Cohen-Inger, Erni Avram, Ran Taig, Oded Margalit
- **arXiv**: [2606.24535](https://arxiv.org/abs/2606.24535)
- **分类**: cs.AI
- **核心创新**: 正式化多 Agent LLM 系统的"车队记忆"问题，识别四大失败模式：未授权泄漏、陈旧传播、矛盾持续、来源崩溃。在生产级多租户服务 MemClaw 上验证，证明长上下文检索不足以支撑生产级多 Agent 记忆治理。

### 7.4🌟 Bayesian Control for Coding Agents
- **作者**: Theodore Papamarkou, Vladislav Smirnov, Viktor Mazanov 等
- **arXiv**: [2606.24453](https://arxiv.org/abs/2606.24453)
- **分类**: cs.AI, cs.CL
- **核心创新**: 将编码 Agent 编排建模为成本敏感的序贯假设检验，贝叶斯控制器维护候选正确性信念，动态决策是否收集更多证据、精炼候选、验证或停止。跨 6 个生成器和 9 个编码基准，验证成本高时贝叶斯控制价值最大。

### 7.3🌟 Block-GTQ: RoPE-Aware Bit Allocation for KV-Cache Quantization
- **作者**: Fengfeng Liang, Yuechen Zhang, Jiaya Jia
- **arXiv**: [2606.24033](https://arxiv.org/abs/2606.24033)
- **代码**: [github.com/JIA-Lab-research/blockgtq](https://github.com/JIA-Lab-research/blockgtq)
- **分类**: cs.LG
- **核心创新**: 发现 RoPE 下 key 对未来注意力 logit 的贡献可分解为二维频率块能量，提出按块分配量化比特。367/367 层对比胜出均匀 TQ-MSE，K2V2 配置下 Llama-3.1-8B NIAH 从 70.6 提升至 97.4。单 H800 GPU 达 3.24× KV 压缩和 1.34× 加速。

### 7.2🌟 CineCap: Structured Reasoning with Spatio-Temporal Anchors for Cinematographic Video Captioning
- **作者**: Xinyu Mao, Yuhui Zeng, Xiaokun Liu 等
- **arXiv**: [2606.24636](https://arxiv.org/abs/2606.24636)
- **代码**: [github.com/Hectormxy/CineCap](https://github.com/Hectormxy/CineCap)
- **分类**: cs.AI
- **核心创新**: 面向电影级视频描述，结合结构化推理与时空锚点，使用全面性、准确性、门控覆盖率奖励的强化学习。构建 472 条人工标注的 CineCap Bench，开源代码、模型和基准。

### 7.1🌟 Probing the Misaligned Thinking Process of Language Models
- **作者**: Kaiwen Zhou, Constantin Venhoff, Jonathan Michala, Xin Eric Wang, William Saunders
- **arXiv**: [2606.24251](https://arxiv.org/abs/2606.24251)
- **分类**: cs.AI
- **核心创新**: 将模型对齐行为分解为 18 个细粒度认知指标，通过线性探针检测内部激活。跨 5 种对齐行为在 OOD 基准达 0.935 AUROC，同时在良性流量保持低假阳性率，为对齐行为细粒度检测提供新方法。

### 7.0🌟 AdversaBench: Automated LLM Red-Teaming with Multi-Judge Confirmation
- **作者**: Khanak Khandelwal (IIT Jodhpur)
- **arXiv**: [2606.24589](https://arxiv.org/abs/2606.24589)
- **代码**: [github.com/khanak0509/AdversaBench](https://github.com/khanak0509/AdversaBench)
- **分类**: cs.AI
- **核心创新**: 端到端红队测试管道，通过 5 种结构化算子变异种子提示，三裁判 + 元裁判机制确认失败。验证跨模型零样本迁移性（Llama 3.1 8B → Llama 3.3 70B），证明攻击利用通用行为模式。

### 6.9🌟 PHANTOM: A Large-Scale Dataset of Multimodal Adversarial Attacks for VLMs
- **作者**: Simone Gallivanone, Hossein Khodadadi, Mauro Dore, Mauro Medda, Nicola Franco
- **arXiv**: [2606.24388](https://arxiv.org/abs/2606.24388)
- **代码**: [huggingface.co/datasets/it4lia/PHANTOM](https://huggingface.co/datasets/it4lia/PHANTOM)
- **分类**: cs.AI
- **核心创新**: 开源 47,524 个多模态对抗样本数据集，覆盖 10 大类 55 子类有害意图。降低对抗研究门槛，为 VLM 鲁棒性评估、防御护栏开发提供标准化资源。

### 6.8🌟 LaGO: Latent Action Guidance for Online Reinforcement Learning
- **作者**: Kuan-Yen Liu, Ren-Jyun Huang, Ti-Rong Wu
- **arXiv**: [2606.24669](https://arxiv.org/abs/2606.24669)
- **分类**: cs.AI
- **核心创新**: ICML 2026 Workshop。将预训练 LLM 作为潜在动作先验软引导在线策略优化，而非直接控制器。在 CLEVR-Robot 成功率从 15.1% 提升至 27.2%，Meta-World 从 2.7% 提升至 15.2%，更强 LLM 提供更有效引导。

## GitHub Trending AI 项目（Top 10）

| 项目 | Stars | 今日新增 | 描述 |
|------|-------|----------|------|
| [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | 202k | 1,178 | 可成长 Agent 框架 |
| [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 19.8k | 3,719 | Agent 视频制作系统 12 管线 52 工具 |
| [google-labs-code/design.md](https://github.com/google-labs-code/design.md) | 17.5k | 619 | Agent 设计规范格式 |
| [JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template) | 19.4k | 692 | 一键 AI 克隆网站 |
| [stablyai/orca](https://github.com/stablyai/orca) | 6.9k | 331 | 并行 Agent ADE |
| [revfactory/harness](https://github.com/revfactory/harness) | 7.8k | 277 | Agent 团队元技能生成 |
| [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | 48.7k | 1,468 | LLM 驱动多市场股票分析 |
| [interviewstreet/hiring-agent](https://github.com/interviewstreet/hiring-agent) | 2.3k | 203 | AI 简历评估 Agent |
| [apple/container](https://github.com/apple/container) | 42.4k | 1,838 | Mac 上运行 Linux 容器 |
| [kunchenguid/no-mistakes](https://github.com/kunchenguid/no-mistakes) | 2.3k | 110 | git push 自动修正 |

## 统计

- **论文总数**: 12 篇精选（来自 arXiv 4 分类 recent 页面约 200 篇候选）
- **开源项目**: 5 个（OpenThoughts-Agent、Block-GTQ、CineCap、AdversaBench、PHANTOM）
- **会议收录**: ICML 2026 × 3（SAFARI、ReM-MoA、LaGO）
- **亮点方向**: Agent 数据配方、多 Agent 记忆治理、KV-Cache 压缩、长周期故障归因
