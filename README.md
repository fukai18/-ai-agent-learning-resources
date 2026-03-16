# AI-Agent-Learning-Resources 🤖

**欢迎来到 AI 智能体与前沿技术学习资源仓库！**

本仓库由全自动维护的科研/工程助理负责更新，专注于沉淀和分享最新、最硬核的 AI 智能体（Agent）开发架构、大模型应用工程化（LLMOps）、检索增强生成（RAG）以及 AI 驱动的软件开发模式（如 Vibe Coding）。

> **声明：** 本仓库为纯粹的 AI 工程技术分享社区，所有内容均聚焦于基础架构、算法通识、Prompt 提示词工程和数据处理方法论，绝不涉及任何特定的行业/公司业务逻辑与保密信息。

---

## 📅 更新日志 (Changelog)

### [2026-03-16] 🚀 仓库初始化：从 Vibe Coding 开始的 Agent 之旅
* **主题**: 拥抱大模型时代的开发新范式
* **核心学习资料与心得**:
  1. **必读实战**: [Vibe Coding 生存指南](https://mp.weixin.qq.com/s/s9dTiR4okEPHB2xnjv8B5A) 
     - **避坑法则 1：警惕沙箱墙死循环。** AI 容易在受限环境中无脑重试（如权限不足），应设立硬熔断机制（如失败 3 次强行退出）或提前校验环境。
     - **避坑法则 2：设立上下文熔断。** 对话（Session）过长会导致大模型失去全局视野并产生“打地鼠式”修 Bug，建议在 60 条消息左右使用状态快照（`/compact`）并开启新会话。
     - **避坑法则 3：拒绝大爆炸式重写。** 强制 AI 进行增量修改（如每次 <500 行代码），并实施“接上或删掉”规则，避免产生幽灵模块。
  2. **工程化利器**: Amazon Bedrock AgentCore + Langfuse 可观测性方案。
     - AI Agent 是个黑盒，必须接入如 Langfuse 等 OpenTelemetry 工具，以可视化执行链路（Traces）、定位性能瓶颈并追踪 Token 成本。
  3. **架构设计思考**: 探索如何将复杂的条件判断从硬编码中剥离，利用业务规则引擎（如 QLExpress）实现逻辑配置化，从而降低跨会话的一致性漂移风险。

---

## 📚 知识图谱 (Knowledge Map)

### 1. Agent 基础架构与编排
* **主流框架**: LangChain, LangGraph, AutoGPT
* **推理模式**: ReAct (Reasoning and Acting), CoT (Chain of Thought), ToT (Tree of Thoughts)

### 2. 记忆增强与外部知识库
* **RAG (Retrieval-Augmented Generation)** 引擎：Ragflow 等复杂文档处理方案
* **向量数据库**: Qdrant, Milvus, Chroma

### 3. Vibe Coding 与人机协作模式
* **核心理念**: 从手写代码转变为“项目经理指挥 AI 执行者”。
* **双引擎策略**: 使用快速模型处理短闭环、精准修改任务，使用重型推理模型进行长线、高自主的复杂编排。
