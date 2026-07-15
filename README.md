# 你好，我是 PLKJ666

方向：AI Agent / 大模型应用开发 / AI 全栈 / 后端工程 / 数据工作流。

我主要关注一件事：把真实业务流程做成可运行、可评估、可维护的 AI 应用系统。

目前重点沉淀的是 Agent 工具链、RAG-style 检索、结构化输出、企业 API 集成、异步任务编排、数据工作流和前后端工程化。

English keywords: AI Agent Engineering, LLM Application, Full-Stack Development, Backend Engineering, Data Workflow.

## 当前关注方向

- AI Agent 工程化与大模型应用基础设施
- 面向业务数据的 RAG-style 检索
- Tool Calling、任务编排、结构化输出和工具调用轨迹
- FastAPI / Next.js / TypeScript / Python 全栈系统
- 企业 API 集成、队列、重试、幂等、CI 和隐私扫描
- AI 营销科技场景：素材管理、KOL 投放数据、复盘报告、数据回写
- 语音 / TTS 基础：FastSpeech2、Mel 频谱、声码器、WER、SIM

## 核心作品集项目

### AI Marketing Asset Agent

状态：私有仓库，已完成公开前主要工程化准备，等待最终 License 和公开决策。

这是一个面向 AI 营销运营场景的脱敏版 Agent 作品集项目，用来展示企业级 Agent 应用的工程结构：素材检索、业务工具调用、结构化输出、评估集、前端 Demo、CI、隐私扫描、截图和 Demo 视频。

已完成能力：

- RAG-style 营销素材检索
- Tool Calling 工作流：
  - `search_materials`
  - `query_kol_performance`
  - `generate_marketing_copy`
  - `create_feishu_doc`
- FastAPI 后端接口：`POST /api/agent/chat`
- Next.js 前端 Demo：
  - Agent 控制台
  - 脱敏素材浏览页
  - 评估 Dashboard
- 20 条 deterministic evaluation cases
- 评估指标：
  - intent accuracy
  - tool selection accuracy
  - parameter extraction accuracy
  - retrieval hit rate
  - task success rate
  - unsupported answer rate
- README 截图和 36 秒 Demo 视频
- GitHub Actions CI：
  - 后端测试
  - 前端测试和构建
  - 隐私扫描

边界说明：

这个项目是脱敏作品集项目，不包含公司源码、内部数据、真实客户或品牌名称、飞书标识、对象存储 bucket、token、secret 或未脱敏截图。

## 作品集路线图

### 1. Enterprise Document Workflow Agent

定位：企业文档工作流 Agent 的脱敏复刻版。

计划公开内容：

- Mock Feishu adapter
- command parser
- 文档 / 表格 / 多维表格创建工具
- URL / Markdown / Text 导入工具
- mock ownership transfer
- queue / retry / idempotency 示例
- 从固定命令升级到 LLM Tool Calling 的说明

原始经历的安全摘要：

- 独立开发并主导内部文档自动化工作流
- 服务约 100 名内部用户
- 约五周内处理 1,500+ 内容项
- 成功率保持在 99% 以上
- 在平台规则允许范围内解决个人文档创建额度和交接效率问题

### 2. Marketing Asset Archive Platform

定位：营销素材上传、归档、权限和交接平台的脱敏复刻版。

计划公开内容：

- 上传方 / 接收方 / 管理员三端
- 使用本地存储或 MinIO 替代真实对象存储
- 大文件上传和在线预览
- 权限模型
- 素材查重
- 软删除和定时清理

原始经历的安全摘要：

- 独立开发内部素材管理系统
- 服务约 80 名活跃用户
- 管理 1,200+ 素材
- 提升跨团队素材交接、查找、管理和长期访问效率

### 3. KOL Performance Data Agent

定位：基于 Dagster 的营销数据工作流 Agent 脱敏复刻版。

计划公开内容：

- Mock Feishu Bitable source
- Mock external campaign API
- Dagster workflow 1：来源同步
- Dagster workflow 2：效果数据拉取
- Dagster workflow 3：数据回写
- 项目内 KOL 过滤
- 30 天 tracking window
- API 请求日志和回写日志

原始经历的安全摘要：

- 独立开发 KOL 投放效果数据管道系统
- 覆盖 158 个品牌、183 个项目
- 支持媒介运营、KOL 运营、项目经理、客户运营、数据分析和管理层报表场景

### 4. TTS FastSpeech2 Reproduction

定位：面向语音 / TTS 岗位的公开复现项目。

计划公开内容：

- LJSpeech / AISHELL-3 / LibriTTS 数据准备说明
- FastSpeech2 训练和推理复现
- vocoder 链路说明
- WER、SIM、MCD、F0 RMSE、F0 correlation、RTF、MOS-style subjective rating
- 调优记录：采样率、文本规范化、forced alignment、learning rate、loss weights、speaker embedding、vocoder checkpoint

边界说明：

该项目不会包含百度内部代码、内部数据、内部模型、内部日志或未公开指标。

## 技术栈

### AI / Agent

大模型应用、Tool Calling、RAG-style 检索、结构化输出、工作流 Agent、评估集、脱敏作品集重构。

### 后端 / 全栈

Python、TypeScript、FastAPI、Fastify、Next.js、React、Node.js、Pydantic、PostgreSQL、Redis、BullMQ、Docker。

### 数据工作流

Dagster、SQLAlchemy、Alembic、scheduled jobs、sensors、incremental sync、writeback logs、API request logs。

### 企业集成

Feishu OpenAPI-style integrations、Feishu Bitable-style workflows、webhook bots、external API integration、queue-based orchestration。

### 稳定性 / 存储

对象存储概念、presigned URLs、大文件上传、multipart upload、权限控制、幂等、重试、软删除、定时清理。

### 语音 / TTS

FastSpeech2、AISHELL、LibriTTS、Mel spectrograms、FFT、vocoders、speaker embeddings、forced alignment、WER、SIM。

## 接下来会做什么

- `ai-marketing-asset-agent` 完成 License 和公开检查后再改 Public。
- 给 Agent Demo 增加 hosted preview。
- 继续做 `enterprise-document-workflow-agent` 脱敏复刻。
- 继续做 `marketing-asset-archive-platform` 脱敏复刻。
- 继续做 `kol-performance-data-agent` 脱敏复刻。
- 继续做 `tts-fastspeech2-reproduction` 语音方向复现项目。

## 隐私和安全边界

所有公开仓库都只使用脱敏重构、Mock API、示例数据和重新编写的代码。

我不会公开：

- 公司源码
- 内部数据
- 真实客户或品牌名称
- 飞书链接或用户标识
- 对象存储 bucket
- token、secret 或 credentials
- 未脱敏截图

## 联系方式

- GitHub：`github.com/PLKJ666`
- 当前状态：正在以公开安全的方式构建作品集
