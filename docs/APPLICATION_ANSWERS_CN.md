# 字节跳动 2026 年 AI 全栈挑战赛报名材料草稿

## 推荐课题意向

### 第一意向

实现一个可以端到端交付全栈项目的“超级个体”

理由：Jarvis 项目完整覆盖 AI Coding、产品设计、移动端前端、FastAPI 后端、SQLite 数据层、LLM orchestration、工具调用、安全确认机制、测试回归和 Demo 交付，能够直接展示一个人如何借助 AI Coding 完成端到端全栈应用开发。

### 第二意向

AgentHub - 多 Agent 协作平台

理由：Jarvis 后端已经按照 bounded context 拆分为日程、任务、本地服务、文档记忆、旅行、天气和费用等能力模块，可进一步扩展为多 Agent / 多能力协作平台。

### 第三意向

实现一个基于 RAG 的多模态电商智能导购 Agent

理由：已有 RAG 项目基础和 Jarvis 中的推荐、比较、文档记忆能力，可迁移到商品识别、跨平台比价、历史价格分析和自然语言导购场景。

## 代表性项目 1：Jarvis Personal AI Assistant

Jarvis Personal AI Assistant 是我正在独立开发的一款 iOS 个人 AI 助理原型，目标是将自然语言指令转化为安全、可验证、可执行的个人事务操作。系统覆盖日程管理、任务管理、文件与会议准备、天气简报、本地服务推荐、旅行方案比较和费用记录等场景。

技术实现上，前端基于 React Native / Expo 构建 iOS 交互界面，后端基于 FastAPI 与 SQLite 构建可沙盒化的数据与工具调用层，并通过 LLM orchestration 将用户意图解析为结构化 action frame，再由不同能力模块执行。后端采用 bounded context 设计，将 calendar、tasks、document memory、travel、weather、money 等模块拆分为独立能力接口。

项目重点不是单纯聊天，而是“确认优先”的安全执行机制：所有会修改用户数据的操作，如日历改期、复合日程草稿、旅行行程保存和费用创建，都会先生成确认卡片，用户确认后再执行。当前 demo 已覆盖 morning brief、日程查询与改期、冲突提醒、文件预览、餐厅推荐、旅行比较、费用保存和 calendar verification 等完整 golden journey。

当前阶段：已拥有可展示 Demo，正在继续扩展 live adapters、移动端体验和长期记忆能力。

## 代表性项目 2：Yuwen-RAG / Research Knowledge Retrieval System

Yuwen-RAG 是我此前搭建的检索增强生成系统，用于将文档、论文或结构化知识拆解为可检索单元，并通过 query embedding 与相似度匹配实现基于上下文的回答生成。该项目帮助我理解 RAG 系统中的文档解析、chunking、embedding、相似度检索、上下文重组和回答生成流程。

在此基础上，我进一步探索了 AI coding 与 agentic workflow，将 Codex / AI coding 工具用于需求拆解、代码生成、调试、测试与交付流程自动化。这一经历直接延伸到 Jarvis 项目中，使我能够以“超级个体”的方式推进全栈项目开发：从产品目标、功能拆解、后端接口、前端交互、模拟器测试到 README / 演示材料准备，均通过 AI coding 工具辅助完成。

## 主要技术栈

前端 / 移动端：React Native、Expo、iOS Simulator、component-based UI、mobile interaction design

后端：Python、FastAPI、REST API、modular backend architecture、bounded context design

数据与存储：SQLite、sandboxed stores、seeded/mock adapters、structured action state

AI / Agent：LLM orchestration、tool calling、intent parsing、action frame generation、confirmation-first mutation、RAG、embedding-based retrieval

工程与测试：Codex、AI coding workflow、simulator replay、smoke tests、targeted scenario tests、golden-journey regression、UX replay review

相关工具：Git/GitHub、Markdown documentation、API integration、prompt engineering

## 项目阶段

已经拥有完整 Demo。

## 全栈工程能力

非常熟悉全栈开发。Jarvis 项目覆盖移动端前端、后端服务、数据存储、LLM orchestration、工具调用、安全确认机制、测试回归与 Demo 交付。

## AI Coding 工具使用

经常使用 AI Coding 工具进行开发。Jarvis 项目中的需求拆解、代码迭代、测试设计、UI 体验复盘、README 与 Demo 材料准备均大量使用 Codex / AI coding workflow 辅助完成。

## 希望了解的信息

希望进一步了解各课题的最终交付标准、是否必须公开完整源代码、线上部署平台要求、AI coding 工具使用范围，以及评审是否更看重业务完整度、工程质量、创新性还是 demo 可用性。
