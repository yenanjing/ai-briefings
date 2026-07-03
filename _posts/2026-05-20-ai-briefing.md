---
layout: default
title: "AI Research Briefing - 2026-05-20"
date: 2026-05-20
---

<h1>AI Research Briefing - 2026-05-20</h1>
<p><em>2026年5月20日（周三）| 12 篇精选论文 | 10 个 GitHub Trending 项目</em></p>

<h2>📄 精选论文</h2>

<h3>1🌟 8/10 TIDE: Efficient and Lossless MoE Diffusion LLM Inference with I/O-aware Expert Offload</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Zhiben Chen, Youpeng Zhao, Yang Sui, Jun Wang, Yuzhang Shang</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20179">2605.20179</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: 首个针对 MoE 架构扩散语言模型（dLLM）的推理优化系统。利用扩散解码的时间稳定性，通过 I/O 感知的专家卸载策略，在资源受限设备上实现无损推理，解决了 AR 模型方法在 dLLM 场景下面临的 I/O 开销过高和计算瓶颈问题。</li>
</ul>

<h3>2🌟 7.5/10 From Seeing to Thinking: Decoupling Perception and Reasoning Improves Post-Training of Vision-Language Models</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Juncheng Wu, Hardy Chen, Haoqin Tu, Xianfeng Tang, Freda Shi</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20177">2605.20177</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL, cs.CV</li>
<li><strong>核心创新</strong>: 系统性揭示 VLM 性能瓶颈在视觉感知而非推理能力。提出三阶段解耦后训练范式——视觉感知、视觉推理、文本推理，使用专门化训练数据。证明视觉感知需独立优化且能显著提升整体视觉任务表现。</li>
</ul>

<h3>3🌟 7.5/10 TideGS: Scalable Training of Over One Billion 3D Gaussian Splatting Primitives via Out-of-Core Optimization</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Chonghao Zhong, Linfeng Shi, Hua Chen, Tiecheng Sun, Hao Zhao</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20150">2605.20150</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 突破 3DGS 训练的内存瓶颈，利用训练的稀疏性和轨迹条件特性（每次迭代仅激活当前相机批次可见的高斯），将 GPU 内存作为工作集缓存而非持久参数存储，out-of-core 优化支持单 GPU 训练十亿级 3DGS 原语。</li>
</ul>

<h3>4🌟 7/10 SAGE: Scalable Automatic Gating Ensemble for Confident Negative Harvesting in Fraud Detection</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Sudheer Tubati, Amit Goyal</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20157">2605.20157</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.LG</li>
<li><strong>核心创新</strong>: 针对流媒体刷量欺诈检测中合法边缘案例（超级粉丝、睡眠音乐）与欺诈模式高度相似的问题，提出反事实感知负采样方法，结合 SimHash 分层采样与模块化门控集成，实现高置信度负样本收割。</li>
</ul>

<h3>5🌟 7/10 Not Every Rubric Teaches Equally: Policy-Aware Rubric Rewards for RLVR</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Utkarsh Tyagi, Xingang Guo, MohammadHossein Rezaei, Daniel George, Anas Mahmoud</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20164">2605.20164</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.AI</li>
<li><strong>核心创新</strong>: 揭示 RLVR 中静态 rubric 聚合的根本缺陷——将人类标注重要性与其当前优化信号价值混为一谈，许多重要标准已饱和或过时。提出 policy-aware 动态聚合策略，根据策略当前状态自适应调整各标准的优化权重。</li>
</ul>

<h3>6🌟 6.5/10 ClinSeekAgent: Automating Multimodal Evidence Seeking for Agentic Clinical Reasoning</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Juncheng Wu, Letian Zhang, Yuhan Wang, Haoqin Tu, Hardy Chen</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20176">2605.20176</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: 提出从被动证据消费到主动多模态证据获取的临床 Agent 推理范式。ClinSeekAgent 从原始异构数据源中自动规划、迭代搜索和综合多模态临床证据，更贴近真实临床工作流程。</li>
</ul>

<h3>7🌟 6.5/10 CaMo: Camera Motion Grounded Evaluation and Training for Vision-Language Models</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Hsiang-Wei Huang, Junbin Lu, Kuang-Ming Chen, Jianxu Shangguan, Cheng-Yen Yang</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20165">2605.20165</a></li>
<li><strong>代码</strong>: <a href="https://github.com/hsiangwei0903/CaMo">GitHub</a></li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 揭示现有空间 VLM 缺乏基础相机运动理解能力。提出 Spatial Narrative Score（SNS）评估框架，要求 VLM 生成同时捕捉场景语义和相机运动的空间叙事，用冻结 LLM 进行推理评分，并在训练中引入相机运动基础。</li>
</ul>

<h3>8🌟 6.5/10 KoRe: Compact Knowledge Representations for Large Language Models</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Davide Cavicchini, Fausto Giunchiglia, Jacopo Staiano</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20170">2605.20170</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: 针对知识图谱与 LLM 参数化知识各自局限（KG 不自然但可编辑，LLM 知识不透明难更新），提出紧凑知识表示方法，在知识密集任务上融合 KG 的可读可编辑优势与 LLM 的推理能力，减少幻觉。</li>
</ul>

<h3>9🌟 6.5/10 When Does Model Collapse Occur in Structured Interactive Learning?</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Yuchen Wu, Kangjie Zhou, Weijie Su</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20151">2605.20151</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.LG</li>
<li><strong>核心创新</strong>: 理论分析结构化交互学习中的模型坍缩问题。当模型使用其他模型的合成输出进行持续训练时，数据分布偏离目标群体且训练过程产生相关性，研究精确刻画坍缩发生的条件及其与交互结构的关系。</li>
</ul>

<h3>10🌟 6/10 PixVerve: Advancing Native UHR Image Generation to 100MP with a Large-Scale High-Quality Dataset</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Haojun Chen, Haoyang He, Chengming Xu, Qingdong He, Junwei Zhu</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20147">2605.20147</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 首个大规模高质量超高分辨率 T2I 数据集 PixVerve-95K（95K 张 100MP 图像，覆盖多样场景），配合精心设计的数据管线，推动文本到图像生成从 1K-2K 分辨率跨入原生 100MP 时代。</li>
</ul>

<h3>11🌟 6/10 A Methodology for Selecting and Composing Runtime Architecture Patterns for Production LLM Agents</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Vasundra Srinivasan</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20173">2605.20173</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.AI, cs.SE</li>
<li><strong>核心创新</strong>: 提出「随机-确定性边界」（SDB）作为生产级 Agent 运行时的核心架构原语——由 Proposer、Verifier、Commit、Reject 四部分契约构成。围绕 SDB 组织 Coordination/State/Control 三大关注点，提供可复用的运行时架构模式选择方法论。</li>
</ul>

<h3>12🌟 6/10 MSAVBench: Towards Comprehensive and Reliable Evaluation of Multi-Shot Audio-Video Generation</h3>
<ul>
<li><strong>机构</strong>: 未知</li>
<li><strong>作者</strong>: Yujie Wei, Yujin Han, Zhekai Chen, Yongming Li, Kaixun Jiang</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.20183">2605.20183</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 首个面向多镜头音视频（MSAV）生成的综合评测基准和自适应混合评估框架，覆盖视频、音频、跨模态对齐、叙事连贯四个维度，解决现有基准范围有限、数据多样性和评估管线僵化的痛点。</li>
</ul>

<h2>🔥 GitHub Trending AI 项目</h2>

<table>
<thead><tr><th>#</th><th>项目</th><th>Stars</th><th>描述</th></tr></thead>
<tbody>
<tr><td>1</td><td><a href="https://github.com/obra/superpowers">obra/superpowers</a></td><td>198,600⭐</td><td>Agent 技能框架与软件开发方法论</td></tr>
<tr><td>2</td><td><a href="https://github.com/multica-ai/andrej-karpathy-skills">multica-ai/andrej-karpathy-skills</a></td><td>138,344⭐</td><td>改善 Claude Code 行为的单 CLAUDE.md 文件</td></tr>
<tr><td>3</td><td><a href="https://github.com/msitarzewski/agency-agents">msitarzewski/agency-agents</a></td><td>101,774⭐</td><td>完整 AI 代理机构模板集</td></tr>
<tr><td>4</td><td><a href="https://github.com/microsoft/ai-agents-for-beginners">microsoft/ai-agents-for-beginners</a></td><td>64,473⭐</td><td>AI Agent 入门 12 课</td></tr>
<tr><td>5</td><td><a href="https://github.com/rtk-ai/rtk">rtk-ai/rtk</a></td><td>51,026⭐</td><td>CLI 代理，减少 60-90% LLM token 消耗</td></tr>
<tr><td>6</td><td><a href="https://github.com/HKUDS/CLI-Anything">HKUDS/CLI-Anything</a></td><td>37,818⭐</td><td>让所有软件 Agent 原生化</td></tr>
<tr><td>7</td><td><a href="https://github.com/Alishahryar1/free-claude-code">Alishahryar1/free-claude-code</a></td><td>26,430⭐</td><td>免费使用 Claude Code</td></tr>
<tr><td>8</td><td><a href="https://github.com/tinyhumansai/openhuman">tinyhumansai/openhuman</a></td><td>21,613⭐</td><td>个人 AI 超级智能，私有、简洁</td></tr>
<tr><td>9</td><td><a href="https://github.com/humanlayer/12-factor-agents">humanlayer/12-factor-agents</a></td><td>21,235⭐</td><td>生产级 LLM Agent 的 12 条原则</td></tr>
<tr><td>10</td><td><a href="https://github.com/anthropics/claude-plugins-official">anthropics/claude-plugins-official</a></td><td>20,282⭐</td><td>Anthropic 官方 Claude Code 插件目录</td></tr>
</tbody>
</table>

<h2>📊 今日趋势</h2>
<ul>
<li><strong>Agent 基础设施化</strong>：GitHub Trending 被 Claude Code 生态和 Agent 框架主导（8/10 与 Agent 相关），obra/superpowers 以 19.8 万星领跑</li>
<li><strong>MoE 推理优化</strong>：TIDE 首次解决扩散语言模型 MoE 部署的 I/O 瓶颈</li>
<li><strong>VLM 感知 vs 推理</strong>：两篇论文独立揭示 VLM 瓶颈在感知层而非推理层</li>
<li><strong>3D 视觉规模化</strong>：TideGS 突破 3DGS 单 GPU 十亿级原语训练</li>
<li><strong>RLVR 细节优化</strong>：Policy-aware rubric 奖励揭示静态聚合的盲区</li>
</ul>
