---
name: git-workflow
description: 管理 Git 开发工作流。开始新的独立开发任务时，自动创建或复用任务分支；用户要求提交代码或生成提交日志时，按约定生成中文提交信息。普通只读分析不创建分支。
---

# Git Workflow

根据任务意图加载对应流程，避免执行无关 Git 操作。

## 能力

- **Branch**：开始独立开发任务，或明确要求创建、切换分支时，先阅读 [references/branch.md](references/branch.md)，在修改代码前准备分支。同一任务的后续修改复用原分支。
- **Commit**：用户要求提交代码或生成提交信息时，阅读 [references/commit.md](references/commit.md)。仅生成信息时不执行写操作。

## 通用原则

- 新独立任务默认授权按 Branch 流程创建**本地分支**，但不代表授权 Commit、Push、Merge、删除分支或改写历史。
- 保留用户已有代码修改及暂存状态；遇到无法安全操作或无法确定目标的情况先询问。
- 遵循项目约定和用户明确指令；基于实际 Git 状态执行，仅报告已完成的操作。
