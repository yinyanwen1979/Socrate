---
title: "AI Agent 智能体"
topic: "AI Agent"
target_audience: "intermediate"
difficulty: "intermediate"
estimated_total_hours: 0
generated_date: "2026-04-24"
---

# Learning Outline: AI Agent 智能体

## Chapter 1: AI Agent 基础概念

### Topic 1.1: 什么是 AI Agent

**Overview**: AI Agent（智能体）是指能够自主感知环境、做出决策并执行动作的人工智能系统。与传统 AI 助手不同，Agent 能够自主规划、调用工具、并通过反馈循环不断优化行为。

**Knowledge Points**:
- **KP-1.1.1**: Agent vs Assistant 区别
  - Difficulty: easy
  - Time: 30min
  - Prerequisites: []
  - Introduction: Question approach

- **KP-1.1.2**: Agent 的核心组件（感知、规划、行动）
  - Difficulty: medium
  - Time: 45min
  - Prerequisites: ["KP-1.1.1"]
  - Introduction: Scenario approach

- **KP-1.1.3**: ReAct / Plan-and-Execute 范式
  - Difficulty: medium
  - Time: 50min
  - Prerequisites: ["KP-1.1.2"]
  - Introduction: Contrast approach

### Topic 1.2: 单智能体架构

**Overview**: 单智能体系统由 LLM + 工具 + 记忆三部分组成，形成闭环的感知-决策-执行系统。

**Knowledge Points**:
- **KP-1.2.1**: LLM 作为大脑（推理能力、工具调用）
  - Difficulty: medium
  - Time: 40min
  - Prerequisites: ["KP-1.1.1"]
  - Introduction: Question approach

- **KP-1.2.2**: 工具调用（Tool Use / Function Calling）
  - Difficulty: medium
  - Time: 45min
  - Prerequisites: ["KP-1.2.1"]
  - Introduction: Scenario approach

- **KP-1.2.3**: 记忆系统（短期/长期/向量数据库）
  - Difficulty: hard
  - Time: 60min
  - Prerequisites: ["KP-1.2.2"]
  - Introduction: Question approach

---

## Chapter 2: 多智能体系统

### Topic 2.1: 多智能体协作模式

**Overview**: 多个 Agent 协作可以解决复杂任务，常见模式包括层次结构、并行执行和协商机制。

**Knowledge Points**:
- **KP-2.1.1**: Agent Team / Manager-Worker 模式
  - Difficulty: medium
  - Time: 45min
  - Prerequisites: ["KP-1.2.1"]
  - Introduction: Scenario approach

- **KP-2.1.2**: 智能体间通信协议
  - Difficulty: hard
  - Time: 50min
  - Prerequisites: ["KP-2.1.1"]
  - Introduction: Question approach

### Topic 2.2: 实际多智能体框架

**Overview**: 主流多智能体开发框架及其适用场景。

**Knowledge Points**:
- **KP-2.2.1**: CrewAI / AutoGen / LangGraph 对比
  - Difficulty: medium
  - Time: 60min
  - Prerequisites: ["KP-2.1.1"]
  - Introduction: Contrast approach

---

## Review Phase: AI Agent Mastery

### Review 1: 单智能体实现
- Combine KP-1.1.1, KP-1.2.1, KP-1.2.2
- Build: 一个带工具调用和记忆的 AI Agent
- Time: 3 hours

### Final Project: 多智能体协作系统
- Integrate Chapter 1 + 2
- Build: 多智能体代码审查系统（规划 Agent + 执行 Agent + 审查 Agent）
- Time: 6 hours
