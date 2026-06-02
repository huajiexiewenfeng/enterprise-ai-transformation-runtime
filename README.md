# Enterprise AI Transformation Runtime

这是一个关于企业 AI 转型架构的长期学习、实践和沉淀仓库。

本仓库不是单独记录 RAG、Agent 框架或某个工具的使用笔记，而是围绕一条完整的企业 AI 转型主线持续建设：

```text
RAG / Knowledge Runtime
-> Role Agent Copilot
-> Agentic Workflow 工程化
-> AI Native App 产品化重构
-> Autonomous Operation 受控自治
```

## North Star

本项目的目标是打通企业 AI 转型的端到端架构闭环：

> 从可信知识底座开始，让 AI 进入岗位、进入流程、进入业务系统，最终形成可治理、可审计、可评测、可受控自治的 Enterprise AI Operating System。

## 当前学习计划

主课程文档：

- [Enterprise AI Transformation Runtime 学习计划](./enterprise-ai-transformation-runtime-learning-plan.zh.md)

课程周期：

```text
150 个有效学习日
= 15 个 Sprint
= 每个 Sprint 10 个学习日
```

课程采用螺旋式结构，不是先孤立学习 RAG，再学习 Role Agent，再学习 Workflow，而是每个 Sprint 同时包含：

- 主技术能力
- Role Copilot 应用验证
- Agentic Workflow 连接点
- Runtime / Governance 抽象沉淀
- 一个可见产出

## 五层主线

### 1. RAG / Knowledge Runtime

建立企业 AI 的可信知识底座，重点包括文档治理、chunk、metadata、retrieval、rerank、citation、权限过滤、trace、eval 和知识生命周期。

### 2. Role Agent Copilot

让 AI 进入具体岗位和业务场景，沉淀 Role、Workflow、Scenario、Context、Tool、Guardrail、Trace 和 Human Review。

### 3. Agentic Workflow 工程化

把单个 skill 或 copilot 升级成可追踪、可恢复、可审批的流程系统，学习 agent loop、tool calling、handoff、LangGraph、human-in-the-loop、幂等、重试和失败恢复。

### 4. AI Native App 产品化重构

让 AI 不只是外挂聊天框，而是进入业务对象、操作模型、复核队列、审批界面、trace dashboard、eval dashboard 和知识运营后台。

### 5. Autonomous Operation 受控自治

建立企业 AI 的受控自治能力，包含 tool safety level、policy engine、approval workflow、rollback、audit、agent registry、tool registry、eval registry 和 continuous evaluation。

## 仓库将沉淀什么

后续本仓库会持续更新：

- 学习进度
- 每个 Sprint 的学习笔记
- 架构图
- schema 设计
- Role Copilot 方法论
- Agentic Workflow 实验
- AI Native App 产品化设计
- Governance / Policy / Registry 设计
- 作品集材料

## 相关项目

- [role-copilot-skills](https://github.com/huajiexiewenfeng/role-copilot-skills)：面向企业团队提效的 Role Copilot Skills 集合。

## 核心判断

企业 AI 转型不是做一个单点 RAG demo，也不是把聊天框接入业务系统。

更合理的路线是：

```text
可信知识
-> 岗位 Copilot
-> 工程化 Workflow
-> 产品化 App
-> 受控自治治理
```

先纵向打通一条最小闭环，再横向补齐每一层能力。
