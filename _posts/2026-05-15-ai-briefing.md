---
layout: default
title: "AI研究简报 2026-05-15"
date: 2026-05-15T10:10:00+08:00
tags: [ai, arxiv, research, github-trending, briefing]
---

<h1>🤖 AI 研究简报 — 2026-05-15</h1>

<p><strong>时间范围</strong>: 2026-05-15 | <strong>论文</strong>: 12 篇精选 | <strong>GitHub</strong>: 10 个</p>

<h2>📑 本期速览</h2>
<ul>
<li>🏆 Top 论文：OpenDeepThink（Bradley-Terry 并行推理，Elo +405）、VGGT-Ω（前馈3D重建规模化）、MeMo 记忆模型</li>
<li>🌟 重点领域：Test-time Compute Scaling · 3D 视觉重建 · Agent 记忆 · 世界模型 · 视频生成</li>
<li>📈 GitHub 今日增长最快：<a href="https://github.com/mattpocock/skills">mattpocock/skills</a>（🔥 +2,987）</li>
</ul>

<h2>📚 arXiv 精选论文</h2>

<h3>1🌟 OpenDeepThink: Parallel Reasoning via Bradley--Terry Aggregation</h3>
<ul>
<li><strong>作者</strong>: Shang Zhou, Wenhao Chai, Kaiyuan Liu, Huanzhi Mao, Qiuyang Mang...</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15177">2605.15177</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.AI</li>
<li><strong>核心创新</strong>: 提出基于群体 Test-time Compute 的并行推理框架，通过 Bradley-Terry 成对比较聚合多候选推理路径的排名。将 Gemini 3.1 Pro 的 Codeforces Elo 提升 +405 分（8 轮约 27 分钟）。相比 pointwise LLM 评判，成对比较更鲁棒且可迁移到弱模型。</li>
</ul>

<h3>2🌟 VGGT-Ω: Scalable Feed-Forward 3D Reconstruction</h3>
<ul>
<li><strong>作者</strong>: Jianyuan Wang, Minghao Chen, Shangzhan Zhang, Nikita Karaev, Johannes Schönberger...</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15195">2605.15195</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 证明前馈 3D 重建模型的质量可随模型和数据规模可预测地扩展。简化 VGGT 架构为单密集预测头 + 多任务监督，引入 register attention 聚合场景信息，大幅提升静态/动态场景重建精度和效率。</li>
</ul>

<h3>3🌟 MeMo: Memory as a Model</h3>
<ul>
<li><strong>作者</strong>: Ryan Wei Heng Quek, Sanghyuk Lee, Alfred Wei Lun Leong, Arun Verma, Alok Prakash...</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15156">2605.15156</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL, cs.AI, cs.LG</li>
<li><strong>核心创新</strong>: 将新知识编码到独立记忆模型中，LLM 参数保持不变。支持跨文档关系建模、抗检索噪声、避免灾难性遗忘，且推理成本与语料库大小无关。可 plug-and-play 接入闭源 LLM。</li>
</ul>

<h3>4🌟 SANA-WM: Efficient Minute-Scale World Modeling</h3>
<ul>
<li><strong>作者</strong>: Haoyi Zhu, Haozhe Liu, Yuyang Zhao, Tian Ye, Junsong Chen...</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15178">2605.15178</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 2.6B 参数开源世界模型，原生支持 1 分钟 720p 视频生成和 6-DoF 相机控制。混合线性注意力（GDN + softmax）、双分支相机控制、两阶段长视频精炼管线，视觉质量可比大模型但效率显著提升。</li>
</ul>

<h3>5🌟 FutureSim: Replaying World Events to Evaluate Adaptive Agents</h3>
<ul>
<li><strong>作者</strong>: Shashwat Goel, Nikhil Chandak, Arvindh Arun, Ameya Prabhu, Steffen Staab...</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15188">2605.15188</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.LG, cs.AI, cs.CL</li>
<li><strong>核心创新</strong>: 构建基于真实世界事件时序回放的仿真评测框架，让 Agent 预测 2026 年 1-3 月世界事件。揭示前沿 Agent 能力差距显著（最佳 25% 准确率），为长期自适应 Agent 评测提供新范式。</li>
</ul>

<h3>6🌟 EntityBench: Entity-Consistent Long-Range Multi-Shot Video Generation</h3>
<ul>
<li><strong>作者</strong>: Ruozhen He, Meng Wei, Ziyan Yang, Vicente Ordonez</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15199">2605.15199</a></li>
<li><strong>代码</strong>: <a href="https://github.com/Catherine-R-He/EntityBench/">GitHub</a></li>
<li><strong>分类</strong>: cs.CV, cs.AI</li>
<li><strong>核心创新</strong>: 140 集（2,491 镜头）的多镜头视频实体一致性基准，从真实叙事媒体构建。三维评测柱：镜头内质量、提示对齐、跨镜头一致性，含 fidelity gate。</li>
</ul>

<h3>7🌟 RAVEN: Real-time Autoregressive Video Extrapolation</h3>
<ul>
<li><strong>作者</strong>: Yanzuo Lu, Ronglai Zuo, Jiankang Deng</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15190">2605.15190</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 将因果自回归视频扩散的 self rollout 重打包为交叉历史端点 + 噪声去噪状态序列。CM-GRPO 将一致性采样步骤重述为条件高斯转移，实现高效长视频实时流生成。</li>
</ul>

<h3>8🌟 ATLAS: Agentic or Latent Visual Reasoning? One Word is Enough</h3>
<ul>
<li><strong>作者</strong>: Ziyu Guo, Rain Liu, Xinyan Chen, Pheng-Ann Heng</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15198">2605.15198</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV, cs.AI, cs.CL</li>
<li><strong>核心创新</strong>: 用单个离散"功能 token"同时充当 agentic 操作和 latent 视觉推理单元，无需视觉监督，统一 agentic 推理的灵活性与 latent 推理的效率。</li>
</ul>

<h3>9🌟 RefDecoder: Enhancing Visual Generation with Conditional Video Decoding</h3>
<ul>
<li><strong>作者</strong>: Xiang Fan, Yuheng Wang, Bohan Fang, Zhongzheng Ren, Ranjay Krishna</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15196">2605.15196</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV, cs.LG</li>
<li><strong>核心创新</strong>: 发现视频 VAE 解码器缺少条件注入导致细节丢失，提出参考条件视频解码器。轻量图像编码器将参考帧映射为高维 token，PSNR 提升 +2.1dB。</li>
</ul>

<h3>10🌟 VGGT-Edit: Feed-forward Native 3D Scene Editing</h3>
<ul>
<li><strong>作者</strong>: Kaixin Zhu, Yiwen Tang, Yifan Yang, Renrui Zhang, Bohan Zeng...</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15186">2605.15186</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV, cs.AI</li>
<li><strong>核心创新</strong>: 前馈原生 3D 场景编辑框架，引入深度同步文本注入对齐语义引导与空间位姿，残差场预测实现文本条件 3D 编辑。</li>
</ul>

<h3>11🌟 Hand-in-the-Loop: Improving Dexterous VLA</h3>
<ul>
<li><strong>作者</strong>: Zhuohang Li, Liqun Huang, Wei Xu, Zhengming Zhu, Nie Lin...</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15157">2605.15157</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.RO, cs.LG</li>
<li><strong>核心创新</strong>: 无缝人机协同纠错方法 HandITL，将人类纠正意图与自主策略执行融合。干预抖动减少 99.8%，抓取失败减少 87.5%。</li>
</ul>

<h3>12🌟 Self-Distilled Agentic Reinforcement Learning</h3>
<ul>
<li><strong>作者</strong>: Zhengxi Lu, Zhiyuan Yao, Zhuowen Han, Zi-Han Wang, Jinyang Wu...</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.15155">2605.15155</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.LG, cs.AI, cs.CL</li>
<li><strong>核心创新</strong>: 将 OPSD 作为门控辅助目标整合到 RL 主干中（SDAR），通过 sigmoid gate 解决多轮 Agent 蒸馏不稳定问题。</li>
</ul>

<h2>🔥 GitHub Trending</h2>

<table>
<thead><tr><th>今日增长</th><th>项目</th><th>语言</th><th>简介</th></tr></thead>
<tbody>
<tr><td>🔥 +2,987</td><td><a href="https://github.com/mattpocock/skills">mattpocock/skills</a></td><td>Shell</td><td>工程师可直接复用的 Claude skills 集合</td></tr>
<tr><td>🔥 +1,879</td><td><a href="https://github.com/rohitg00/agentmemory">rohitg00/agentmemory</a></td><td>TypeScript</td><td>AI Coding Agent 持久化记忆方案</td></tr>
<tr><td>🔥 +1,780</td><td><a href="https://github.com/obra/superpowers">obra/superpowers</a></td><td>Shell</td><td>Agentic skills 框架和软件开发方法论</td></tr>
<tr><td>🔥 +1,715</td><td><a href="https://github.com/ruvnet/RuView">ruvnet/RuView</a></td><td>Rust</td><td>WiFi 信号实时空间智能与生命体征监测</td></tr>
<tr><td>🔥 +1,354</td><td><a href="https://github.com/CloakHQ/CloakBrowser">CloakHQ/CloakBrowser</a></td><td>Python</td><td>反指纹 Chromium，30/30 bot 检测通过</td></tr>
<tr><td>🔥 +1,232</td><td><a href="https://github.com/github/spec-kit">github/spec-kit</a></td><td>Python</td><td>GitHub 官方 Spec-Driven Development 工具包</td></tr>
<tr><td>🔥 +1,128</td><td><a href="https://github.com/supertone-inc/supertonic">supertone-inc/supertonic</a></td><td>Swift</td><td>快速 ONNX 端侧多语言 TTS</td></tr>
<tr><td>🔥 +915</td><td><a href="https://github.com/garrytan/gstack">garrytan/gstack</a></td><td>TypeScript</td><td>Garry Tan 的 Claude Code 设置：23 个角色工具</td></tr>
<tr><td>🔥 +851</td><td><a href="https://github.com/Genymobile/scrcpy">Genymobile/scrcpy</a></td><td>C</td><td>Android 设备显示和控制工具</td></tr>
<tr><td>🔥 +654</td><td><a href="https://github.com/K-Dense-AI/scientific-agent-skills">K-Dense-AI/scientific-agent-skills</a></td><td>Python</td><td>研究/科学/工程/金融 Agent Skills 集合</td></tr>
</tbody>
</table>

<p><em>Generated on 2026-05-15 by AI Research Briefing Automation</em></p>
