---
layout: default
title: "AI Research Briefing - 2026-05-29"
date: 2026-05-29
tags: [AI, daily-briefing]
---

<h1>AI Research Briefing - 2026-05-29</h1>

<p><em>自动生成于 2026-05-29 | arXiv export API 限流，使用 4 分类 recent 页面 fallback，约 200 篇候选</em></p>

<h2>📄 今日论文精选（12 篇）</h2>

<h3>1⭐ 9🌟 RL 训练招募功能性福利轴：语言模型内部表征的系统性发现</h3>
<ul>
<li><strong>机构</strong>: NYU</li>
<li><strong>作者</strong>: Andy Q. Han, David J. Chalmers, Pavel Izmailov</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.30232">2605.30232</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.LG</li>
<li><strong>核心创新</strong>: 发现 RL 训练招募的是语言模型中<strong>预存在的功能性福利表征轴</strong>（functional welfare axis），而非创造新的。在语义中性的迷宫环境中训练多个 LLM 后，提取的"惩罚向量"表现出负面福利表征特征：促进失败/不可能 token、对齐负面情绪、负向追踪目标达成，且能诱导病理性回溯和拒绝行为。奖励向量是其镜像，二者近乎反平行。该轴在 RL 训练前就已存在，控制 tile-to-reward 映射、scale、模型族、LoRA vs 全参微调后效应依然稳健，对可解释性和对齐研究具有深远启示。</li>
</ul>

<h3>2⭐ 8.5🌟 RiM：解锁大语言模型工作记忆的隐式推理</h3>
<ul>
<li><strong>机构</strong>: JKU Linz / EPU</li>
<li><strong>作者</strong>: Lukas Aichberger, Sepp Hochreiter</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.30343">2605.30343</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: 受人类认知中工作记忆机制的启发，提出 <strong>Reasoning in Memory (RiM)</strong>，用固定记忆块（memory blocks）替代自回归生成中间推理步骤。记忆块是特殊 token 的固定序列，可在单次前向传播中处理，实现计算高效的隐式推理。采用两阶段课程学习：先逐步预测显式推理步骤（grounding），再丢弃步骤级监督迭代精炼最终答案。在多个模型族和规模上匹配或超越现有隐式推理方法。</li>
</ul>

<h3>3⭐ 8.5🌟 STV：自训练验证突破推理模型自改进瓶颈</h3>
<ul>
<li><strong>机构</strong>: CMU</li>
<li><strong>作者</strong>: Chen Henry Wu, Aditi Raghunathan</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.30290">2605.30290</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.LG</li>
<li><strong>核心创新</strong>: 针对推理模型自改进的<strong>验证器瓶颈</strong>（V-R 循环停滞、自训练引入错误数据），提出 <strong>Self-Trained Verification (STV)</strong>。核心观察：模型虽无法独自捕获自身错误，但在参考答案辅助下可以。利用这种不对称性将"更知情版本"的判断作为监督目标训练验证器。测试时 STV 大幅改善 V-R 循环：数学难题准确率翻倍，科学推理从 1.5% 提升至 21%（14 倍）。训练时结合 ViL（verifier-in-the-loop），pass@1 额外提升 33%，无验证器的独立 pass@1 相对提升 30%。</li>
</ul>

<h3>4⭐ 8.4🌟 minWM：全栈开源实时交互式视频世界模型框架</h3>
<ul>
<li><strong>机构</strong>: 未知机构</li>
<li><strong>作者</strong>: Min Zhao, Hongzhou Zhu, Bokai Yan 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.30263">2605.30263</a></li>
<li><strong>代码</strong>: 开源（链接待补充）</li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 提出端到端流水线，将现有双向 T2V/TI2V 视频基础模型转换为<strong>相机可控的少步自回归世界模型</strong>。框架涵盖相机控制微调 → Causal Forcing / Causal Forcing++ 管线（AR 扩散训练、因果 ODE 或一致性蒸馏、非对称 DMD）→ 少步自回归生成器。在 Wan2.1-T2V-1.3B 和 HY1.5-TI2V-8B 上实例化，支持 cross-attention 和 MMDiT 架构，可适配已有世界模型到新数据分布和延迟目标。+1🌟 开源</li>
</ul>

<h3>5⭐ 8🌟 EFC：Agent Harness 的有效反馈计算 Scaling Law</h3>
<ul>
<li><strong>机构</strong>: 未知机构</li>
<li><strong>作者</strong>: Xuanliang Zhang, Dingzirui Wang, Keyan Xu 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.29682">2605.29682</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: 提出 <strong>Effective Feedback Compute (EFC)</strong> 作为 Agent Harness 的 Scaling 新坐标，只计算"信息丰富、有效、非冗余且被后续决策保留"的反馈。在合成可控任务、代码执行任务、真实 benchmark trace 和前瞻验证批次上，EFC 一致预测失败率优于 raw compute（R²=0.33/0.42 vs SAS=0.88 vs EFC=0.94, Oracle-EFC/D_task=0.99）。关键发现：harness scaling 由"原始预算转换为持久任务充分反馈的效率"决定，而非计算总量。</li>
</ul>

<h3>6⭐ 8🌟 AgentDoG 1.5：轻量可扩展的 Agent 安全对齐框架</h3>
<ul>
<li><strong>机构</strong>: 未知机构</li>
<li><strong>作者</strong>: Dongrui Liu, Yu Li, Zhonghao Yang 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.29801">2605.29801</a></li>
<li><strong>代码</strong>: 开源（链接待补充）</li>
<li><strong>分类</strong>: cs.AI</li>
<li><strong>核心创新</strong>: 更新 Agent 安全分类体系以覆盖 Codex/OpenClaw 执行场景的新兴风险，构建 taxonomy-guided 数据引擎配合影响函数净化，仅需约 1k 样本训练 0.8B-8B 参数变体，性能可比 GPT-5.4。构建高效 SFT/RL 训练环境，部署开销降低两个数量级，并可作为无训练在线护栏。+1🌟 开源</li>
</ul>

<h3>7⭐ 8🌟 CRITIC-R1：结构化批评者框架改进 RAG</h3>
<ul>
<li><strong>机构</strong>: 未知机构</li>
<li><strong>作者</strong>: Wenhan Xiao, Ziwei Zhang, Chuanyue Yu 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.29886">2605.29886</a></li>
<li><strong>代码</strong>: 开源（链接待补充）</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: 将 RAG 批评学习为显式<strong>错误诊断问题</strong>，使用 RL 训练结构化批评者。将常见 RAG 错误分为多个诊断维度（判定、错误定位、推理分析、修复生成）。设计两阶段奖励函数：CJA 先鼓励校准的高层判断缓解过度干预，DQA 通过门控奖励进一步改善细粒度诊断。使用 GRPO-based RL 配合外部 LLM 教师模型的过程级监督训练。+1🌟 开源</li>
</ul>

<h3>8⭐ 7.5🌟 LoRA 记忆定律：参数化记忆的定量刻画与阈值引导优化</h3>
<ul>
<li><strong>机构</strong>: 未知机构</li>
<li><strong>作者</strong>: Ziwen Xu, Haiwen Hong, Linsong Yu 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.30260">2605.30260</a></li>
<li><strong>代码</strong>: 代码将发布（链接待补充）</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: 首次系统量化 LoRA 的<strong>精确参数化记忆容量</strong>，发现<strong>参数化记忆定律</strong>：损失减少 ΔL 与有效参数和序列长度遵循幂律关系。细粒度分析揭示确定性相变：预测概率 p > 0.5 构成贪婪解码下逐字回忆的充分条件。基于此提出 MemFT，动态将训练预算重新分配给未达阈值 token。</li>
</ul>

<h3>9⭐ 7.5🌟 双路径架构：灵活缩放 LLM 的计算与容量</h3>
<ul>
<li><strong>机构</strong>: SAP</li>
<li><strong>作者</strong>: Markus Frey, Behzad Shomali, Joachim Koehler 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.30202">2605.30202</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: 提出 <strong>Dual-Path Block</strong>，在单层内同时暴露"计算"（深度子层共享参数复用 K 次）和"容量"（宽子层扩大 FFN 应用一次）两个轴。独立 per-token 门控组合两个路径，可学习的门具有直接可解释性：功能词和词汇内容趋向宽路径，标点/符号/算术 token 趋向深路径。</li>
</ul>

<h3>10⭐ 7.5🌟 MMPO：元认知记忆策略优化</h3>
<ul>
<li><strong>机构</strong>: 未知机构</li>
<li><strong>作者</strong>: Ziyan Liu, Zhezheng Hao, Yeqiu Chen 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.30159">2605.30159</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.AI</li>
<li><strong>核心创新</strong>: 针对 LLM Agent 长时任务中递归摘要逐步丢失任务相关信息的问题，提出 <strong>Belief Entropy</strong> 自监督代理——探测模型在当前记忆下对潜在任务状态的不确定性。基于此提出 <strong>MMPO</strong>，通过显式惩罚高认识不确定性摘要提供细粒度记忆级监督。1.75M token 上下文下保持 97.1% 性能。</li>
</ul>

<h3>11⭐ 7.5🌟 EvoRubric：自进化标准驱动的开放域 RL 对齐</h3>
<ul>
<li><strong>机构</strong>: 未知机构</li>
<li><strong>作者</strong>: Xin Guan, Xiaomeng Hu, Shen Huang 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.29847">2605.29847</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CL</li>
<li><strong>核心创新</strong>: <strong>单策略协同进化 RL 框架</strong>，消除对静态人类标注标准和外部 LLM 标准生成器的依赖。统一响应生成和标准生成于单一策略，动态交替 Reasoner 和 Rubric Generator。引入多层验证管线（元验证器 + 零方差剪枝 + Leave-One-Out 同行共识）防止奖励黑客。在医疗、写作、科学领域持续超越传统方法。</li>
</ul>

<h3>12⭐ 7.5🌟 VideoMLA：分钟级自回归视频扩散的低秩隐式 KV 缓存</h3>
<ul>
<li><strong>机构</strong>: 未知机构</li>
<li><strong>作者</strong>: Hidir Yesiltepe, Jiazhen Hu, Tuna Han Salih Meral 等</li>
<li><strong>arXiv</strong>: <a href="https://arxiv.org/abs/2605.30351">2605.30351</a></li>
<li><strong>代码</strong>: 暂无</li>
<li><strong>分类</strong>: cs.CV</li>
<li><strong>核心创新</strong>: 首次在视频扩散中研究 <strong>Multi-Head Latent Attention (MLA)</strong>，用共享低秩内容隐式和 3D-RoPE 位置键替代逐头 KV，每层每 token KV 内存减少 92.7%。揭示重要理论发现：预训练视频注意力本身不是低秩的，但 MLA 瓶颈（而非预训练谱）决定了有效秩。VBench 上匹配短程基线，长程最佳，单 B200 吞吐提升 1.23×。</li>
</ul>

<h2>🔥 GitHub Trending AI 项目（Top 10）</h2>

<table>
<thead><tr><th>#</th><th>项目</th><th>描述</th><th>⭐ Stars</th></tr></thead>
<tbody>
<tr><td>1</td><td><a href="https://github.com/obra/superpowers">obra/superpowers</a></td><td>Agentic skills framework & 软件开发方法论</td><td>211,236</td></tr>
<tr><td>2</td><td><a href="https://github.com/affaan-m/ECC">affaan-m/ECC</a></td><td>Agent harness 性能优化系统</td><td>197,425</td></tr>
<tr><td>3</td><td><a href="https://github.com/anthropics/skills">anthropics/skills</a></td><td>Anthropic 官方 Agent Skills 仓库</td><td>142,944</td></tr>
<tr><td>4</td><td><a href="https://github.com/microsoft/markitdown">microsoft/markitdown</a></td><td>Python 文件转 Markdown 工具</td><td>127,895</td></tr>
<tr><td>5</td><td><a href="https://github.com/unclecode/crawl4ai">unclecode/crawl4ai</a></td><td>开源 LLM 友好 Web 爬虫</td><td>67,019</td></tr>
<tr><td>6</td><td><a href="https://github.com/harry0703/MoneyPrinterTurbo">harry0703/MoneyPrinterTurbo</a></td><td>AI 一键生成高清短视频</td><td>66,781</td></tr>
<tr><td>7</td><td><a href="https://github.com/Lum1104/Understand-Anything">Lum1104/Understand-Anything</a></td><td>代码转交互式知识图谱</td><td>43,050</td></tr>
<tr><td>8</td><td><a href="https://github.com/twentyhq/twenty">twentyhq/twenty</a></td><td>AI 时代开源 CRM（Salesforce 替代）</td><td>47,917</td></tr>
<tr><td>9</td><td><a href="https://github.com/Leonxlnx/taste-skill">Leonxlnx/taste-skill</a></td><td>提升 AI 审美品味</td><td>26,661</td></tr>
<tr><td>10</td><td><a href="https://github.com/EveryInc/compound-engineering-plugin">EveryInc/compound-engineering-plugin</a></td><td>Claude Code/Codex 复合工程插件</td><td>17,811</td></tr>
</tbody>
</table>

<h2>📊 今日趋势</h2>
<ul>
<li><strong>Agent 基础设施</strong>占据 GitHub 热榜 6/10 席位，Agent 工程化进入爆发期</li>
<li><strong>RL 对齐</strong>持续深化：STV 突破验证器瓶颈、EvoRubric 自进化标准、CRITIC-R1 结构化批评</li>
<li><strong>视频世界模型</strong>框架化：minWM 全栈开源、VideoMLA 效率突破</li>
<li><strong>LLM 推理机制</strong>新发现：RiM 工作记忆隐式推理、福利轴预存在性、LoRA 记忆定律</li>
<li><strong>Scaling Law</strong>扩展至 Agent Harness：EFC 证明反馈质量 > 计算总量</li>
</ul>
