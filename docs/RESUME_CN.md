# 张昱文｜AI 全栈挑战赛中文简历

**方向：AI 全栈开发 / Agent 系统 / RAG / 智能工程系统**  
GitHub: johnZYW  
邮箱: yuwen.zhang@sydney.edu.au  
LinkedIn: linkedin.com/in/yuwen-zhang-07950b170

## 个人简介

悉尼大学航空航天工程博士研究生，长期关注 AI、Agent 系统、RAG 知识检索、工程优化与智能化工作流开发。近期独立开发 **Jarvis Personal AI Assistant**，一个基于 React Native / Expo、FastAPI、SQLite 与 LLM orchestration 的 iOS 个人 AI 助理原型，支持用户通过自然语言完成日程管理、任务管理、文件预览、天气简报、旅行规划、本地服务推荐与费用记录等操作。

擅长将复杂系统拆解为可执行模块，并通过 AI Coding 工具辅助完成需求澄清、方案拆解、代码生成、测试回归与演示交付。此前搭建过 RAG 知识检索系统，并在航空仿真、eVTOL 多学科优化、机器人控制与 AI 辅助研究工作流方面积累了跨学科项目经验。

## 教育背景

**悉尼大学｜航空航天工程博士研究生**  
2021 – 2026  
研究方向：多学科系统优化、eVTOL 飞行器设计、AI 辅助工程建模、智能化仿真工作流

**悉尼大学｜航空航天工程学士，一等荣誉学位**  
2016 – 2020  
GPA: 3.9 / 4.0

## 技术能力

**AI / Agent / RAG**：LLM orchestration、Agent workflow、tool calling、RAG 知识检索、embedding-based retrieval、prompt engineering、AI coding workflow、confirmation-first action safety

**全栈开发**：React Native、Expo、FastAPI、REST API、SQLite、Python、JavaScript、模块化后端设计、移动端交互原型开发

**AI Coding 与工程交付**：Codex、AI-assisted development、需求拆解、代码生成、debugging、smoke test、scenario test、simulator-based regression、README / Demo / Slide 交付材料生成

**工程仿真与优化**：FlightStream、Ansys Fluent、MATLAB、Simulink、NSGA-II、多目标优化、飞行动力学建模、机器人控制

## 代表性项目经历

### Jarvis Personal AI Assistant｜iOS AI 全栈个人助理原型

**项目阶段：已有完整 Demo，持续开发中**  
**技术栈：React Native / Expo、FastAPI、SQLite、LLM orchestration、Python、JavaScript、iOS Simulator**

独立开发一款 Jarvis 风格的 iOS 个人 AI 助理原型，目标是将用户自然语言指令转化为安全、结构化、可验证的个人事务操作。系统覆盖日程管理、任务管理、文件与会议准备、天气简报、本地服务推荐、旅行方案比较和费用记录等场景。

主要工作：

- 构建 React Native / Expo 移动端界面，设计聊天、日历、任务、设置等核心交互页面。
- 使用 FastAPI 与 SQLite 搭建后端服务，支持可沙盒化的数据存储与模拟器演示。
- 将后端按 bounded context 拆分为 calendar、tasks、document memory、travel、weather、local services、money 等模块。
- 设计 LLM orchestration 流程，将自然语言请求解析为结构化 action frame，再交由不同能力模块执行。
- 实现 confirmation-first action safety：所有会修改用户数据的操作，例如日历改期、复合日程草稿、旅行行程保存和费用创建，都先生成确认卡片，用户确认后再执行。
- 构建 simulator-based golden journey QA，覆盖 morning brief、天气简报、日程查询、会议改期、文件预览、餐厅推荐、旅行比较、日历验证与费用视图。
- 通过 Codex / AI Coding 工具辅助完成需求拆解、代码迭代、测试回归、UI 体验检查、README 与 Demo 材料准备。

项目亮点：该项目不仅是聊天机器人，而是一个面向真实生活事务的 AI action system，重点展示 AI 如何从“回答问题”进一步走向“理解目标、调用工具、生成可确认操作并修改应用状态”。

### Yuwen-RAG｜RAG 知识检索与问答系统

**项目阶段：原型完成，可开源展示**  
**技术栈：Python、文本解析、向量检索、语义匹配、RAG pipeline**

搭建基于 RAG 的知识检索与问答系统，用于将文档、论文或结构化资料拆解为可检索单元，并通过 query embedding 与相似度匹配实现基于上下文的回答生成。

主要工作：

- 设计文档拆解流程，将长文档切分为可检索的知识片段。
- 使用 embedding / 语义检索思路将 query 与文档片段进行匹配。
- 构建语义检索流程，根据用户问题匹配最相关内容片段。
- 将检索结果与大模型生成能力结合，形成面向问题的回答。
- 为 Jarvis 项目的 document memory 与智能文件预览能力提供技术基础。

### AI Coding / OpenHarness 工作流探索

围绕 AI Coding 工具探索“超级个体”式开发流程，即通过 AI 辅助完成从产品目标、需求澄清、架构拆解、代码生成、调试、测试、文档到 Demo 包装的端到端开发。

主要工作：

- 使用 Codex 辅助进行代码生成、bug 定位、模块重构和测试用例设计。
- 将复杂任务拆分为多个可验证阶段，形成从需求到交付的开发闭环。
- 为 Jarvis 项目设计分层回归流程，包括 20/80 smoke test、targeted scenario test、UX replay review 和 full regression gate。
- 自动生成 README、简历 bullet、展示材料和 demo 脚本，提升工程项目的交付表达能力。

## 工作与实习经历

### Simcenter FlightStream / Siemens｜航空工程实习生

2023.10 – 2024.02｜美国阿拉巴马州奥本市

- 研究并实现 Conway 螺旋桨推进模型，用于替代 FlightStream 软件中原有附圆盘部分布假设。
- 设计可调参数控制模型推力和扭矩条件下的配平算法，并与 FlightStream 仿真平台集成。
- 相关成果于 2024 年 AIAA SciTech 国际会议展示。

### SPACETY｜控制部门实习生

2020.07 – 2020.10｜中国湖南长沙

- 研究并实现基于 LQR 的小卫星姿态控制算法。
- 使用 MATLAB / Simulink 建立卫星动力学模型，完成地球指向与太阳跟踪任务仿真验证。

### DJI 大疆创新｜气动设计实习生

2019.11 – 2020.01｜中国深圳

- 使用 Ansys Fluent 对多种飞行器设计进行气动与飞行动力学仿真评估。
- 参与 RoboMaster 大学生机器人大赛相关技术方案与仿真报告撰写。
- 技术报告发布于 RoboMaster 官方网站，供学生参考学习。

## 论文与研究成果

- Zhang, Y., Ahuja, V., Hartfield, R., & Verstraete, D. (2024). **Mid-Fidelity Numerical Calculation of XV-15 Proprotor.** AIAA SCITECH 2024 Forum.
- Zhang, Y. **GPT is All You Need: A Cognitive and Psychological Perspective on Human-AI Interaction.** Manuscript under review / in preparation.
