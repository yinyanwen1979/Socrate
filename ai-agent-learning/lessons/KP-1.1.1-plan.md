---
title: "Agent vs Assistant 区别"
kp_id: "KP-1.1.1"
chapter: "Chapter 1: AI Agent 基础概念"
difficulty: "easy"
estimated_time: "30min"
generated_date: "2026-04-24"
---

# UbD Lesson Plan: KP-1.1.1 — Agent vs Assistant 区别

## Stage 1: Desired Results（预期结果）

### Enduring Understandings（持久理解）

1. **AI Agent 与 AI Assistant 本质上是不同的设计范式** —— Assistant 被动响应，Agent 主动行动
2. **"自主性"是 Agent 的核心特征** —— 能自主设定目标、规划路径、执行多步任务
3. **工具调用和多步推理使 Agent 能够处理复杂、开放式任务**，而 Assistant 通常处理单轮请求

### Essential Questions（核心问题）

1. 为什么 Siri、ChatGPT 这些工具叫"助手"而不是"代理"？两者在行为上有什么区别？
2. 一个真正自主的 AI Agent 需要具备哪些"能力"？这些能力目前 AI 已经达到了吗？
3. 如果让 Agent 自主在互联网上搜集信息并写报告，它和传统搜索引擎有什么本质不同？

### SWBAT（学生将能够）

1. **区分** AI Assistant（被动问答式）和 AI Agent（主动行动式）在交互模式上的差异
2. **解释** Agent 区别于 Assistant 的三个关键特征：目标导向、工具使用、迭代反馈
3. **列举** 至少 2 个当前主流 AI Agent 的实际案例（如 Claude Code、Cursor Agent）
4. **描述** Agent 的"感知-规划-行动"循环的基本工作原理

### Common Misconceptions（常见误解）

- ❌ "Agent 就是更强的 Assistant" —— 两者是本质不同的设计哲学
- ❌ "Agent 不需要人类监督" —— 实际应用中人类仍是最终决策者
- ❌ "Agent 就是能调用工具的 ChatGPT" —— 工具调用只是 Agent 能力的一部分

---

## Stage 2: Evidence of Understanding（理解证据）

### Diagnostic Questions (CFU) / 理解检查

1. **CFU-1**: "如果让一个 AI 帮你订机票，它属于 Assistant 还是 Agent？为什么？"
2. **CFU-2**: "为什么 ChatGPT 每次回答完就'忘记'了，而 Agent 可以记住并在下次继续？"

---

## Stage 3: Learning Plan（学习流程）

### Phase 1: Hook（引入）—— 5min

**Socratic Question**:
> "想象一下：你对 Siri 说'帮我订明天早上8点去上海的机票'。Siri 打开了订票 App，你自己去选座、付款。这个过程中，Siri 扮演了什么角色？"

**Purpose**: 让学生意识到传统 Assistant 的本质是"工具的触发器"，而非真正的行动者。

### Phase 2: Exploration（探索）—— 15min

**Socratic Sequence**:

Q1: "那如果 AI 不只是打开 App，而是自动帮你比较所有航班价格、选出最优选项、替你付款，并把你的行程加到日历里——这还是'助手'吗？"

> 引导学生认识到：Agent 在执行一个**目标（goal）**，而 Assistant 在执行一个**指令（command）**。

Q2: "但 AI 自己怎么知道什么是最优选择？它需不需要提前知道你的偏好？"

> 引出 Agent 的**规划（planning）**能力，以及对**上下文/记忆**的需求。

Q3: "假设 AI 订票时发现那张卡余额不足，它会怎么做？是直接失败告诉你，还是会尝试换一张卡？"

> 引出 Agent 的**迭代反馈循环（iterative feedback）**——通过尝试-失败-调整来完成任务。

### Phase 3: Concept Formation（概念形成）—— 8min

**总结 Agent vs Assistant 对比表**：

| 维度 | AI Assistant | AI Agent |
|------|-------------|----------|
| 交互模式 | 单轮问答 | 多轮迭代 |
| 目标设定 | 人类设定 | Agent 自主分解 |
| 工具使用 | 人类触发 | Agent 自主调用 |
| 记忆 | 无状态 | 有上下文记忆 |
| 典型例子 | Siri, ChatGPT | Claude Code, AutoGPT |
| 适用场景 | 信息查询、单轮任务 | 复杂多步项目 |

### Phase 4: Check for Understanding（理解检查）—— 2min

**Exit Ticket**:
> "用一句话向没学过 AI 的朋友解释：AI Agent 和 Siri 这样的助手有什么本质区别？"

---

*本备课由 Socrate 系统生成 | UbD Stage 1 + 苏格拉底式对话设计 | 2026-04-24*
