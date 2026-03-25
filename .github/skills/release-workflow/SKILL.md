---
name: release-workflow
description: "Use when: preparing a release, validating release readiness, generating release notes, assessing rollout risks, or planning rollback steps in this repository."
---

# Release Workflow

这个 Skill 用于把发布前后的关键工作串成一个完整流程，适合以下场景：

- 版本发布前检查
- 高风险改动上线准备
- 生成发布说明
- 制定回滚方案

## 使用时机

Use when:

- 需要确认是否具备发布条件
- 需要生成发布说明和回滚计划
- 需要对高风险变更做上线前检查

## 工作流

### 第一步：确认发布范围

先明确：

- 本次发布包含哪些改动
- 影响哪些模块
- 哪些验证已经完成
- 哪些高风险项仍未确认

### 第二步：发布准备

至少检查：

- 测试和构建结果
- 已知风险
- 兼容性影响
- 需要同步的依赖方

### 第三步：生成交付物

至少补齐：

- 发布说明
- 风险清单
- 回滚方案
- 发布后验证项

### 第四步：发布后复盘

如果有异常或高风险点，整理：

- 实际问题
- 根因分析
- 改进项

## 推荐搭配

这个 Skill 可以搭配以下资产使用：

- `release-notes.prompt.md`
- `rollback-plan.prompt.md`
- `retrospective.prompt.md`
- `release-checker.agent.md`

## 注意事项

- 不要只写发布说明，必须同时考虑回滚和验证
- 对高风险改动，优先先做发布检查再决定是否上线
