# Jarvis Personal AI Assistant Showcase

Public showcase repository for ByteDance 2026 AI Full-Stack Challenge review and portfolio demonstration.

> Core implementation is currently closed-source. This repository contains the public demo package: project overview, architecture notes, resume bullets, application narrative, and video placeholder. The latest iOS app source code, production backend implementation, local databases, credentials, logs, and user data are intentionally excluded.

## 项目简介

Jarvis 是一个 iOS 个人 AI 助理原型，目标是把自然语言转成可靠、安全、可验证的生活事务操作。它不仅是聊天机器人，还能围绕日程、文件、餐厅推荐、旅行规划和费用记录形成完整工作流。

技术上，Jarvis 使用 React Native / Expo 构建 iOS 前端，FastAPI 构建后端，并用 SQLite 做可沙盒化的数据存储。后端按 DDD / bounded context 拆分为 calendar、tasks、document memory、travel、local service、weather、money 等模块。所有会改动用户数据的操作都会先生成确认卡片，用户确认后才执行。

## What the demo shows

- Morning brief: weather, yesterday recap, today schedule, and next useful action.
- Calendar operations: schedule lookup, meeting reschedule, conflict warning, confirmation-first mutation, and calendar verification.
- File and meeting prep: mock PDF, DOCX, and spreadsheet discovery with in-app preview.
- Local-service planning: restaurant recommendations with rating, distance, phone number, and dinner windows.
- Travel comparison: flight and hotel options ranked by price, duration, and trade-off score.
- Money beside Calendar: confirmed dinner and itinerary drafts save planned costs into a compact cost view.
- Safety surface: cards for review, confirmation, choices, completed actions, and structured objects.

## Competition track fit

Primary track: **实现一个可以端到端交付全栈项目的“超级个体”**.

Jarvis demonstrates how one developer can use AI coding tools to move from product goal, requirement decomposition, backend capability design, mobile UI, LLM orchestration, safety confirmation, simulator QA, and portfolio delivery.

Secondary fit:

- **AgentHub - 多 Agent 协作平台**: Jarvis already decomposes assistant capabilities into bounded contexts that can be generalized into an agent/capability hub.
- **实现一个基于 RAG 的多模态电商智能导购 Agent**: the older RAG prototype and Jarvis recommendation flows provide a transferable foundation for retrieval-driven guidance.

## Technical scope

- **Frontend**: React Native / Expo iOS interface.
- **Backend**: FastAPI service layer.
- **Data**: SQLite sandbox stores for demo-safe state management.
- **AI layer**: LLM orchestration, intent parsing, action frame generation, clarification, and response synthesis.
- **Tool/capability layer**: calendar, tasks, local services, document memory, travel, weather, attachments, and money/cost tracking.
- **Safety layer**: confirmation-first mutation for calendar changes, itinerary saves, compound schedule drafts, and cost creation.
- **QA layer**: simulator-based golden journey, scenario tests, smoke tests, and UX replay review.

## Demo video

The actual MP4/MOV file was not included in the uploaded materials available to this repository push. Recommended next step:

1. Record or export `jarvis_ai_fullstack_assistant_demo.mp4`.
2. Upload it through the GitHub web interface to this repository, a GitHub Release, or a README issue/asset.
3. Replace this placeholder with the GitHub asset URL.

Suggested file path:

```text
demo/jarvis_ai_fullstack_assistant_demo.mp4
```

## Public / private boundary

Public in this repository:

- Project overview
- Architecture summary
- Competition narrative
- Resume bullets
- Demo-video placeholder
- Security and privacy note

Private for now:

- Latest iOS app source code
- Production backend implementation
- User data, credentials, logs, local databases, and live adapters

## 中文简历版项目描述

**Jarvis 个人 AI 助理** - 基于 React Native / Expo、FastAPI、SQLite 和 LLM orchestration 构建 iOS 个人助理原型。设计了日程、任务、文件、餐厅/本地服务、旅行、天气和费用等 bounded contexts，实现了确认优先的安全执行机制、文档预览、旅行/费用保存、Calendar/Money 视图，以及基于模拟器的端到端 golden journey 回归测试。
