# Enterprise AI Transformation Runtime 学习计划

## 1. North Star

本课程的最终目标不是单独学习 RAG、Agent 框架或某个工具，而是打通企业 AI 转型的一条完整架构线路：

```text
RAG / Knowledge Runtime
-> Role Agent Copilot
-> Agentic Workflow 工程化
-> AI Native App 产品化重构
-> Autonomous Operation 受控自治
```

课程的 North Star 是：

> 完成企业 AI 转型的端到端架构闭环：从可信知识底座开始，让 AI 进入岗位、进入流程、进入业务系统，最终形成可治理、可审计、可评测、可受控自治的 Enterprise AI Operating System。

这个 North Star 用来判断每个学习内容是否值得进入课程：

- 它是否帮助企业知识变得可信、可引用、可维护？
- 它是否帮助 AI 进入一个具体岗位或业务流程？
- 它是否让 Agent 行为变得可追踪、可恢复、可审批？
- 它是否帮助业务系统从外挂聊天框变成 AI Native App？
- 它是否让自治操作具备权限、审计、评测和回滚边界？

## 2. 课程周期

建议周期：

```text
150 个有效学习日
= 15 个 Sprint
= 每个 Sprint 10 个学习日
```

如果按每周 5 天、每天 60-90 分钟学习：

```text
150 个学习日 = 30 周 = 约 7 个月
```

本课程不是线性课程，不是先只学 RAG，再只学 Role Agent，再只学 Workflow。

它采用螺旋式结构：

```text
每个 Sprint 同时包含：
1. 主技术能力
2. Role Copilot 应用验证
3. Agentic Workflow 连接点
4. Runtime / Governance 抽象沉淀
5. 一个可见产出
```

五层能力一直都在，只是每个阶段权重不同：

```text
Day 1-30:
RAG / Knowledge Runtime 权重最高，但每个 Sprint 都接入 Role Copilot case。

Day 31-60:
Role Agent Copilot 权重最高，但继续补 RAG、trace、eval、权限。

Day 61-90:
Agentic Workflow 权重最高，但 workflow 必须串起 RAG 和 Role Copilot。

Day 91-120:
AI Native App 权重最高，但产品界面必须展示 trace、eval、approval、knowledge lifecycle。

Day 121-150:
Autonomous Operation 权重最高，但治理对象必须是前面做出来的 Role Copilot 和 workflow。
```

## 3. 总体能力地图

### 3.1 RAG / Knowledge Runtime

目标：

> 建立企业 AI 的可信知识底座。

核心能力：

- 文档治理
- chunk / metadata
- embedding / retrieval / rerank
- citation
- ACL / 权限过滤
- memory / context
- trace
- eval
- 知识生命周期

阶段成果：

- Agent Knowledge Runtime v0.1
- chunk schema
- citation schema
- RAG trace schema
- RAG eval cases
- 知识治理规范

### 3.2 Role Agent Copilot

目标：

> 让 AI 进入具体岗位，而不是停留在知识问答。

核心能力：

- Role
- Workflow
- Scenario
- Context
- Tool
- Guardrail
- Trace
- Human Review
- 判断型 Copilot
- 执行型 Copilot
- 混合型 Copilot

阶段成果：

- Role Copilot 通用模板
- HR Agent Copilot 样板
- DevOps Agent Copilot 样板
- Project Agent Copilot 样板
- skill manifest
- role manifest
- tool schema
- approval policy

### 3.3 Agentic Workflow 工程化

目标：

> 把单个 skill / copilot 升级成可追踪、可恢复、可审批的流程系统。

核心能力：

- 裸 agent loop
- OpenAI Agents SDK
- LangGraph / state graph
- tool calling
- handoff
- human-in-the-loop
- 状态机
- 幂等
- 重试
- 失败恢复
- 长任务 trace

阶段成果：

- 手写最小 agent loop
- LangGraph workflow demo
- 跨 skill Role Copilot workflow
- workflow state schema
- retry / approval / failure recovery 设计

### 3.4 AI Native App 产品化重构

目标：

> 让 AI 不只是外挂聊天框，而是重构业务应用形态。

核心能力：

- AI-first interaction
- 业务对象建模
- AI action model
- 人工复核界面
- 用户纠错机制
- 知识运营后台
- trace dashboard
- eval dashboard
- 成本与质量看板

阶段成果：

- AI Native App 原型设计
- Knowledge Operation Console
- DevOps Copilot Console
- 业务对象 schema
- AI action schema
- trace / eval / audit 页面草图

### 3.5 Autonomous Operation 受控自治

目标：

> 形成企业 AI 受控自治的治理能力。

核心能力：

- tool safety level
- policy engine
- approval workflow
- rollback
- audit
- agent registry
- tool registry
- eval registry
- cost governance
- multi-domain governance
- continuous evaluation

阶段成果：

- Enterprise AI Operating System 架构图
- Agent Registry 设计
- Tool Registry 设计
- Risk / Approval Policy
- Autonomous Operation 分级模型
- 持续评测闭环

## 4. 15 个 Sprint 课程安排

## Sprint 1: RAG 链路与企业 AI 主链路

时间：

```text
Day 1-10
```

主技术能力：

- RAG 完整链路
- query -> retrieval -> context -> answer -> citation -> eval
- 普通 RAG demo 与企业 Knowledge Runtime 的区别

Role Copilot 应用验证：

- HR Copilot 为什么需要证据引用
- DevOps Copilot 为什么需要项目文档检索
- Project Copilot 为什么需要项目上下文

Agentic Workflow 连接点：

- 把 RAG 看成 Role Copilot workflow 中的一个能力节点
- 区分 Knowledge QA 和 Operation Tool

Runtime / Governance 抽象：

- source
- citation
- trace_id
- evidence
- insufficient_evidence

可见产出：

- 企业 AI 主链路图
- 一个 Role Copilot 场景里的 RAG trace case

验收问题：

- 为什么企业 AI 不能只做一个知识库问答？
- 一个 Role Copilot 在什么情况下需要 RAG？
- 没有证据时，Agent 应该如何回答？

## Sprint 2: chunk / metadata 与岗位知识建模

时间：

```text
Day 11-20
```

主技术能力：

- chunk 设计
- metadata 设计
- 文档版本
- heading / source_path / updated_at
- 权限标签

Role Copilot 应用验证：

- HR 简历和 JD 如何 chunk
- DevOps 发布文档如何 chunk
- Project Copilot 项目文档如何 chunk

Agentic Workflow 连接点：

- workflow 节点如何使用 metadata filter
- 不同 Role 如何只召回自己的领域知识

Runtime / Governance 抽象：

- chunk schema
- metadata schema
- domain
- role
- visibility
- lifecycle_status

可见产出：

- 通用 chunk schema v0.1
- HR / DevOps / Project 三类文档 chunk 对比表

验收问题：

- chunk 与原文如何追溯？
- metadata 如何减少错召回？
- 权限字段为什么不能交给模型判断？

## Sprint 3: citation / trace / eval 与可信输出

时间：

```text
Day 21-30
```

主技术能力：

- citation 格式
- RAG trace
- eval case
- hallucination 定位
- rule judge / human judge / LLM judge

Role Copilot 应用验证：

- HR 候选人评分如何引用简历事实
- DevOps 失败诊断如何引用日志和文档
- Project review 如何引用代码、需求和测试结果

Agentic Workflow 连接点：

- 每个 workflow 节点都要产生可追踪证据
- 输出结果必须能回到 trace

Runtime / Governance 抽象：

- citation schema
- trace schema
- eval case schema
- bad case schema

可见产出：

- 10-20 个 RAG / Role Copilot eval cases
- Agent Knowledge Runtime v0.1 设计草案

验收问题：

- citation 存在是否等于结论可信？
- trace 如何帮助定位 retrieval、context builder、generation 的问题？
- 哪些 eval 可以规则判断，哪些必须人工判断？

## Sprint 4: Role / Workflow / Scenario 建模

时间：

```text
Day 31-40
```

主技术能力：

- Role Agent 方法论
- Workflow 抽取
- Scenario 拆分
- 标准工作流 Agent 化

Role Copilot 应用验证：

- DevOps Package / Release Copilot
- HR Resume Screening Copilot
- Project Develop Copilot

Agentic Workflow 连接点：

- 每个 scenario 对应一个 workflow 入口
- 每个 workflow 都需要输入、输出、状态和风险等级

Runtime / Governance 抽象：

- role manifest
- scenario manifest
- workflow manifest
- trigger rule

可见产出：

- Role Copilot 通用设计模板
- 一个标准工作流 Agent 化拆解案例

验收问题：

- 什么样的流程适合 Agent 化？
- Role Agent 和普通聊天机器人有什么区别？
- Scenario 为什么比泛泛的 intent 更稳定？

## Sprint 5: Tool / Guardrail 与执行型 Copilot

时间：

```text
Day 41-50
```

主技术能力：

- tool schema
- command preview
- 参数校验
- 执行前确认
- tool safety level

Role Copilot 应用验证：

- DevOps Package Copilot
- build / package / push / release 的风险分级
- 项目文档作为事实来源

Agentic Workflow 连接点：

- ToolProvider
- AuthProvider
- approval_required
- execution_trace

Runtime / Governance 抽象：

- tool registry
- tool safety policy
- command trace
- execution report format

可见产出：

- DevOps 执行型 Copilot v0.1 样板
- tool safety level 表

验收问题：

- 为什么模型不能直接执行世界？
- 哪些操作可以自动执行，哪些必须确认？
- Agent 如何避免发明脚本参数？

## Sprint 6: Rubric / Human Review 与判断型 Copilot

时间：

```text
Day 51-60
```

主技术能力：

- rubric 设计
- 证据抽取
- 事实与判断分离
- 人工复核
- 受保护属性 guardrail

Role Copilot 应用验证：

- HR Resume Screening Copilot
- Candidate Detail Report
- Interview Question Generator

Agentic Workflow 连接点：

- judgment workflow
- review_required
- evidence-based scoring

Runtime / Governance 抽象：

- rubric schema
- human review schema
- scoring trace
- protected attribute policy

可见产出：

- HR 判断型 Copilot v0.1 样板
- 判断型 Copilot eval rubric

验收问题：

- AI 评分为什么必须区分事实和判断？
- 什么内容必须作为面试验证点，而不是直接定论？
- 判断型 Copilot 的风险和执行型 Copilot 有什么不同？

## Sprint 7: 裸 Agent Loop 与最小 Agent Runtime

时间：

```text
Day 61-70
```

主技术能力：

- 裸 agent loop
- LLM -> tool -> result -> next step -> final
- tool result 作为上下文
- exit condition

Role Copilot 应用验证：

- DevOps 打包请求如何形成执行循环
- HR 分析请求如何形成证据循环
- Project fix 如何形成诊断循环

Agentic Workflow 连接点：

- agent state
- tool call state
- max retry
- stop condition

Runtime / Governance 抽象：

- agent run schema
- tool call schema
- loop trace
- failure boundary

可见产出：

- 手写最小 agent loop
- 一个 Role Copilot agent run trace

验收问题：

- Agent loop 和普通函数调用有什么区别？
- 为什么必须有退出条件？
- tool result 为什么不能无校验地进入下一轮？

## Sprint 8: LangGraph / State Graph 与跨 Skill Workflow

时间：

```text
Day 71-80
```

主技术能力：

- LangGraph
- state graph
- nodes / edges
- checkpoint
- human-in-the-loop
- streaming

Role Copilot 应用验证：

- Project Agent Copilot 的 init -> ingest -> develop -> review -> finish
- DevOps build -> diagnose -> report

Agentic Workflow 连接点：

- 把多个 skills 串成状态图
- 每个节点都可追踪、可暂停、可恢复

Runtime / Governance 抽象：

- workflow state schema
- checkpoint schema
- node trace
- handoff schema

可见产出：

- LangGraph workflow demo
- 一个跨 skill workflow 设计

验收问题：

- 什么时候需要 LangGraph，什么时候 Skill + Script 就够？
- 状态图比简单 agent loop 多解决了什么问题？
- checkpoint 对企业工作流有什么价值？

## Sprint 9: Handoff / Retry / Approval 与工程化工作流

时间：

```text
Day 81-90
```

主技术能力：

- handoff
- retry
- idempotency
- failure recovery
- approval workflow
- long-running task

Role Copilot 应用验证：

- DevOps Release Copilot 的审批和失败恢复
- Project Fix Copilot 的诊断与回滚建议
- MAS / SRE Copilot 的人工交接

Agentic Workflow 连接点：

- agent handoff
- human review
- approval_required
- retryable / non_retryable

Runtime / Governance 抽象：

- approval policy
- retry policy
- failure classification
- idempotency key

可见产出：

- Agentic Workflow v0.1
- retry / approval / handoff 设计文档

验收问题：

- 为什么企业 Agent 不能无限重试？
- 什么情况下需要 handoff 给人？
- 幂等对工具调用为什么重要？

## Sprint 10: AI Native App 信息架构

时间：

```text
Day 91-100
```

主技术能力：

- AI Native App
- 业务对象建模
- AI action model
- 人机协作入口
- 可解释界面

Role Copilot 应用验证：

- Knowledge Operation Console
- DevOps Copilot Console
- HR Screening Console

Agentic Workflow 连接点：

- workflow state 在页面中可见
- 人工复核和审批不只在聊天里完成

Runtime / Governance 抽象：

- business object schema
- AI action schema
- UI state
- review queue

可见产出：

- AI Native App 信息架构
- 一个 Console 原型草图

验收问题：

- AI Native App 和普通业务系统外挂聊天框有什么区别？
- 哪些 AI 行为应该被设计成 action？
- 人类如何纠正 AI 的中间判断？

## Sprint 11: Trace / Eval Dashboard 与知识运营后台

时间：

```text
Day 101-110
```

主技术能力：

- trace dashboard
- eval dashboard
- bad case 管理
- 知识命中率
- 引用质量
- 反馈闭环

Role Copilot 应用验证：

- HR 评分 bad case
- DevOps 构建失败 bad case
- Project review 漏检 case

Agentic Workflow 连接点：

- 每个 workflow run 进入 trace dashboard
- 每个 bad case 反向更新知识、工具或 policy

Runtime / Governance 抽象：

- bad case schema
- eval report schema
- feedback schema
- quality metric

可见产出：

- Trace / Eval Dashboard 设计
- 知识运营后台模块图

验收问题：

- 如何判断一个 Copilot 是否真的变好？
- bad case 应该反向改 prompt、知识、tool 还是 policy？
- 哪些质量指标能规则化？

## Sprint 12: Action Model 与人机协作产品形态

时间：

```text
Day 111-120
```

主技术能力：

- AI action
- draft action
- write action
- review queue
- approval UX
- rollback UX

Role Copilot 应用验证：

- DevOps release draft
- HR candidate recommendation
- Project code review action

Agentic Workflow 连接点：

- action 与 workflow state 绑定
- 用户可以批准、拒绝、修改、退回

Runtime / Governance 抽象：

- action schema
- approval record
- rollback hint
- audit event

可见产出：

- AI Native App v0.1 产品化设计
- action / approval / audit 数据模型

验收问题：

- AI 的建议、草稿和执行动作如何区分？
- 用户修改 AI 输出后，系统如何学习？
- 审批记录如何进入 audit？

## Sprint 13: Policy / Registry 与多 Role Copilot 治理

时间：

```text
Day 121-130
```

主技术能力：

- policy engine
- agent registry
- skill registry
- tool registry
- domain adapter registry
- eval registry

Role Copilot 应用验证：

- HR / DevOps / Project 共享 Runtime
- 不同 Role 使用不同工具和权限
- 同一工具在不同 Role 下风险等级不同

Agentic Workflow 连接点：

- workflow 运行前读取 policy
- tool 调用前检查 registry 和 permission

Runtime / Governance 抽象：

- registry schema
- policy schema
- domain adapter schema
- role permission matrix

可见产出：

- Enterprise AI Runtime Registry 设计
- 多 Role Copilot 治理模型

验收问题：

- Runtime 为什么不能写死 HR、DevOps、MAS？
- Domain Adapter 应该定义哪些内容？
- Tool Registry 和 Skill Registry 有什么区别？

## Sprint 14: Autonomous Operation 分级与受控执行闭环

时间：

```text
Day 131-140
```

主技术能力：

- autonomous operation
- risk level
- approval level
- policy enforcement
- rollback
- continuous eval

Role Copilot 应用验证：

- DevOps read/build/write/dangerous 分级
- SRE 查询/建议/工单/重启分级
- HR 推荐/拒绝/录用决策边界

Agentic Workflow 连接点：

- 低风险自动执行
- 中风险人工确认
- 高风险审批执行
- 危险动作默认禁止

Runtime / Governance 抽象：

- autonomy level model
- risk approval matrix
- continuous monitoring
- audit trail

可见产出：

- Autonomous Operation 分级模型
- 受控自治 demo 设计

验收问题：

- 受控自治和完全自动化有什么区别？
- 为什么企业 Agent 需要默认禁止某些动作？
- eval 如何参与自治级别提升？

## Sprint 15: 总架构复盘与作品集整合

时间：

```text
Day 141-150
```

主技术能力：

- 企业 AI 转型总架构
- 作品集叙事
- 能力地图
- 下一阶段规划

Role Copilot 应用验证：

- HR / DevOps / Project 三类 Copilot 总结
- 选择一个最有代表性的端到端 demo

Agentic Workflow 连接点：

- 从知识到岗位、流程、应用、自治治理的一条完整链路

Runtime / Governance 抽象：

- Enterprise AI Operating System 架构图
- 五层能力地图
- 统一术语表
- v0.1 -> v1.0 路线

可见产出：

- Enterprise AI Transformation Runtime 总架构图
- 3 分钟项目介绍
- README / Portfolio 文案
- 下一阶段 90 天深入计划

验收问题：

- 你如何向别人解释这套企业 AI 转型架构？
- 你已经打通了哪条最小闭环？
- 下一阶段应该加深 RAG、Role Copilot、Workflow、Product 还是 Governance？

## 5. 每 10 天复盘模板

每个 Sprint 结束时，用下面的模板复盘：

```markdown
## Sprint N 复盘

- 主学习点：
- Role Copilot 验证：
- Workflow 连接点：
- Runtime / Governance 沉淀：
- 可见产出：
- 当前最清楚的能力：
- 当前最薄弱的能力：
- 需要进入下个 Sprint 的问题：
- 是否达到有效进度：
```

有效进度判断标准：

```text
0-2/5：只看过概念，不能解释用途或边界
3/5：能用自己的话说明，并回答一个验证问题
4/5：能解释场景、边界、误区或设计取舍
5/5：能迁移到自己的 Role Copilot / Runtime 设计里
```

## 6. 最小闭环优先级

课程始终遵守一个原则：

> 先纵向打通一条最小闭环，再横向补齐每一层能力。

推荐第一条最小闭环：

```text
企业文档 / 项目文档
-> RAG / Knowledge Runtime
-> DevOps 或 HR Role Copilot
-> 可追踪 Agentic Workflow
-> 轻量 AI Native Console 或报告
-> 审批 / trace / eval / audit
```

打通以后，再逐层加厚：

```text
RAG 层：GraphRAG / hybrid search / rerank / knowledge lifecycle
Role 层：更多 Copilot / 更多 domain adapter
Workflow 层：LangGraph / 状态机 / handoff / long-running task
App 层：Console / Dashboard / Review Queue
Operation 层：Policy / Registry / Governance / Continuous Eval
```

## 7. 与当前已有资产的关系

本课程不是从零开始。

当前已有资产可以直接纳入课程：

- Role Agent 方法论文章
- Enterprise Agent Copilot Taxonomy
- DevOps Release Copilot 设计
- `role-copilot-skills` 仓库
- HR Agent Copilot skills
- DevOps Agent Copilot skills
- Project Agent Copilot skills
- Agent Knowledge Runtime 学习记录

这些资产的关系是：

```text
方法论文章：解释为什么企业 Agent 应该从 Role Agent 开始
Taxonomy：定义 Runtime / Role Copilot / Skill 的分层和命名
Skills 仓库：验证 Role Copilot 的实际工作流
Learning Plan：把知识、框架、产品和治理串成长期能力路线
```

## 8. 课程最终交付物

150 个有效学习日结束时，理想交付物包括：

- Enterprise AI Transformation Runtime 总架构图
- Agent Knowledge Runtime v0.1 设计
- Role Copilot 通用模板
- HR / DevOps / Project 三类 Copilot 样板
- 一个 Agentic Workflow demo
- 一个 AI Native App / Console 原型设计
- Policy / Registry / Governance 设计
- trace / eval / audit schema
- 作品集 README
- 3 分钟项目介绍
- 下一阶段 90 天计划

最终要能清楚表达：

> 我不是只会做一个 RAG demo，也不是只会写 prompt 或用某个 Agent 框架。我能从企业 AI 转型的角度，把知识底座、岗位 Copilot、流程工程化、AI Native App 和受控自治治理串成一条可落地的架构路线。
