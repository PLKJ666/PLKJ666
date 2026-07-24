# Nike

### AI 应用开发 · 企业工作流 · 全栈后端

把内容生产、企业自动化和营销数据中的人工流程，做成真正可运行、可验证、可维护的 AI 系统。

`3 个公开项目` · `2 个真实上线系统` · `从需求到部署独立交付`

[代表项目](#代表项目) · [交付能力](#交付能力) · [真实案例](#真实案例) · [English](#english)

---

## 代表项目

### [ContentGuard AI 内容卫士](https://github.com/PLKJ666/contentguard-ai)

**让营销内容从 Brief、脚本、视频到 AI 预审和人工终审都有明确状态与责任。**

面向品牌、代理商、创作者和运营角色设计的 AI 全栈项目。它把分散的内容版本、审核意见和最终决策收进同一条人机协同流程，并覆盖多租户、异步媒体处理和可追踪交付。

[![ContentGuard AI 内容审核工作台](https://raw.githubusercontent.com/PLKJ666/PLKJ666/main/docs/portfolio/covers/contentguard-ai-cover.png)](https://github.com/PLKJ666/contentguard-ai)

- **关键能力：** 结构化 AI 审核、人机协同决策、多租户权限、异步视频处理、SSE 进度与审计记录
- **技术栈：** FastAPI · Next.js · PostgreSQL · Celery · Redis · Logto
- **公开证据：** 完整产品截图、技术架构、脱敏实现与可执行验证流程

### [小红书 AI 内容创作工作台](https://github.com/PLKJ666/xiaohongshu-ai-content-studio)

**把选题参考、提示词分析、批量生图、花字加工和素材中转连成一条连续生产线。**

[![小红书 AI 内容创作工作台](https://raw.githubusercontent.com/PLKJ666/PLKJ666/main/docs/portfolio/covers/xiaohongshu-ai-content-studio-cover.png)](https://github.com/PLKJ666/xiaohongshu-ai-content-studio)

- **解决问题：** 运营人员不再需要在多个模型、表格和图片工具之间反复切换
- **关键能力：** 多模型适配、批量任务、失败恢复、SSE 增量进度、Canvas 预览与 Pillow 全分辨率输出
- **验证证据：** 918 项后端测试、75 项前端测试、生产构建与隐私扫描
- **技术栈：** FastAPI · React · SQLite · Alembic · Canvas · Pillow

### [企业内容工作流案例](https://github.com/PLKJ666/enterprise-content-workflow)

**让跨系统内容任务在失败、重试和异步执行后，仍只产生一个归属正确、结果明确的业务资源。**

[![企业内容工作流案例](https://raw.githubusercontent.com/PLKJ666/PLKJ666/main/docs/portfolio/covers/enterprise-content-workflow-cover.png)](https://github.com/PLKJ666/enterprise-content-workflow)

- **解决问题：** 创建、导入、所有权移交、幂等重试和异步回执之间缺少统一业务完成标准
- **真实结果：** 原部署约运行 5 周，服务约 100 名独立用户，成功处理 1,535 次内容操作；按已确认内部口径，允许规则范围内成功率超过 99%
- **公开验证：** 从零重写的脱敏 Demo，使用 Mock 适配器和示例数据，通过 64 项测试及完整 CI
- **技术栈：** Fastify · TypeScript · Async Workflow · Idempotency · Retry

---

## 交付能力

- **把模糊需求变成可交付系统：** 梳理使用者、原流程、约束和完成标准，再设计产品与技术方案。
- **把 Demo 推到长期运行：** 补齐权限、队列、幂等、重试、日志、对象存储、回写、部署和故障处理。
- **把 AI 放进受控流程：** 使用结构化输出、工具调用、评估和人工确认，不把模型输出直接当最终业务事实。
- **把成果变成证据：** 以真实使用范围、测试、CI、演示和反馈说明价值，不编造指标。

## 真实案例

<details>
<summary><strong>查看经过脱敏的企业案例</strong></summary>

- **营销素材交付平台：** 解决素材分散、版本和权限不清、大文件交付不稳定及交付后难追溯；原系统约 80 名活跃用户，管理 1,200+ 份素材，我负责三端产品、全栈开发、对象存储与生产部署。
- **KOL 效果数据流程：** 独立设计名单同步、增量拉取、30 天追踪、质量检查和业务回写，减少人工查询与遗漏。
- **AI 营销素材助手：** 用受控工具调用、结构化输出和离线评估连接素材检索、效果查询、文案生成与复盘。
- **企业账号生命周期自动化：** 从零重写多租户、幂等、fencing、Outbox 和凭据安全案例；脱敏版本通过 117 项测试。

</details>

## 公开边界

企业案例只保留经过确认的脱敏业务事实。公开仓库仅使用从零重写的实现、Mock API 和示例数据，不包含公司源码、内部数据、真实客户或品牌名称、人员标识、平台链接、对象存储信息、内部域名、凭据或未脱敏截图。

<a id="english"></a>
<details>
<summary><strong>English profile</strong></summary>

### AI Applications · Enterprise Workflows · Full-stack Backend

I turn operational bottlenecks in content production, business automation, and marketing data into reliable, testable systems. My work focuses on the parts that make AI applications production-ready: permissions, state transitions, ownership, idempotency, retries, human review, delivery evidence, and data write-back.

**Selected work**

- [ContentGuard AI](https://github.com/PLKJ666/contentguard-ai): a multi-role marketing content review platform combining structured AI analysis with human decisions.
- [Xiaohongshu AI Content Studio](https://github.com/PLKJ666/xiaohongshu-ai-content-studio): a continuous workflow for discovery, prompt analysis, batch image generation, visual finishing, and asset distribution.
- [Enterprise Content Workflow](https://github.com/PLKJ666/enterprise-content-workflow): a sanitized case study for reliable cross-system creation, ownership transfer, retries, and asynchronous results.

Open to AI application engineering, full-stack backend roles, and enterprise automation collaboration.

</details>
