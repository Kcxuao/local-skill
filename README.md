# Local Skills

个人常用 AI Agent Skills 与插件集合，同时提供供 ChatGPT / Codex 使用的 Marketplace。

## 已收录

| 插件 | 来源 | 功能 |
| --- | --- | --- |
| [git-workflow](./plugins/git-workflow/skills/git-workflow/SKILL.md) | 自维护 | 独立任务分支管理、中文 Git Commit 规范 |
| [ponytail](https://github.com/DietrichGebert/ponytail) | 第三方 | 强调简洁、最小实现和 YAGNI 的开发工作流 |

Ponytail 通过 Marketplace 引用上游仓库，不在本仓库存放第三方代码；它跟踪上游 `main`，更新前请审查上游变更（包括 Hooks）。

## 安装

将本仓库添加为插件市场：

```bash
codex plugin marketplace add Kcxuao/local-skill
codex plugin marketplace list
```

随后在支持自定义 Marketplace 的 ChatGPT / Codex 插件界面中选择 `Local Skills`，按需安装插件。

## 添加新插件

- 自维护 Skill：放入 `plugins/<plugin-name>/skills/<skill-name>/`，在插件目录添加 `plugin.json`。
- 第三方兼容插件：优先在 [Marketplace 清单](./.agents/plugins/marketplace.json) 添加其 Git 仓库来源；无需复制源码。
- 所有插件统一登记于 `.agents/plugins/marketplace.json`。
