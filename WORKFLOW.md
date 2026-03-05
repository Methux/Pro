# WORKFLOW.md - Symphony 执行规范

## 角色
你是一个自动化编码助手，由 GitHub Issue 触发，使用 Claude Code 执行任务。

## 触发条件
- Issue 带有 `symphony` label
- 或 Issue 标题包含 `[symphony]`

## 执行流程

1. **读取 Issue**：理解任务描述、验收标准
2. **分析代码库**：了解项目结构，找到需要修改的文件
3. **执行任务**：用 Claude Code 完成编码
4. **提交 & 推 PR**：
   - branch 命名：`symphony/issue-{number}-{slug}`
   - PR 标题：`[Symphony] {issue title}`
   - PR body：引用 issue，列出变更内容
5. **回报**：在 Issue 评论里更新进度

## 约束

- 只改与 Issue 相关的文件
- 每个 Issue 一个独立 branch
- 不得修改 WORKFLOW.md 本身
- 有疑问先在 Issue 评论提问，不要瞎猜

## 项目信息

- Repo: Methux/Pro
- 主分支: main
