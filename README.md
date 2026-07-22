# PLKJ666

### AI 应用开发 · 企业工作流 · 全栈后端 · 营销数据工程

我把企业内容生产、素材交付和营销数据中的人工阻塞，变成可运行、可验证、可维护的业务系统。关注的不只是“接入模型”，更是权限、状态、所有权、幂等、重试、交付证据和数据回写这些决定系统能否真正落地的环节。

`3 个公开项目` · `2 个真实上线系统` · `1 条营销数据闭环` · `从需求到部署独立交付`

## 公开可查看 / Public projects

### [ContentGuard AI 内容卫士](https://github.com/PLKJ666/contentguard-ai)

**让营销内容从 Brief、脚本、视频到 AI 预审和人工终审都有明确状态与责任。**

面向品牌、代理商、创作者和运营角色设计的个人 AI 全栈项目。它把分散的内容版本、审核意见和最终决策收进同一条人机协同流程，并覆盖多租户、异步媒体处理和可追踪交付。

`AI Content Review` `Human-in-the-loop` `FastAPI` `Next.js` `PostgreSQL` `Celery`

### [小红书 AI 内容创作工作台](https://github.com/PLKJ666/xiaohongshu-ai-content-studio)

**把选题参考、提示词分析、批量生图、花字加工和素材中转连成一条连续生产线。**

这是我独立完成的内容生产工具，不是公司生产系统。公开版本保留完整 FastAPI + React 实现；GitHub Actions 已验证 918 项后端测试、75 项前端测试、生产构建和隐私扫描。

`Content Workflow` `Image Generation` `SSE` `Canvas` `Pillow` `FastAPI` `React`

### [企业内容工作流案例](https://github.com/PLKJ666/enterprise-content-workflow)

**让跨系统内容任务在失败、重试和异步执行后，仍只产生一个归属正确、结果明确的业务资源。**

公开仓库是基于真实企业内容自动化经历从零重写的脱敏案例，展示创建与导入、所有权移交、幂等、重试、异步状态和安全回执。原部署约运行 5 周，服务约 100 名独立用户，成功处理 1,535 次内容操作；按已确认内部口径，允许规则范围内成功率超过 99%。公开 Demo 已通过 64 项测试及完整 CI。

`Async Workflow` `Idempotency` `Retry` `Ownership Transfer` `Fastify` `TypeScript`

## 私有案例 / Private case studies

这些仓库保留为 Private，用于保护实现边界；这里仅展示经过脱敏、可以对外说明的业务问题与个人贡献。

| 案例 | 解决的问题 | 已确认结果 |
| --- | --- | --- |
| `marketing-asset-delivery-platform` | 素材分散、版本与权限不清、大文件交付不稳定、交付后难追溯 | 原系统约 80 名活跃用户，管理 1,200+ 份素材；我完成三端产品、全栈开发、对象存储与生产部署 |
| `kol-performance-data-agent` | KOL 效果数据分散在项目台账与平台接口，人工查询和回写容易遗漏 | 独立设计名单同步、增量拉取、30 天追踪、质量检查和业务回写流程 |
| `ai-marketing-asset-agent` | 素材检索、效果查询、文案生成和复盘文档彼此割裂 | 用受控工具调用、结构化输出和离线评估验证营销运营 Agent 工作流 |
| `enterprise-account-lifecycle-automation` | 入职、离职和额度审批跨系统执行，容易重复开户、漏停账号、重复加额和泄露临时凭据 | 独立完成真实系统，并从零重写多租户、幂等、fencing、Outbox 和凭据安全案例；Private 仓库已通过 117 项测试 |
| `dolphin-avss-reproduction` | 视听语音分离复现与新结构实验缺少完整训练、评估和对照链路 | 独立完成远程 GPU 训练与 LRS2 基线评估，设计 speech/noise 竞争双支路实验 |

## 我能负责什么

- **把模糊需求变成可交付系统：**梳理使用者、原流程、约束和完成标准，再设计产品与技术方案。
- **把 Demo 推到长期运行：**补齐权限、队列、幂等、重试、日志、对象存储、回写、部署和故障处理。
- **把 AI 放进受控流程：**使用结构化输出、工具调用、评估和人工确认，不把模型输出直接当最终业务事实。
- **把成果变成证据：**以真实使用范围、测试、CI、演示和反馈说明价值，不编造指标。

## 公开边界

企业案例只保留经过确认的脱敏业务事实。公开仓库仅使用从零重写的实现、Mock API 和示例数据，不包含公司源码、内部数据、真实客户或品牌名称、人员标识、平台链接、对象存储信息、内部域名、凭据或未脱敏截图。

<details>
<summary><strong>English profile</strong></summary>

### AI applications · Enterprise workflows · Full-stack backend · Marketing data engineering

I turn manual bottlenecks in enterprise content, asset delivery, and marketing data operations into systems that are operational, verifiable, and maintainable. My work focuses on the controls a generic AI button does not provide by itself: permissions, workflow state, ownership, idempotency, retries, delivery evidence, and data writeback.

**Public projects**

- [ContentGuard AI](https://github.com/PLKJ666/contentguard-ai): a personal human-in-the-loop platform for traceable marketing content review across briefs, scripts, video, AI pre-checks, and final human decisions.
- [Xiaohongshu AI Content Studio](https://github.com/PLKJ666/xiaohongshu-ai-content-studio): an end-to-end workspace for reference discovery, prompt analysis, batch image generation, visual finishing, and asset handoff.
- [Enterprise Content Workflow](https://github.com/PLKJ666/enterprise-content-workflow): a sanitized, from-scratch case study of reliable creation/import, ownership transfer, idempotency, retries, and bounded asynchronous receipts.

**Private case studies** cover enterprise asset delivery, KOL performance data workflows, a controlled marketing operations Agent, employee account lifecycle automation, and audio-visual speech separation research. Their repositories remain private; only sanitized business problems, personal responsibilities, and verified outcomes are described publicly.

Public repositories contain newly written implementations, mock APIs, and synthetic data. They do not contain company source code, customer data, credentials, or private integrations.

</details>
