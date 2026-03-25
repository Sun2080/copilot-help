---
description: "Use when: creating or updating Copilot customization files such as .prompt.md, .agent.md, .instructions.md, or copilot-instructions.md in this workspace."
applyTo: ".github/**/*.md"
---

# Copilot 定制文件规则

适用于本仓库中的 prompt、agent 和 instruction 文件。

## 通用要求

- description 必须明确写出 Use when 触发语义，方便 Copilot 发现
- frontmatter 使用合法 YAML，避免未转义冒号
- 文件名要体现用途，避免过于泛化
- 内容围绕 VS Code GitHub Copilot 实战，不写无关主题

## Prompt 要求

- 适合单次任务，目标明确
- 尽量写清输入、输出格式和限制条件
- 优先覆盖高频工作流，例如规划、审查、修复、测试、PR

## Agent 要求

- 角色边界清楚，不要让一个 Agent 同时承担过多职责
- description 中直接写出适用场景和触发关键词
- 优先聚焦“规划”“审查”“文档整理”这类稳定角色

## Instructions 要求

- 项目级规则放 copilot-instructions.md
- 文件级规则放 .github/instructions
- applyTo 不要滥用 `**`，优先使用明确的匹配范围
