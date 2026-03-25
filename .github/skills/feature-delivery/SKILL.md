---
name: feature-delivery
description: "Use when: delivering a medium or large feature end-to-end in this repository, especially when you need requirement analysis, task breakdown, implementation planning, validation, and delivery notes."
---

# Feature Delivery

这个 Skill 用于把中大型功能交付流程串成一个完整工作流，适合以下场景：

- 新功能落地
- 跨模块改动
- 重构后重新交付
- 需要同时输出计划、验证结果和交付说明的任务

## 使用时机

Use when:

- 需要先分析需求，再拆任务，再实施
- 需要明确验证方式和交付物
- 需要把功能开发从临时聊天升级成稳定工作流

## 工作流

### 第一步：需求分析

先明确：

- 目标是什么
- 影响哪些模块
- 哪些信息已经明确
- 哪些信息仍然缺失

### 第二步：任务拆解

把任务拆成 3 到 7 个可验证步骤。

每一步至少说明：

- 目标
- 受影响区域
- 风险点
- 验证方式

### 第三步：执行策略

- 低风险任务可以直接执行
- 中高风险任务先给计划，再小步推进
- 不要一次性大范围改动后再统一验证

### 第四步：验证与交付

至少输出：

- 修改文件
- 运行过的验证
- 测试或构建结果
- 剩余风险
- 交付说明或 PR 描述

## 推荐搭配

这个 Skill 可以搭配以下资产使用：

- `feature-plan.prompt.md`
- `task-breakdown.prompt.md`
- `bugfix.prompt.md`
- `pr-description.prompt.md`
- `planner.agent.md`
- `reviewer.agent.md`

## 注意事项

- 不要在信息不完整时直接进入大规模实现
- 不要省略验证步骤
- 不要把所有任务都塞进一次对话里，优先分阶段推进
