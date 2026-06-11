

## 2026-06-07 · 📡 今日播报 · Parallight Lab

# 今日 AI 播报

> 按重要性排序，去重合并，聚焦 Agent / RAG / Context Engineering 方向

---

## 🔴 核心基础设施

**1. MemPalace — 当前 benchmark 最优的开源 AI 记忆系统**
定位 agent 的 memory layer，直接影响 RAG 与长期记忆架构选型，优先关注。
→ [github.com/MemPalace/mempalace](https://github.com/MemPalace/mempalace)

**2. khoj-ai/khoj — 自托管 AI second brain（RAG + Agent 完整参考实现）**
支持本地/在线 LLM、自定义 agent、deep research 与自动化调度，是目前最完整的开源 RAG + agent 工程参考。
→ [github.com/khoj-ai/khoj](https://github.com/khoj-ai/khoj)

---

## 🟠 Agent 工程与可靠性

**3. Statewright — 用状态机约束 Agent 行为路径**
以可视化状态机解决 LLM agent 不可预测性，适合生产级 agent 可靠性保障场景。
→ [github.com/statewright/statewright](https://github.com/statewright/statewright)

**4. Rowboat — 多 Agent 系统的开源 IDE**
专为 multi-agent orchestration 设计的集成开发环境，对 agent 编排与 context engineering 实践有直接参考价值。
→ [github.com/rowboatlabs/rowboat](https://github.com/rowboatlabs/rowboat)

---

## 🟡 外部信息获取 / Context Engineering

**5. Agent-Reach — 免 API 费的全网信息获取工具层**
为 agent 提供 Twitter / Reddit / YouTube / GitHub 等多源数据接入，是类 MCP 工具层的实用方案。
→ [github.com/Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach)

**6. last30days-skill — 多源检索与摘要合成的 Agent Skill 示例**
跨 Reddit / X / YouTube / HN 聚合信息，展示 context engineering 中多源信息聚合的典型模式，可直接参考实现。
→ [github.com/mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill)

---

## 🟢 RAG 相关

**7. Code2LoRA — 用超网络动态生成 LoRA 替代 RAG 长上下文注入（论文）**
为代码 LLM 提供仓库级知识注入的新路径，对比 RAG 方案有架构参考价值。
→ [arxiv.org/abs/2606.06492v1](http://arxiv.org/abs/2606.06492v1)

**8. Onyx — 内置 RAG 的开源 Chat UI（YC W24）**
可作为 LLM agent + RAG 应用的快速前端起点，工程落地参考。
→ [news.ycombinator.com/item?id=46045987](https://news.ycombinator.com/item?id=46045987)

---

## ⚪ 延伸关注

**9. HANDOFF — 人形机器人 Planning-Control 接口设计（论文）**
具身 agent 的任务规划与全身控制接口研究，planning → control 的指令传递与蒸馏机制，供具身方向参考。
→ [arxiv.org/abs/2606.06493v1](http://arxiv.org/abs/2606.06493v1)

---

*今日重点：memory layer（MemPalace）+ agent 可靠性（Statewright）+ 外部工具接入（Agent-Reach）三个方向值得优先跟进。*


## 2026-06-07 · 📡 今日播报 · Parallight Lab

# 今日 AI 播报

> 主题聚焦：Agent 架构 · RAG 演进 · 开发工具链

---

## 🔥 重要度 TOP

### 1. Code2LoRA — 用超网络动态生成仓库级 LoRA，挑战 RAG 长上下文方案
为代码 LLM 按仓库动态生成 LoRA adapter，绕开 RAG 注入长上下文的瓶颈，也无需逐仓库微调。是 context engineering 方向值得重点跟踪的新范式。

### 2. MemPalace — 开源 AI 记忆系统，benchmarks 领先
直击 LLM agent 长期记忆与上下文管理的核心痛点，可作为 RAG / 记忆模块的基准参考实现。

### 3. khoj-ai/khoj — 完整 agent+RAG 系统的开源参考实现
自托管 AI second brain，覆盖 web+本地文档 RAG、自定义 agent、定时自动化，兼容主流 LLM，是目前开源 agent 全栈中完整度较高的项目。

---

## ⚙️ Agent 架构与工具链

### 4. Rowboat — 多 agent 系统的开源 IDE（YC S24）
专为构建和调试 multi-agent 系统设计，填补 agent 开发工具链空白，是 agent 调试基础设施的具体实践。

### 5. Statewright — 用可视化状态机约束 agent 行为
以状态机定义 agent 的合法流转路径，解决 LLM agent 不可预测性问题，是 agent 可靠性工程的实用思路。

### 6. HANDOFF — 人形机器人全身控制的分层 agent 架构
解决任务规划与底层执行之间的"命令空间"接口问题，展示 task planning → action 分层 agent 架构在具身 AI 中的落地实践。

---

## 🔌 Agent 外部能力扩展

### 7. Agent-Reach — 给 agent 接入多平台实时检索，零 API 费用
覆盖 Twitter / Reddit / YouTube / GitHub 等平台，即插即用增强 agent 外部感知能力。

### 8. last30days-skill — 跨多源检索合成的 agent skill
跨 Reddit / X / HN / Polymarket 检索并合成摘要，是 agent tool-use + RAG 的典型轻量实现案例。

### 9. Onyx — 开源企业级 Chat UI，内置 RAG 管道（YC W24）
生产级 RAG + chat 架构的参考实现，适合评估企业内部知识库对话方案。

---

**一句话总结**：今日信息密度集中在两条线——**RAG 的替代与增强**（Code2LoRA、MemPalace、Agent-Reach）和 **agent 可靠性与工具链成熟度**（Rowboat、Statewright、HANDOFF），两者正同步推进 agent 系统从原型走向生产。


## 2026-06-07 · 📡 今日播报 · Parallight Lab

# 今日 AI 播报

> 今日主线：**Agent 工程化**全面提速——从记忆、状态管理、多源数据接入到开发工具链，生产级 agent 基础设施正在快速成型。

---

## 🧠 Agent 基础设施

**1. MemPalace — 开源 AI 记忆系统**
当前 benchmark 领先，直接填补 LLM agent 长期记忆空白，可作为 agent context 管理的基础组件优先评估。

**2. Statewright — 用可视化状态机约束 Agent 行为**
通过形式化状态机限制 agent 动作空间，从根源解决 LLM agent 不确定性与失控问题，对生产级 agent 落地有直接参考价值。

**3. AgentScope — 微软系可观测 Agent 框架**
强调可观测性与可信赖性，内置调试与审计能力，适合需要追踪 agent 行为的工程场景。
→ https://github.com/agentscope-ai/agentscope

---

## 🔧 开发工具与 IDE

**4. Rowboat — 多 Agent 系统开源 IDE**
专为多 agent 编排设计，覆盖 agent 定义、调试与协作流程，是目前少见的 agent 原生开发环境。

**5. Code2LoRA — 超网络动态生成仓库级 LoRA 适配器**
为代码 LLM 按仓库动态生成 LoRA，绕开 RAG 长上下文注入的成本与脆弱性，提供 context engineering 的替代路径，值得跟进。

---

## 🌐 Context 扩展与数据接入

**6. Agent-Reach — Agent 多平台实时数据接入 CLI**
零 API 费用接入 Twitter / Reddit / YouTube / GitHub 实时数据，直接扩展 agent 的外部 context 获取能力。

**7. last30days-skill — 多源信息研究 Agent Skill**
聚合 Reddit / X / HN / Polymarket / Web 的 skill 模块，展示了**skill 模块化组合**用于 context 合成的设计范式，可作为 skill 工程的参考模板。

---

## 📦 全栈参考实现

**8. Khoj — 可自托管 AI Second Brain**
支持 web + 本地文档 RAG、自定义 agent、定时自动化，兼容主流 LLM，是 context engineering + agent 全栈的完整参考实现。

**9. Onyx (YC W24) — 开源企业级 Chat UI**
内置 RAG 能力，支持对接多种后端，适合快速搭建企业知识问答系统的团队直接取用。

---

**编辑观察：** 今日 9 条内容几乎全部围绕 agent 工程化展开——记忆（MemPalace）、状态控制（Statewright）、数据接入（Agent-Reach）、开发环境（Rowboat）同日涌现，说明 agent infra 层正在从概念验证加速走向工具标准化阶段。


## 2026-06-07 · 📡 今日播报 · Parallight Lab

# 今日 AI Agent & RAG 播报

> 按重要性排序，去重合并同类项

---

## 🔧 Agent 开发基础设施

**1. Rowboat — 多 Agent 系统开源 IDE**
专为构建和调试 multi-agent 系统设计，覆盖 orchestration 与 context 管理，是目前少见的专项 agent 开发环境。

**2. Statewright — 用状态机约束 Agent 行为**
以可视化状态机建模 agent 控制流，直接针对 LLM 不确定性问题，适合需要可靠性保障的生产场景。

**3. AgentScope — 微软开源 Agent 框架**
强调可观测性与可信赖性，内置调试与审计能力，适合企业级 agent 工程落地。

---

## 🧠 RAG & 记忆系统

**4. MemPalace — 开源 AI 记忆系统**
声称基准测试最优，针对跨会话长期记忆场景，是 RAG/context engineering 的关键基础设施选项。

**5. Khoj — 可自托管 AI 第二大脑**
集文档 RAG、自定义 agent、定时自动化与深度研究于一体，兼容本地/云端多种 LLM，context 场景覆盖最完整。

**6. Onyx — 开源 RAG Chat UI（YC）**
内置 RAG 能力，可接企业知识库，是快速落地对话式 RAG 应用的参考实现。

**7. Code2LoRA — 超网络动态生成仓库级 LoRA**【论文】
用超网络为代码 LLM 按仓库动态生成 LoRA adapter，替代 RAG 长上下文注入，解决代码场景下 RAG 的上下文成本与脆弱性问题。

---

## 🌐 Agent 工具扩展

**8. Agent-Reach — 零费用多平台信息获取 CLI**
为 agent 提供 Twitter/Reddit/YouTube/GitHub/B站/小红书等平台搜索与读取能力，无需 API 费用，扩展外部信息获取边界。

**9. last30days-skill — 多源研究摘要 Agent 插件**
跨 Reddit/X/YouTube/HN/Polymarket 研究并合成摘要，典型的 RAG + agent tool use 实践案例。

---

## 🤖 具身 & 检测前沿

**10. HANDOFF — 人形机器人全身控制 Agent 接口**【论文】
提出任务规划 agent 与底层控制器之间的语义接口，解决 LLM agent 驱动具身机器人的语义鸿沟问题。

**11. AI 文本检测基准 — 人机协同编辑场景**【论文】
覆盖 LLM agent 辅助写作的真实工作流，评估 agent 生成内容的可检测性，对 AI 内容治理有参考意义。
→ [arxiv.org/abs/2606.06481v1](http://arxiv.org/abs/2606.06481v1)

---

**今日重点关注**：Agent 开发工具链正在快速成熟（IDE → 框架 → 状态管理），RAG 基础设施分化为通用记忆系统与垂直场景优化（代码仓库 LoRA）两条路线，值得持续跟踪。


## 2026-06-07 · 📡 今日播报 · Parallight Lab

# 今日 AI 播报

> 主题聚焦：Agent 可靠性 · 记忆与上下文 · 多智能体协调

---

## 🔴 重点关注

**1. Statewright — 用有限状态机约束 Agent 行为**
用可视化状态机（FSM）硬约束 LLM agent 的执行路径，直击 agent 不可预测、难调试的核心痛点。是目前 agent 可靠性工程方向最具工程价值的思路之一。

**2. MemPalace — 开源 AI 记忆系统（benchmark 最优）**
专注解决 LLM agent 长期记忆问题，benchmark 表现当前最优。对 RAG + 记忆管理架构有直接参考价值。

**3. Code2LoRA — 用超网络动态生成仓库级 LoRA Adapter**
为每个代码仓库动态生成专属 LoRA adapter，替代 RAG 长上下文注入或逐仓库微调，对"如何高效压缩 repo 上下文进模型"这一 context engineering 核心问题给出新路径。

---

## 🟠 工具与平台

**4. Rowboat — 多 Agent 系统开源 IDE**
专为构建和调试 multi-agent workflow 设计，填补 agent 编排开发工具的空白，是做 agent 系统工程的基础设施参考。

**5. khoj-ai/khoj — 自托管 AI 第二大脑**
支持文档 RAG、自定义 agent、定时自动化、深度研究，兼容主流 LLM，是 context engineering 完整落地的高质量参考实现。

**6. Agent-Reach — 给 Agent 接入多平台实时信息**
覆盖 Twitter / Reddit / YouTube / GitHub 等多源实时读取，zero API fee，是扩展 agent 外部上下文信息源的实用工具。

**7. Onyx (YC W24) — 开源 RAG Chat UI**
提供可自托管的企业知识库对话前端，内置 RAG 管道，是构建内部知识 agent 的可用底座。

---

## 🟡 研究参考

**8. HANDOFF — 类人机器人任务规划与全身控制的接口设计**
研究如何解耦 agent 的 task-space 与 action-space，对 LLM 驱动具身机器人的架构设计有直接参考价值。

**9. DNQ: Deep Nash Q-Network — 多智能体博弈中的 Nash 均衡学习**
在部分可观测多智能体场景（拍卖、资源分配等）中学习 Nash 均衡策略，是多 agent 竞争与协调的方法论参考。
→ [arXiv](http://arxiv.org/abs/2606.06480v1)

**10. last30days-skill — RAG + Agent Tool 组合实践案例**
跨 Reddit / X / YouTube / HN 多源检索并合成摘要，是 RAG + agent tool 组合的典型工程实践，可直接参考实现模式。

---

**今日主线**：Agent 的核心挑战正在从"能不能用"转向"可不可靠、记不记得、上下文够不够用"——状态机约束、长期记忆、动态 adapter 是当前三条并行的解题路径。


## 2026-06-07 · 📡 今日播报 · Parallight Lab

# 今日 AI 播报

> 主题聚焦：**Agent 可靠性 · RAG 落地 · 记忆与上下文管理**

---

## 🔴 重点关注

**1. Statewright — 用有限状态机约束 AI Agent 行为**
用可视化状态机定义 agent 的合法流转路径，从架构层解决 LLM agent 不可预测、难调试的根本问题。工程落地思路值得重点参考。

**2. MemPalace — 开源 AI 长期记忆系统**
号称 benchmark SOTA，直击 agent 长期记忆这一 context engineering 核心瓶颈。长期记忆方案目前仍是空白，值得跟进其实现机制。

---

## 🟠 值得跟进

**3. Rowboat — Multi-Agent 系统开源 IDE**
专为多 agent 系统构建与调试设计，覆盖编排、context 管理、可观测性，是目前少有的 agent 开发全流程工具。

**4. Code2LoRA — 用超网络为代码仓库动态生成 LoRA Adapter**
替代 RAG 长输入或 per-repo fine-tuning，解决软件持续演化下 context 注入成本高且易碎的问题。技术路径新颖，值得关注。

**5. khoj — 自托管 AI Second Brain（RAG + Agent 全栈）**
支持本地/网络文档 RAG、自定义 agent、定时自动化，是目前最完整的开源 RAG+Agent 参考实现之一。

---

## 🟡 扩展参考

**6. Onyx — 开源企业级 RAG 聊天 UI（YC W24）**
多数据源接入、对话界面完整，是目前较成熟的企业 RAG 落地方案，可作产品形态参考。

**7. Agent-Reach — Agent 多平台信息获取 CLI 工具**
零 API 费用接入 Twitter / Reddit / YouTube / GitHub，解决 agent 实时信息获取的工具层问题。

**8. last30days-skill — 多源 RAG Agent Skill 示例**
跨 Reddit / X / YouTube / HN 研究话题并生成综合摘要，展示如何将多源 RAG 封装为可复用 skill，适合作为 skill 设计的模式参考。

---

**今日主线：** Agent 的三大基础设施正在快速补全——**行为约束（Statewright）、长期记忆（MemPalace）、开发工具链（Rowboat）**，加上 RAG 持续走向工程化落地，整体方向从"能跑"迈向"可靠可维护"。


## 2026-06-08 · 📡 今日播报 · Parallight Lab

# 今日 AI 播报 · 精选

> 聚焦 Agent 架构、记忆系统、工具链三大主线，去重排序如下

---

## 🔴 重要度 ★★★★★

**1. Mempalace — 开源 AI 记忆系统（benchmark 最优）**
直击 RAG/Agent 长期记忆的核心痛点，是当前 context engineering 最值得跟进的基础设施项目。

**2. Statewright — 用可视化状态机约束 Agent 行为**
用有限状态机解决 LLM Agent 不可预测性，提供可靠性工程的系统性思路，对生产级 Agent 部署有直接参考价值。

**3. Rowboat — Multi-Agent 系统开源 IDE**
目前少见的专注 Agent 开发与调试的工具链产品，补全了 Agent 工程化落地的缺失环节。

---

## 🟠 重要度 ★★★★

**4. MemDreamer — 长视频理解的层次图记忆 + Agentic 检索**
本质是视频域的 RAG + Agent 架构，解耦感知与推理的设计对长上下文管理有通用借鉴意义。
[→ arXiv](http://arxiv.org/abs/2606.07512v1)

**5. Hermes-Agent（NousResearch）— "随用户成长"的 Agent 框架**
NousResearch 出品，主打个性化 context 管理与 Agent 架构设计，值得关注其长期记忆与个性化方案。
[→ GitHub](https://github.com/NousResearch/hermes-agent)

**6. Agent-Reach — Agent 的"互联网之眼"**
CLI 工具统一读取 Twitter/Reddit/YouTube/GitHub 等多平台，零 API 费用；是 Agent 外部信息获取层的轻量实用方案。

---

## 🟡 重要度 ★★★

**7. Agentopia — 多 LLM Agent 社会模拟框架**
研究 Agent 能否从社交经验中学习以复现人类行为，对 Agent 长期记忆与社会交互设计有学术参考价值。
[→ arXiv](http://arxiv.org/abs/2606.07513v1)

**8. last30days-skill — 多源信息聚合 Agent Skill**
跨 Reddit/X/YouTube/HN/Polymarket 研究任意话题并合成摘要，展示了 Agent 多源 context 构建的实践范式。

**9. Onyx（YC W24）— 开源企业级 Chat UI + RAG**
支持企业知识库接入，HN 254pts 高热度，适合快速搭建内部知识问答场景。

**10. TurboVec — Rust 实现的高性能向量索引库**
Python 绑定，基于 TurboQuant；RAG 底层检索性能瓶颈的潜在替代方案，适合性能敏感场景评估。
[→ GitHub](https://github.com/RyanCodrai/turbovec)

---

> **今日主线**：Agent 可靠性工程（Statewright）× 记忆系统基础设施（Mempalace、MemDreamer）× 工具链完善（Rowboat、Agent-Reach）三条线同步推进，Agent 工程化正从概念走向系统化落地。


## 2026-06-09 · 📡 今日播报 · Parallight Lab

# 今日 AI Agent 播报

---

## 🔬 研究前沿

**1. LLM 强化学习后训练中的离策略与 Trust-Region 分析**
深入拆解 RL 后训练中的 divergence regularization 问题，直接影响 LLM agent 训练稳定性与效果，是当前 agent 训练方法论的重要参考。
[→ arxiv](http://arxiv.org/abs/2606.09821v1)

**2. Evaluation Cards：AI 评估结果的统一解读层**
解决 leaderboard / model card 等来源结果无法横向比较的痛点，对 agent 与 LLM 评估生态有实际指导意义。
[→ arxiv](http://arxiv.org/abs/2606.09809v1)

**3. OmniGameArena：基于 UE5 的 VLM Agent 统一基准**
覆盖多/单智能体场景，填补 agent 评估协议不一致的空缺，对 benchmark 设计有参考价值。
[→ arxiv](http://arxiv.org/abs/2606.09826v1)

---

## 🛠️ 工程工具

**4. Statewright：用有限状态机约束 Agent 行为**
通过可视化状态机解决 LLM agent 不可预测、难以调试的核心可靠性痛点，可靠性工程方向值得关注。

**5. Rowboat：Multi-Agent 系统的开源 IDE**
专为构建和调试多 agent 系统设计的集成开发环境，工程化 agent 开发流程的实用基础设施。

**6. google/skills：Google 官方 Agent Skills 集合**
覆盖 Google 产品与技术的官方 skill 库，其 skill 规范与接口设计范式值得重点参考。
[→ GitHub](https://github.com/google/skills)

**7. mempalace：开源 AI 记忆系统（benchmark 最优）**
直接对应 RAG / long-term agent memory 的上下文持久化需求，可作为 agent 记忆模块的选型参考。

---

## 🔌 能力扩展

**8. last30days-skill：跨平台话题研究 Agent Skill**
跨 Reddit / X / YouTube / HN / Polymarket 多源合成摘要，展示了 agent skill 模块化设计的实际落地形态。

**9. Agent-Reach：零费用多平台网络感知 CLI**
为 agent 提供 Twitter / Reddit / YouTube / GitHub / B站 / 小红书等平台的上下文感知能力，轻量零 API 费用。

**10. Onyx：内置 RAG 的企业知识库开源 Chat UI**
YC W24 项目，可作为企业内部知识问答基础设施的快速起点。

---

## 📚 学习资源

**11. claude-howto：Claude Code Agent 可视化实践指南**
示例驱动，覆盖基础到高级 agent 开发，含可复用模板，适合快速掌握 agent 上下文工程实践。
[→ GitHub](https://github.com/luongnv89/claude-howto)


## 2026-06-10 · 📡 今日播报 · Parallight Lab

# 今日 AI 播报 · 精选

---

## 🔬 研究前沿

**1. SFT 目标分布设计的统一视角**
重新审视 token-level 监督微调目标，系统梳理噪声轨迹与 prior 不匹配问题，对 LLM agent 对齐与泛化有直接指导意义，是理解 SFT 本质的重要理论工作。
→ [arxiv](http://arxiv.org/abs/2606.11189v1)

**2. EEVEE：首个真实场景下的 Agent 测试时 Prompt 学习框架**
支持多数据集、真实任务流，解决 agent prompt 在分布外场景下的自适应难题，是 context engineering 与 agent 鲁棒性研究的重要参考。
→ [arxiv](http://arxiv.org/abs/2606.11182v1)

**3. 数据新闻 Agent：从原始数据到可验证多模态报道**
端到端多模态 agent 系统设计案例，展示 LLM 在复杂、多步骤真实任务中的工程实践思路。
→ [arxiv](http://arxiv.org/abs/2606.11176v1)

---

## 🛠️ 工具与开源

**4. Google 官方 Agent Skills 集合**
Google 发布覆盖自家产品与技术栈的 agent skills，是理解 skill 规范与 MCP-like 工具封装模式的一手参考，具有标杆价值。

**5. Statewright：用可视化状态机约束 Agent 行为**
通过显式状态机限定 agent 执行路径，直击 LLM agent 不可预测的核心痛点，适合追求生产级可靠性的开发者。

**6. Rowboat：Multi-Agent 系统的开源 IDE**
专为构建与调试多 agent 系统设计，集成 context engineering 与 agent orchestration，是当前稀缺的专用开发工具。

**7. Agent-Reach：零费用的 Agent 全网信息触角**
CLI 工具，免 API 费用打通 Twitter/Reddit/YouTube/GitHub/B站/小红书等多平台，是 agent 外部工具集成的实用参考案例。

**8. last30days-skill：多源 RAG Agent Skill 参考实现**
跨 Reddit/X/YouTube/HN/Polymarket 检索并综合摘要，典型的 multi-source RAG + agent skill 架构，适合参考工具组合设计。

---

## ⚡ 基础设施

**9. turbovec：Rust 实现的高性能向量索引库（含 Python bindings）**
RAG 管道底层检索组件的备选方案，Rust 性能优势明显，值得在高吞吐场景下评测。

**10. Onyx (YC W24)：高热度开源 RAG 聊天 UI**
支持接入多种后端，254 pts 社区热度印证认可度，适合快速搭建企业级 RAG 应用前端。

---

> **今日主线**：Agent 可靠性（状态机约束 + 测试时自适应）× 工具生态成熟（Google skills 标准化 + 专用 IDE）× RAG 基础设施持续优化，三条脉络同步推进。


## 2026-06-11 · 📡 今日播报 · Parallight Lab

# 今日 AI 播报

> 聚焦 Agent 工程、Context 压缩、多源工具链，按重要性排序

---

## 🔬 前沿研究

**1. Doc-to-Atom：长文档压缩为可组合记忆原子**
将长文档蒸馏为轻量"记忆原子"并注入模型参数，提供 RAG 之外的上下文压缩新路线，对长文档理解与多步推理有重要启发。
→ [arxiv](http://arxiv.org/abs/2606.12400v1)

**2. TAHOE：Text-to-SQL 的自动 Hint 优化**
LLM agent 从历史经验中自动提炼优化 hint，解决生产级 Text-to-SQL 的大 schema、方言与用户偏好难题，RAG + Agent 结合的典型落地案例。
→ [arxiv](http://arxiv.org/abs/2606.12387v1)

**3. 多轮对话增量压缩方案**
跨轮记忆共享的增量压缩机制，直接缓解长对话 context 膨胀带来的计算开销，Context Engineering 核心问题的针对性解法。
→ [arxiv](http://arxiv.org/abs/2606.12411v1)

**4. DIRECT：具身 Agent 的 Test-Time Compute 分配**
系统研究 VLM 作为高层规划器时的算力分配策略，揭示盲目扩展的收益递减规律，为 Agent 推理效率优化提供实证参考。
→ [arxiv](http://arxiv.org/abs/2606.12402v1)

---

## 🛠️ 工具与开源

**5. Google 官方 Agent Skills 合集**
Google 发布的官方 skill 规范集，与 MCP 类 tool 标准对齐，代表平台级标准化方向，值得持续跟踪。

**6. Statewright：状态机约束 Agent 行为**
用可视化状态机管控 LLM agent 的行为流转，从架构层面提升可靠性，是解决 agent 不确定性的务实工程思路。

**7. Rowboat：Multi-Agent 开源 IDE**
专为构建与调试多 agent 系统设计的开发环境，填补 agent 工程链路中缺乏专用工具的空白。

**8. last30days-skill：多源研究 Agent Skill**
跨 Reddit/X/YouTube/HN/Polymarket 等平台自动研究并合成摘要，展示 multi-source agent 的实际落地形态，skill 架构设计可直接参考。

---

## 📚 学习资源

**9. claude-howto：Claude Code 可视化实践指南**
从基础概念到高级 agent 的系统化示例，含可复用模板，Context Engineering 实践参考价值较高。

**10. Hands-On-AI-Engineering：RAG/Agent 工程实战合集**
覆盖 RAG、Agent、OCR 等方向的可运行项目集合，适合快速获取工程实现参考。
→ [github](https://github.com/Sumanth077/Hands-On-AI-Engineering)

**11. Onyx (YC W24)：开源 Chat UI**
支持多后端接入与 RAG 集成的对话界面，可作为企业知识库问答前端的参考实现。
