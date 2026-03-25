---
description: "生成 Pull Request 描述，适用于总结本次改动的背景、改动点、测试结果、风险和回滚说明。"
---

# PR 描述生成

请基于当前改动生成一份 PR 描述。

## 输入

- 背景：${input:background}
- 重点改动：${input:changes}
- 已完成验证：${input:validation}

## 输出结构

1. 背景
2. 改动内容
3. 测试与验证
4. 风险与兼容性影响
5. 回滚建议
