# Methux Pro

Symphony AI 自动化编码系统。

## 简介

Methux Pro 是一个由 Symphony AI 驱动的自动化编码项目。通过将 Linear issue 与 Claude Code 集成，实现从任务描述到代码提交的全自动工作流。

## 使用流程

1. **创建 Linear Issue** — 在 Linear 中描述需求和验收标准
2. **Claude Code 执行** — Symphony 自动触发 Claude Code，分析代码库并实现变更
3. **自动提交 PR** — 完成后自动创建 Pull Request，关联对应 issue

整个流程无需人工编码干预，Issue 进 → PR 出。

## 技术栈

- **Node.js** — 运行时环境
- **Claude Code** — AI 编码引擎
- **GitHub Actions** — CI/CD 自动化流水线
