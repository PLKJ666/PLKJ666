# GitHub Profile Polish Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** 将 Nike 的 GitHub 公开主页优化为身份明确、首屏简洁、项目顺序合理且可由未登录访客验证的个人作品集入口。

**Architecture:** 以 GitHub Profile 仓库 `README.md` 作为内容层，以 GitHub 用户资料和 pinned repositories 作为账号展示层。所有修改基于远端 `main` 最新状态串行执行，最后从未登录访客页面核验三层展示结果。

**Tech Stack:** Markdown、Git、GitHub CLI、GitHub Web UI

---

### Task 1: 压缩 Profile README 首屏

**Files:**
- Modify: `README.md:1-11`

- [ ] **Step 1: 核对远端基线**

Run:

```powershell
git fetch origin main
git status --short --branch
git rev-parse HEAD
git rev-parse origin/main
```

Expected: worktree 无未提交改动，执行前 `HEAD` 与 `origin/main` 一致。

- [ ] **Step 2: 替换首屏文案**

将 `README.md` 开头替换为：

```markdown
# Nike

### AI 应用开发 · 企业工作流 · 全栈后端

把内容生产、企业自动化和营销数据中的人工流程，做成真正可运行、可验证、可维护的 AI 系统。

`3 个公开项目` · `2 个真实上线系统` · `从需求到部署独立交付`

[代表项目](#代表项目) · [交付能力](#交付能力) · [真实案例](#真实案例) · [English](#english)

---
```

- [ ] **Step 3: 验证文档边界**

Run:

```powershell
git diff --check
git diff -- README.md
rg -n "1 条营销数据闭环|开放方向|# PLKJ666" README.md
```

Expected: `git diff --check` 无输出；差异只涉及首屏；最后一个搜索命令无匹配。

- [ ] **Step 4: 提交并推送**

Run:

```powershell
git add README.md docs/superpowers/specs/2026-07-23-github-profile-polish-design.md docs/superpowers/plans/2026-07-23-github-profile-polish.md
git commit -m "docs: 精简 Nike GitHub 主页首屏"
git push origin main
```

Expected: push 成功，远端 `main` 包含首屏优化和过程记录。

### Task 2: 更新 GitHub 账号展示字段

**Files:**
- Modify externally: GitHub account public profile `Name`

- [ ] **Step 1: 设置公开姓名**

Run:

```powershell
gh api --method PATCH user -f name='Nike'
```

Expected: API 返回的 `name` 为 `Nike`。

- [ ] **Step 2: 读取验证**

Run:

```powershell
gh api user --jq '{login,name,bio}'
```

Expected: `login` 为 `PLKJ666`，`name` 为 `Nike`，原 Bio 保持不变。

### Task 3: 调整置顶仓库并做公开验收

**Files:**
- Modify externally: GitHub profile pinned repositories

- [ ] **Step 1: 在 GitHub 主页编辑 pinned repositories**

通过已登录 GitHub 页面进入 `Customize your pins`，只选择以下三个仓库，并按顺序排列：

```text
contentguard-ai
xiaohongshu-ai-content-studio
enterprise-content-workflow
```

Expected: 页面保存后置顶区按该顺序显示三个仓库。

- [ ] **Step 2: 读取 GraphQL 状态**

Run:

```powershell
gh api graphql -f query='query { user(login:"PLKJ666") { pinnedItems(first:6, types:[REPOSITORY]) { nodes { ... on Repository { name } } } } }' --jq '.data.user.pinnedItems.nodes[].name'
```

Expected:

```text
contentguard-ai
xiaohongshu-ai-content-studio
enterprise-content-workflow
```

- [ ] **Step 3: 未登录访客验收**

打开 `https://github.com/PLKJ666`，验证公开姓名、README 首屏、三个置顶仓库及其顺序。

Expected: 页面不依赖登录即可看到全部预期结果；头像保持用户已经修改的版本。

- [ ] **Step 4: 核对仓库最终状态**

Run:

```powershell
git status --short --branch
git rev-parse HEAD
git rev-parse origin/main
```

Expected: worktree 干净，`HEAD` 与 `origin/main` 一致。
