# copilot-help

这是一个面向 VS Code GitHub Copilot 的中文实践仓库，重点不是单独介绍某个按钮，而是说明如何把 Copilot 用到中大型项目开发中。

## 快速开始

如果你第一次进入这个仓库，建议按下面顺序开始：

1. 先看 [docs/当前版本-v1-说明.md](docs/当前版本-v1-说明.md)
2. 再看 [docs/guides/如何在-VS-Code-中使用这些-Copilot-模板.md](docs/guides/如何在-VS-Code-中使用这些-Copilot-模板.md)
3. 如果要接入真实项目，接着看 [docs/guides/如何把这套-Copilot-模板接入真实项目.md](docs/guides/如何把这套-Copilot-模板接入真实项目.md)
4. 如果你只想先试最小组合，优先使用：`feature-plan`、`code-review`、`bugfix`、`pr-description`、`planner`

## 前置条件

使用这套模板前，默认你具备：

- 较新的 VS Code 版本
- 已启用 GitHub Copilot Chat / Agents 相关能力
- 工作区已信任
- 了解 `.github/` 下的 prompts、agents、skills、instructions 会被 VS Code 用作 Copilot 自定义资产

## 当前版本

当前建议将这个仓库视为 `v1`。

这一版的定位不是继续无限扩文件，而是先形成一套可用的中文 Copilot 实战模板库，然后进入真实项目验证阶段。

- 版本状态：`v1` 可用
- 当前重点：教程、模板、Agents、Skills、落地指南
- 下一阶段目标：在真实项目里试跑并基于反馈迭代
- 正式发布：`v1.0.0`

## 仓库内容

- [docs/当前版本-v1-说明.md](docs/当前版本-v1-说明.md)
- [docs/VSCode-GitHub-Copilot-大型项目使用教程.md](docs/VSCode-GitHub-Copilot-大型项目使用教程.md)
- [.github/copilot-instructions.md](.github/copilot-instructions.md)
- [.github/instructions/docs.instructions.md](.github/instructions/docs.instructions.md)
- [.github/instructions/customization.instructions.md](.github/instructions/customization.instructions.md)
- [.github/prompts/feature-plan.prompt.md](.github/prompts/feature-plan.prompt.md)
- [.github/prompts/code-review.prompt.md](.github/prompts/code-review.prompt.md)
- [.github/prompts/bugfix.prompt.md](.github/prompts/bugfix.prompt.md)
- [.github/prompts/pr-description.prompt.md](.github/prompts/pr-description.prompt.md)
- [.github/prompts/requirement-review.prompt.md](.github/prompts/requirement-review.prompt.md)
- [.github/prompts/api-design.prompt.md](.github/prompts/api-design.prompt.md)
- [.github/prompts/release-notes.prompt.md](.github/prompts/release-notes.prompt.md)
- [.github/prompts/rollback-plan.prompt.md](.github/prompts/rollback-plan.prompt.md)
- [.github/prompts/architecture-review.prompt.md](.github/prompts/architecture-review.prompt.md)
- [.github/prompts/migration-plan.prompt.md](.github/prompts/migration-plan.prompt.md)
- [.github/prompts/standup-update.prompt.md](.github/prompts/standup-update.prompt.md)
- [.github/prompts/retrospective.prompt.md](.github/prompts/retrospective.prompt.md)
- [.github/prompts/test-generation.prompt.md](.github/prompts/test-generation.prompt.md)
- [.github/prompts/task-breakdown.prompt.md](.github/prompts/task-breakdown.prompt.md)
- [.github/agents/reviewer.agent.md](.github/agents/reviewer.agent.md)
- [.github/agents/planner.agent.md](.github/agents/planner.agent.md)
- [.github/agents/doc-writer.agent.md](.github/agents/doc-writer.agent.md)
- [.github/agents/release-checker.agent.md](.github/agents/release-checker.agent.md)
- [.github/skills/feature-delivery/SKILL.md](.github/skills/feature-delivery/SKILL.md)
- [.github/skills/release-workflow/SKILL.md](.github/skills/release-workflow/SKILL.md)
- [docs/guides/如何在-VS-Code-中使用这些-Copilot-模板.md](docs/guides/如何在-VS-Code-中使用这些-Copilot-模板.md)
- [docs/guides/如何把这套-Copilot-模板接入真实项目.md](docs/guides/如何把这套-Copilot-模板接入真实项目.md)

## 这份教程覆盖什么

- VS Code 中 GitHub Copilot 的核心能力
- Ask、Plan、Agent 的使用区别
- 大型项目的高效工作流
- Agent 执行 SOP
- 提示词写法与可复用模板
- 团队级落地方式
- 常见误区与成熟度路线图

## 适合谁

- 已经安装 GitHub Copilot，但还没有系统化使用的人
- 想把 Copilot 从补全工具升级成项目协作助手的人
- 正在做中大型项目，希望建立更高效 AI 开发工作流的人

## 推荐阅读方式

1. 先看教程开头的“先看这页”
2. 再看模式选择、30 分钟上手路线
3. 接着看大型项目工作流和 Agent 执行 SOP
4. 最后按自己的项目情况复用提示词模板

## 推荐仓库结构

- README.md：仓库入口与导航
- docs/：教程和长期文档
- .github/copilot-instructions.md：项目级 Copilot 约束
- .github/instructions/：文件级或主题级规则
- .github/prompts/：高频提示模板
- .github/agents/：可复用的定制 Agent

## 仓库定位

这个仓库目前以教程文档为主，后续可以继续扩展为：

- Copilot 指令文件示例
- Prompt 模板集合
- 团队规范骨架
- Agent/Skill/MCP 的落地样例

## 当前已内置的 Copilot 资产

### Prompts

- `feature-plan`：为大型功能生成实施计划
- `code-review`：从审查视角检查改动
- `bugfix`：定位根因并做最小修复
- `pr-description`：生成 PR 描述
- `requirement-review`：评审需求完整性、边界和风险
- `api-design`：设计接口契约、输入输出和约束
- `release-notes`：整理发布说明和变更摘要
- `rollback-plan`：生成回滚策略和风险提示
- `architecture-review`：从架构视角检查设计合理性和边界
- `migration-plan`：生成迁移计划、影响范围和验证步骤
- `standup-update`：生成日报或站会更新
- `retrospective`：生成复盘总结、问题清单和改进项
- `test-generation`：补测试和验证范围
- `task-breakdown`：把大任务拆成多个可执行步骤

### Instructions

- `copilot-instructions`：仓库级总规则
- `docs.instructions`：文档类内容的写法和质量要求
- `customization.instructions`：定制 Copilot 文件时的写法和落点要求

### Agents

- `reviewer`：聚焦问题清单、风险和测试缺口
- `planner`：聚焦任务拆解、模块影响和验证路径
- `doc-writer`：聚焦文档整理、教程和交付说明
- `release-checker`：聚焦发布前检查、风险和回滚准备

### Skills

- `feature-delivery`：把“分析需求 -> 规划 -> 执行 -> 验证 -> 交付说明”串成一个完整工作流
- `release-workflow`：把“发布检查 -> 发布说明 -> 风险评估 -> 回滚准备”串成一个完整工作流

## 使用说明

- [如何在 VS Code 中使用这些 Copilot 模板](docs/guides/如何在-VS-Code-中使用这些-Copilot-模板.md)
- [如何把这套 Copilot 模板接入真实项目](docs/guides/如何把这套-Copilot-模板接入真实项目.md)

## 版本与发布

- [CHANGELOG.md](CHANGELOG.md)
- [docs/releases/v1.0.0.md](docs/releases/v1.0.0.md)
- 当前正式版本：`v1.0.0`

## 当前版本建议

如果你现在要使用这个仓库，不建议继续无目标扩展，而建议：

1. 先把当前版本作为 `v1` 冻结
2. 选一个真实项目试接入
3. 只挑 3 到 5 个高频 prompts 开始使用
4. 根据实际使用反馈再继续增补模板

## 许可证与贡献

- [LICENSE](LICENSE)
- [CONTRIBUTING.md](CONTRIBUTING.md)

## GitHub 仓库

- 仓库地址：https://github.com/Sun2080/copilot-help
