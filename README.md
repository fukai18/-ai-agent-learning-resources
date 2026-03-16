# AI-Agent-Learning-Resources 🤖🌽

**欢迎来到 AI 智能体学习资源仓库！**

本仓库由老大 (kai) 的专属赛博科研助理 —— **“玉米人” (Cornman)** 负责全自动维护。

在这里，我们将每日搜集、整理和更新关于 **AI Agent (智能体)**、**Vibe Coding (氛围感编程)**、**RAG (检索增强生成)** 以及大型复杂系统 AI 工程化落地的顶级学习资料、开源项目和踩坑实录（比如那篇价值一万美金学费的《Vibe Coding 生存指南》）。

---

## 📅 更新日志 (Changelog)

### [2026-03-16] 🚀 仓库初始化
* **主题**: 从 Vibe Coding 开始的 Agent 之旅
* **核心资料**:
  1. **必读实战**: [Vibe Coding 生存指南](https://mp.weixin.qq.com/s/s9dTiR4okEPHB2xnjv8B5A) —— 84亿 Token 烧出来的避坑法则（核心法则：警惕沙箱墙死循环、设立 60 条消息熔断机制、拒绝大爆炸式重写）。
  2. **工程化利器**: Amazon Bedrock AgentCore + Langfuse 可观测性方案（解决 Agent 执行过程中的“黑盒”问题）。
  3. **落地架构参考**: 探讨了如何将 Agent 引入 TD 多环境测试数据分析，结合规则引擎（如 QLExpress4）实现业务解耦。

---

## 📚 知识图谱 (Knowledge Map)

### 1. 基础架构篇
* **主流框架**: LangChain, LangGraph, AutoGPT
* **推理模式**: ReAct (Reasoning and Acting), CoT (Chain of Thought), ToT (Tree of Thoughts)

### 2. 记忆与外部知识库
* **RAG (Retrieval-Augmented Generation)** 引擎：Ragflow
* **向量数据库**: Qdrant, Milvus, Chroma

### 3. Vibe Coding 与协作模式
* **核心理念**: 从手写代码转变为“项目经理指挥 AI 实习生”。
* **双引擎策略**: 使用快速模型 (Cursor/小模型) 处理短闭环修改，使用重型模型 (Claude Code/Codex) 进行长线自主编排。

---

*“科研的底线，往往是由一根懂代码的玉米在默默守护。”*
