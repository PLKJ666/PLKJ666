# Hi, I'm PLKJ666

AI Agent / LLM Application / Full-Stack / Backend Engineer.

我关注的是把真实业务流程变成可运行、可评估、可维护的 AI 应用系统：Agent 工具链、RAG-style 检索、结构化输出、企业 API 集成、异步任务编排、数据工作流和前后端工程化。

I build practical AI application systems around workflow automation, tool backends, retrieval layers, structured outputs, evaluation, and production-oriented full-stack engineering.

## Current Focus

- AI Agent engineering and LLM application infrastructure
- RAG-style retrieval over business data
- Tool Calling, workflow orchestration, and structured outputs
- FastAPI / Next.js / TypeScript / Python full-stack systems
- Enterprise API integration, queues, retries, idempotency, and CI
- Marketing technology workflows: assets, KOL performance, reporting, and writeback
- Speech / TTS fundamentals: FastSpeech2, Mel spectrograms, vocoders, WER, SIM

## Flagship Portfolio Project

### AI Marketing Asset Agent

Status: Private, release-ready, waiting for final public-release decision.

A sanitized AI Agent portfolio project for marketing workflow automation. It demonstrates how an enterprise-style Agent can combine retrieval, business tools, structured outputs, evaluation, frontend demo pages, CI, privacy scanning, screenshots, and demo video.

当前已完成：

- RAG-style marketing asset retrieval
- Tool Calling workflow:
  - `search_materials`
  - `query_kol_performance`
  - `generate_marketing_copy`
  - `create_feishu_doc`
- FastAPI backend with `POST /api/agent/chat`
- Next.js frontend demo:
  - Agent operating console
  - sanitized asset browser
  - evaluation dashboard
- 20-case deterministic evaluation runner
- metrics: intent accuracy, tool selection accuracy, parameter extraction accuracy, retrieval hit rate, task success rate, unsupported answer rate
- screenshots and 36-second demo video
- GitHub Actions CI:
  - backend tests
  - frontend tests/build
  - privacy scan

Boundary:

This is a sanitized portfolio project. It does not contain company source code, internal data, real customer or brand names, Feishu identifiers, object storage buckets, tokens, secrets, or unsanitized screenshots.

## Portfolio Roadmap

### 1. Enterprise Document Workflow Agent

Sanitized reconstruction of a Feishu-style document workflow Agent.

Planned public scope:

- mock Feishu adapter
- command parser
- create doc / sheet / bitable tools
- import URL / markdown / text
- mock ownership transfer
- queue, retry, and idempotency examples
- guide for upgrading fixed commands into LLM Tool Calling

Original experience, summarized safely:

- independently developed and led an internal document automation workflow
- served around 100 users
- processed more than 1,500 content items in about five weeks
- maintained above-99% success rate
- solved document creation quota and handoff bottlenecks within platform rules

### 2. Marketing Asset Archive Platform

Sanitized reconstruction of a full-stack asset upload, archive, permission, and handoff platform.

Planned public scope:

- uploader / receiver / admin surfaces
- local storage or MinIO instead of real object storage
- large-file upload and preview
- permission model
- deduplication
- soft deletion and scheduled cleanup

Original experience, summarized safely:

- independently developed the internal system
- served about 80 active users
- managed more than 1,200 materials
- improved cross-team material handoff, search, management, and long-term access

### 3. KOL Performance Data Agent

Sanitized reconstruction of a Dagster-based marketing data workflow.

Planned public scope:

- mock Feishu Bitable source
- mock external campaign API
- Dagster workflow 1: source sync
- Dagster workflow 2: performance fetch
- Dagster workflow 3: writeback
- project-level KOL filtering
- 30-day tracking window
- API request logs and writeback logs

Original experience, summarized safely:

- independently developed a data pipeline system for KOL campaign tracking
- covered 158 brands and 183 projects
- supported media operations, KOL operations, project managers, client operations, data analysts, and management reporting scenarios

### 4. TTS FastSpeech2 Reproduction

Planned public reproduction project for TTS training, inference, vocoder usage, and speech evaluation.

Planned scope:

- LJSpeech / AISHELL-3 / LibriTTS data preparation notes
- FastSpeech2 training and inference reproduction
- vocoder pipeline notes
- WER, SIM, MCD, F0 RMSE, F0 correlation, RTF, MOS-style subjective rating
- tuning log: sampling rate, text normalization, forced alignment, learning rate, loss weights, speaker embedding, vocoder checkpoint

Boundary:

This will not include Baidu internal code, data, models, logs, or unpublished metrics.

## Tech Stack

### AI / Agent

LLM applications, Tool Calling, RAG-style retrieval, structured outputs, workflow agents, evaluation sets, privacy-safe portfolio reconstruction.

### Backend / Full-Stack

Python, TypeScript, FastAPI, Fastify, Next.js, React, Node.js, Pydantic, PostgreSQL, Redis, BullMQ, Docker.

### Data Workflow

Dagster, SQLAlchemy, Alembic, scheduled jobs, sensors, incremental sync, writeback logs, API request logs.

### Enterprise Integration

Feishu OpenAPI-style integrations, Feishu Bitable-style workflows, webhook bots, external API integration, queue-based orchestration.

### Reliability / Storage

Object storage concepts, presigned URLs, large-file upload, multipart upload, permission control, idempotency, retries, soft deletion, scheduled cleanup.

### Speech / TTS

FastSpeech2, AISHELL, LibriTTS, Mel spectrograms, FFT, vocoders, speaker embeddings, forced alignment, WER, SIM.

## What I Am Building Next

- Make `ai-marketing-asset-agent` public after final license and release checklist.
- Add a hosted preview for the Agent demo.
- Build `enterprise-document-workflow-agent` as the next public sanitized reconstruction.
- Build `marketing-asset-archive-platform` for full-stack asset workflow proof.
- Build `kol-performance-data-agent` for data workflow and marketing analytics proof.
- Build `tts-fastspeech2-reproduction` for speech/TTS roles.

## Privacy and Security Boundary

All public repositories are sanitized reconstructions or portfolio projects using mock data and newly written code.

I do not publish:

- company source code
- internal data
- real customer or brand names
- Feishu links or user identifiers
- object storage buckets
- tokens, secrets, or credentials
- unsanitized screenshots

## Contact

- GitHub: `github.com/PLKJ666`
- Portfolio status: building in public-safe stages
