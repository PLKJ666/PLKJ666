# 你好，我是 PLKJ666 / Hi, I'm PLKJ666

我关注如何把企业内容生产、素材流转和营销数据流程中的人工阻塞，转化为可运行、可验证、可维护的业务系统。

I focus on turning manual bottlenecks in enterprise content production, asset workflows, and marketing data processes into business systems that are operational, verifiable, and maintainable.

在 AI 营销科技公司的实习中，我围绕真实内部流程独立完成需求拆解、方案设计、开发、部署和迭代。相比堆叠技术名词，我更关心系统是否真正进入工作流程、谁在使用，以及它是否减少了重复劳动和交付风险。

During my internship at an AI marketing technology company, I independently handled requirement breakdown, solution design, development, deployment, and iteration around real internal workflows. Rather than stacking technical buzzwords, I care more about whether a system actually becomes part of the workflow, who uses it, and whether it reduces repetitive work and delivery risk.

目标方向：AI 应用开发 / AI 全栈 / 后端工程 / 数据工作流。

Target roles: AI application development / AI full-stack / backend engineering / data workflows.

## 精选工程案例 / Selected Engineering Case Studies

这些仓库不是对公司内部系统的复制，而是基于真实业务经验，从零重写的脱敏案例。它们分别证明 AI 应用、企业工作流、内容资产治理和营销数据工程能力。

These repositories are sanitized, from-scratch case studies based on real business experience, not copies of internal company systems. Together they demonstrate AI applications, enterprise workflows, content governance, and marketing data engineering.

| 企业问题 / Enterprise problem | 案例仓库 / Repository | 可验证内容 / Verifiable evidence |
| --- | --- | --- |
| 营销人员如何找素材、查效果、生成文案并形成复盘 / Turning marketing questions into controlled Agent workflows | [`ai-marketing-asset-agent`](https://github.com/PLKJ666/ai-marketing-asset-agent) | FastAPI、Next.js、工具调用轨迹、20 条评估集、CI、演示视频 / tool traces, 20-case evaluation, CI, demo video |
| 跨系统内容创建、导入和所有权移交如何可靠完成 / Reliable cross-system content creation and ownership transfer | [`enterprise-content-workflow`](https://github.com/PLKJ666/enterprise-content-workflow) | 异步状态、幂等、重试、安全回执、64 项测试 / async state, idempotency, retries, safe receipts, 64 tests |
| 营销素材如何控制版本、权限、交付和归档 / Governing asset versions, access, delivery, and archival | [`marketing-asset-delivery-platform`](https://github.com/PLKJ666/marketing-asset-delivery-platform) | 分片上传、SHA-256、项目权限、软删、30 项测试 / multipart upload, project access, soft deletion, 30 tests |
| KOL 投放数据如何增量追踪并回到业务台账 / Incremental KOL performance tracking and business writeback | [`kol-performance-data-agent`](https://github.com/PLKJ666/kol-performance-data-agent) | Dagster assets、SQLite、30 天窗口、回写日志、8 项测试 / Dagster assets, SQLite, 30-day window, writeback evidence, 8 tests |

> 当前案例仓库保持 Private，待最终许可和公开检查完成后再决定可见性；仓库状态不影响下方真实业务经历的事实口径。
>
> The case-study repositories remain Private pending final permission and public-release review. Repository visibility does not change the factual boundaries of the real business experience described below.

## 我解决过的企业问题 / Enterprise Problems I Have Solved

### 企业内容创建与流转 / Enterprise Content Creation and Workflow

**问题 / Problem**

内部人员频繁创建文档、表格和多维表格时，会受到个人创建额度限制；外部内容导入、结果发送和资源所有权交接也依赖人工处理。

When internal staff frequently create documents, spreadsheets, and multidimensional tables, they can be constrained by personal creation quotas. Importing external content, delivering results, and handing over resource ownership also depend on manual processing.

**我负责的工作 / My Responsibilities**

从 0 到 1 独立完成需求分析、方案设计、开发、部署和上线迭代，重新设计资源创建主体与最终所有者之间的关系。

I independently completed requirement analysis, solution design, development, deployment, and post-launch iteration from 0 to 1, redesigning the relationship between the identity that creates a resource and its final owner.

**解决方式 / Solution**

由应用身份统一创建或导入内容，通过异步任务处理耗时操作，完成后自动将资源所有权转移给发起用户；同时加入幂等去重、失败重试、结果回执和运行日志，保障内部持续使用。

An application identity centrally creates or imports content, while asynchronous tasks handle time-consuming operations. After completion, resource ownership is automatically transferred to the requesting user. Idempotent deduplication, failure retries, result receipts, and runtime logs support continued internal use.

**验证结果 / Verified Results**

- 上线约 5 周服务约 100 名独立用户
- Served approximately 100 distinct users over about five weeks after launch
- 成功处理 1,535 份内容
- Successfully processed 1,535 content items
- 按已确认的内部统计口径，整体成功率超过 99%
- Achieved an overall success rate above 99% under the confirmed internal statistical definition
- 在公司及平台允许的规则范围内实施，缓解个人创建额度对业务流程的限制
- Implemented within the rules permitted by the company and platform, easing the impact of personal creation quotas on business workflows

### 营销素材归档与交付 / Marketing Asset Archiving and Delivery

**问题 / Problem**

素材长期分散在个人、群聊和临时链接中，上传方、接收方和管理员需要反复沟通，素材查找、审核、权限控制和长期访问都缺少统一入口。

Assets were scattered across individuals, group chats, and temporary links over time. Uploaders, recipients, and administrators had to communicate repeatedly, while asset discovery, review, access control, and long-term availability lacked a unified entry point.

**我负责的工作 / My Responsibilities**

独立完成内部素材归档与流转平台的产品梳理、三端系统设计、全栈开发、对象存储接入、生产部署和后续维护。

I independently completed product analysis, three-client system design, full-stack development, object storage integration, production deployment, and ongoing maintenance for an internal asset archiving and workflow platform.

**解决方式 / Solution**

把上传、接收、审核、反馈、授权、归档和清理整合为统一流程；针对大文件采用对象存储直传、分片上传和断点恢复，并通过角色与项目范围控制素材访问。

I integrated uploading, receiving, review, feedback, authorization, archiving, and cleanup into one workflow. For large files, the system uses direct-to-object-storage uploads, multipart uploads, and resumable transfers, while roles and project scope control asset access.

**验证结果 / Verified Results**

- 系统进入真实内部生产流程
- The system became part of a real internal production workflow
- 服务约 80 名活跃用户
- Served approximately 80 active users
- 管理 1,200+ 份素材
- Managed more than 1,200 assets
- 将原有逐人、逐群传递素材的方式转为统一线上流程
- Replaced person-by-person and group-by-group asset handoffs with a unified online workflow

### KOL 投放效果数据流转 / KOL Campaign Performance Data Workflow

**问题 / Problem**

营销项目配置、达人执行记录和外部投放效果数据分散在不同系统中。人工查询和回填不仅耗时，也容易出现项目范围混淆、数据遗漏和统计口径不一致。

Marketing project configurations, creator execution records, and external campaign performance data were distributed across different systems. Manual querying and writeback were time-consuming and prone to project-scope confusion, missing data, and inconsistent statistical definitions.

**我负责的工作 / My Responsibilities**

独立设计并开发数据同步、效果拉取和业务回写流程，连接内部业务表与外部营销数据接口。

I independently designed and developed data synchronization, performance retrieval, and business writeback workflows that connect internal business tables with external marketing data APIs.

**解决方式 / Solution**

将项目配置、KOL 执行记录和效果数据组织为可调度的数据管道，按项目范围和追踪周期增量处理，并保留请求日志、回写日志和失败记录供排查。

I organized project configurations, KOL execution records, and performance data into a schedulable data pipeline, processed data incrementally by project scope and tracking period, and retained request logs, writeback logs, and failure records for troubleshooting.

**验证范围 / Verified Scope**

- 覆盖 158 个品牌、183 个项目的业务配置
- Covered business configurations for 158 brands and 183 projects
- 已确认完成至少 100+ 条 KOL/视频效果数据同步与回写，精确数据口径仍待进一步核准
- Confirmed synchronization and writeback of at least 100+ KOL/video performance records; the precise statistical definition still requires further validation
- 支持媒介运营、KOL 运营、项目经理、客户运营、数据分析和管理报表场景
- Supported media operations, KOL operations, project managers, client operations, data analysis, and management reporting scenarios
- 将分散的人工查询与回填转化为可追踪的数据工作流
- Turned fragmented manual querying and writeback into a traceable data workflow

## 个人项目与工程实验 / Personal Projects and Engineering Experiments

### AI Marketing Asset Agent

一个使用脱敏 Mock 数据构建的个人工程实验，用于验证素材检索、结构化工具执行、调用轨迹和离线评估方法。

A personal engineering experiment built with sanitized mock data to validate asset retrieval, structured tool execution, invocation traces, and offline evaluation methods.

它不是上述企业系统的源码，也不代表真实客户部署。当前实现包含 FastAPI 接口、Next.js 演示界面、确定性评估集、CI、隐私扫描、截图和演示视频。

It is not the source code of the enterprise systems described above and does not represent a real customer deployment. The current implementation includes a FastAPI interface, a Next.js demo UI, a deterministic evaluation set, CI, privacy scanning, screenshots, and a demo video.

> 仓库当前为 Private，完成公开许可与最终隐私检查后再决定是否开放。
>
> The repository is currently Private. Whether to make it public will be decided only after public-release permission and a final privacy review are complete.

### ContentGuard AI

我独立开发的营销内容合规审核产品项目，围绕 Brief、脚本、视频、AI 预审和人工终审构建可追踪的内容交付流程。

An independently developed marketing content compliance review product project that builds a traceable content delivery workflow around briefs, scripts, videos, AI pre-review, and final human review.

项目用于展示我对营销内容协作、人机协同审核和完整 AI 应用工程的理解；它属于个人作品集项目，不表述为已服务真实客户的公司生产系统。

The project demonstrates my understanding of marketing content collaboration, human-AI collaborative review, and end-to-end AI application engineering. It is a personal portfolio project and is not represented as a company production system that has served real customers.

> 仓库当前为 Private，可在合适场景下进行演示。
>
> The repository is currently Private and can be demonstrated in appropriate settings.

## 我的工作方式 / How I Work

- 先理解使用者、原流程、业务约束和成功标准，再选择实现方式
- Understand users, the original process, business constraints, and success criteria before choosing an implementation
- 对需要长期运行的流程补充权限、幂等、重试、日志和失败处理
- Add permissions, idempotency, retries, logging, and failure handling to workflows that need to run over the long term
- 用真实使用范围、测试结果和反馈验证交付，不编造指标
- Validate delivery with real usage scope, test results, and feedback without fabricating metrics
- 区分个人贡献、团队成果和公司成果
- Distinguish personal contributions, team outcomes, and company outcomes
- 公开内容只使用脱敏重构、Mock API、示例数据和重新编写的代码
- Use only sanitized reconstructions, mock APIs, sample data, and newly written code in public materials

## 技术能力 / Technical Skills

- **AI 应用：** 内容审核、结构化输出、Tool Calling、RAG-style 检索、评估集、人机协同流程
- **AI applications:** Content review, structured output, Tool Calling, RAG-style retrieval, evaluation sets, and human-AI collaborative workflows
- **后端与工作流：** Python、TypeScript、FastAPI、Fastify、PostgreSQL、Redis、BullMQ、Celery、Dagster
- **Backend and workflows:** Python, TypeScript, FastAPI, Fastify, PostgreSQL, Redis, BullMQ, Celery, and Dagster
- **全栈与企业集成：** Next.js、React、Feishu OpenAPI-style integration、对象存储、大文件上传、权限控制
- **Full-stack and enterprise integration:** Next.js, React, Feishu OpenAPI-style integration, object storage, large-file uploads, and access control
- **工程可靠性：** Docker、CI、异步任务、幂等、重试、日志、数据回写和隐私扫描
- **Engineering reliability:** Docker, CI, asynchronous tasks, idempotency, retries, logging, data writeback, and privacy scanning
- **语音基础：** TTS、FastSpeech2、AISHELL、LibriTTS、Mel Spectrogram、WER、SIM
- **Speech fundamentals:** TTS, FastSpeech2, AISHELL, LibriTTS, Mel Spectrogram, WER, and SIM

## 信息与隐私边界 / Information and Privacy Boundaries

上述企业案例仅保留经过确认的脱敏业务事实，不公开公司源码、内部数据、真实客户或品牌名称、飞书链接或用户标识、对象存储信息、内部域名、凭据和未脱敏截图。

The enterprise cases above retain only confirmed and sanitized business facts. They do not disclose company source code, internal data, real customer or brand names, Feishu links or user identifiers, object storage information, internal domains, credentials, or unsanitized screenshots.

公开仓库中的代码、接口和数据均为重新实现或 Mock 内容，不能与公司内部系统源码等同。

Code, interfaces, and data in public repositories are reimplementations or mock content and must not be treated as equivalent to the source code of internal company systems.

## 联系方式 / Contact

- GitHub：`github.com/PLKJ666`
- GitHub: `github.com/PLKJ666`
- 当前状态：持续沉淀真实业务问题、可验证结果和公开安全的工程案例
- Current status: Continuously documenting real business problems, verifiable results, and engineering case studies that are safe for public disclosure
