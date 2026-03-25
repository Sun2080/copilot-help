# Contributing

欢迎对这个仓库提出改进建议。

这个仓库的定位不是泛泛介绍 GitHub Copilot，而是沉淀面向 VS Code 场景、中大型项目工作流的中文可复用资产。

## 适合贡献什么

优先欢迎这几类贡献：

- 修正文档中的错误、死链和不清晰表达
- 增加真实项目验证后的优化建议
- 新增高频 Prompt、Agent、Skill 模板
- 补充使用说明、落地 SOP、常见误区

## 不建议的贡献方式

- 只增加一个模板名称，但没有说明使用场景
- 与 VS Code GitHub Copilot 实战无关的内容
- 纯概念介绍，没有工程落地价值的文档
- 没有真实问题支撑、只是为了“更完整”而增加模板数量

## 提交前建议检查

1. 是否说明了适用场景、边界和风险
2. 是否能直接复制使用，而不是只讲概念
3. 是否与仓库现有文件定位重复
4. 如果是自定义文件，frontmatter 是否合法，`description` 是否明确

## 自定义文件放置规则

- 项目级规则：`.github/copilot-instructions.md`
- 文件级规则：`.github/instructions/`
- Prompt：`.github/prompts/`
- Agent：`.github/agents/`
- Skill：`.github/skills/`
- 长文档：`docs/`

## 推荐提交方式

如果你准备新增模板，建议在说明中一并回答：

1. 这个模板解决什么问题
2. 它适合谁用
3. 与现有模板相比新增了什么价值
4. 有没有真实项目或场景验证依据
