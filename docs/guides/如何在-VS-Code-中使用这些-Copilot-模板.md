# 如何在 VS Code 中使用这些 Copilot 模板

这份说明文档回答一个实际问题：仓库里已经有 prompts、agents、instructions 和 skill 了，接下来在 VS Code 里应该怎么用。

## 先理解这几类资产分别做什么

### Instructions

Instructions 是长期规则。

它的作用是告诉 Copilot：在这个仓库里，什么内容应该怎么写，哪些规则需要长期遵守。

例如：

- 文档要用简体中文
- README 负责导航
- Prompt 要写清输入和输出

### Prompts

Prompts 是单次任务模板。

它适合：

- 做功能规划
- 做代码审查
- 生成 PR 描述
- 做需求评审
- 设计接口

### Agents

Agents 是特定角色。

它适合：

- 让一个角色长期保持固定输出风格
- 把“规划”“审查”“文档整理”“发布检查”这类工作固定下来

### Skills

Skills 是多步骤工作流。

它适合：

- 把多个 prompt、agent 和固定步骤组合起来
- 处理功能交付这类不是一句话就能做完的任务

## 在 VS Code 里怎么用

### 1. 使用 Prompt 模板

在 Chat 中输入 `/`，然后选择对应 prompt。

例如：

- `/feature-plan`
- `/code-review`
- `/bugfix`
- `/api-design`
- `/release-notes`

如果 VS Code 已正确发现这些文件，它们会出现在可选列表里。

### 2. 使用 Agent

打开 Chat 后，在 Agent 选择器里切换到自定义 Agent。

例如：

- `planner`
- `reviewer`
- `doc-writer`
- `release-checker`

适合在进入一个明确工作阶段时使用。

### 3. 使用 Skill

如果 Skill 被正确发现，通常也可以通过 `/` 触发。

这个仓库中的 `feature-delivery` 适合在你要做一个完整功能时使用。

### 4. 什么时候该用哪一种

可以按下面这个简单规则来判断：

- 长期规则，用 Instructions
- 单次任务，用 Prompt
- 固定角色，用 Agent
- 多步骤工作流，用 Skill

## 推荐使用顺序

如果你在做一个中大型功能，建议按这个顺序：

1. 先用 `requirement-review` 看需求是否完整
2. 再用 `feature-plan` 或 `task-breakdown` 拆解任务
3. 需要方案评审时，用 `planner` 或 `architecture-review`
4. 开始改动后，用 `reviewer` 做审查
5. 提交前，用 `pr-description`、`release-notes`、`rollback-plan` 补齐交付信息

## 如果 VS Code 没有发现这些模板怎么办

优先检查这几项：

1. 文件是否在正确目录
2. frontmatter 是否合法
3. `description` 是否明确
4. 工作区是否信任
5. VS Code 和 Copilot 是否是较新版本

## 最后建议

不要一开始就把所有模板都用上。

建议你先固定使用这 4 个：

1. `feature-plan`
2. `code-review`
3. `bugfix`
4. `pr-description`

等你已经形成稳定习惯后，再继续引入 agents 和 skill。
