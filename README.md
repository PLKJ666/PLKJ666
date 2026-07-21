# PLKJ666

### AI 应用开发 · AI 全栈 · 后端工程 · 营销数据工作流

我关注的不是给产品套一层 AI，而是把企业内容生产、素材流转和营销数据中的人工阻塞，变成真正可运行、可验证、可维护的业务系统。

在 AI 营销科技实习中，我围绕真实内部流程完成需求拆解、方案设计、开发部署和上线迭代；在个人项目中，我继续验证 Agent 工具调用、内容审核、人机协同和可重复评估。

## 精选项目

### [`ai-marketing-asset-agent`](https://github.com/PLKJ666/ai-marketing-asset-agent)

**营销运营工作流 Agent**

把找素材、查 KOL 效果、生成营销文案和形成复盘文档连接为可追踪的 Agent 工作流。项目包含受控工具调用、结构化输出、20 条离线评估集、FastAPI、Next.js、CI、截图和演示视频。

`RAG-style retrieval` `Tool Calling` `Structured Output` `Evaluation` `FastAPI` `Next.js`

---

### [`enterprise-content-workflow`](https://github.com/PLKJ666/enterprise-content-workflow)

**企业内容创建与流转自动化**

解决内容创建额度、外部内容导入和资源所有权移交依赖人工的问题。通过应用身份、异步任务、幂等、失败重试和安全回执，让跨系统任务在重复请求和异常之后仍然只产生一个归属正确、结果明确的业务资源。

原业务系统上线约 5 周，服务约 100 名独立用户，成功处理 1,535 次内容操作；按已确认内部口径，允许规则范围内成功率超过 99%。公开仓库为从零脱敏重写，包含 64 项测试。

`Async Workflow` `Idempotency` `Retry` `Ownership Transfer` `TypeScript`

---

### [`marketing-asset-delivery-platform`](https://github.com/PLKJ666/marketing-asset-delivery-platform)

**企业营销素材版本、权限、交付与归档控制系统**

解决素材分散、版本混乱、客户拿错版本、大文件交付不稳定和交付后无法追溯的问题。真实系统完成上传、预览、查重、权限、反馈、分享、回收和交付链路；公开仓库验证分片上传、服务端校验、项目权限、软删除和生命周期控制。

原内部部署约投入 40 天，于 2026 年初上线，服务约 80 名活跃用户，管理 1,200+ 份素材。公开仓库包含 30 项测试和完整隐私扫描。

`Multipart Upload` `Object Storage` `Authorization` `Lifecycle` `Fastify`

---

### [`kol-performance-data-agent`](https://github.com/PLKJ666/kol-performance-data-agent)

**KOL 投放效果采集、追踪与业务回写闭环**

把分散在项目台账、平台接口和人工记录中的投放数据，整理成“项目名单同步 → 效果增量拉取 → 30 天追踪 → 数据质量检查 → 业务回写”的可观察数据工作流。

公开仓库包含 Dagster assets、SQLite 持久化、分页重试、项目过滤、增量幂等、请求/回写日志、8 项测试、Docker 和已通过的 GitHub Actions。

`Dagster` `Data Pipeline` `Incremental Sync` `SQLite` `Writeback`

---

### [`contentguard-ai`](https://github.com/PLKJ666/contentguard-ai)

**营销内容合规审核平台**

围绕 Brief、脚本、视频、AI 预审和人工终审构建可追踪的内容交付流程，探索品牌、代理商和创作者之间的人机协同审核。它是独立个人项目，不表述为真实客户生产系统。

`Content Moderation` `Human-in-the-loop` `FastAPI` `Next.js` `PostgreSQL`

## 我解决过的真实问题

| 业务问题 | 我的工作 | 可验证结果 |
| --- | --- | --- |
| 内容创建、导入和所有权移交依赖人工 | 从 0 到 1 设计、开发、部署企业内容工作流 | 约 100 名用户、1,535 次成功操作、成功率 99%+ |
| 素材分散、版本和权限不清、大文件难交付 | 完成三端产品设计、全栈开发、对象存储与生产部署 | 约 80 名活跃用户、1,200+ 份素材 |
| KOL 效果查询和回写分散、口径不一致 | 设计同步、效果拉取、增量追踪和业务回写管道 | 覆盖多项目配置并完成真实数据同步与回写 |

以上数据均为经过确认的脱敏历史口径，不代表公开 Demo 的性能或采用率。

## 我的工作方式

- 先理解使用者、原流程、业务约束和成功标准，再选择技术方案。
- 对长期运行的流程补齐权限、幂等、重试、日志、回写和失败处理。
- 用真实使用范围、测试、CI、演示和反馈证明结果，不编造指标。
- 区分个人贡献、团队成果和公司成果。
- 公开内容只使用脱敏重构、Mock API、示例数据和重新编写的代码。

## 技术方向

`Python` `TypeScript` `FastAPI` `Fastify` `Next.js` `React` `PostgreSQL` `SQLite` `Redis` `Dagster` `Docker` `GitHub Actions`

`LLM Application` `RAG-style Retrieval` `Tool Calling` `Structured Output` `Evaluation` `Human-in-the-loop`

`Async Workflow` `Idempotency` `Retry` `Object Storage` `Data Pipeline` `Observability`

## 公开边界

企业案例仅保留经过确认的脱敏业务事实。公开仓库不包含公司源码、内部数据、真实客户或品牌名称、用户标识、飞书链接、对象存储信息、内部域名、凭据或未脱敏截图。

当前部分案例仓库保持 Private，待最终许可和公开检查完成后再决定可见性。

<details>
<summary><strong>English Profile</strong></summary>

### AI Application · Full-Stack · Backend · Marketing Data Workflows

I build operational, verifiable, and maintainable systems for enterprise content production, asset delivery, and marketing data workflows. My work focuses on the parts that generic AI buttons do not replace automatically: permissions, workflow state, ownership, delivery evidence, data contracts, retries, and evaluation.

Selected work includes:

- **AI Marketing Asset Agent:** controlled retrieval and tools for asset search, KOL performance queries, copy generation, review documents, and offline evaluation.
- **Enterprise Content Workflow:** reliable content creation/import, ownership transfer, idempotency, retries, and asynchronous receipts.
- **Marketing Asset Delivery Platform:** large-file upload, scoped authorization, deduplication, controlled delivery, and asset lifecycle management.
- **KOL Performance Data Agent:** incremental campaign tracking, 30-day windows, data-quality gates, Dagster orchestration, and business writeback.
- **ContentGuard AI:** a personal human-in-the-loop marketing content compliance platform.

Public repositories use sanitized reconstructions, mock APIs, synthetic data, and newly written code. They do not contain company source code, customer data, credentials, or private integrations.

</details>
