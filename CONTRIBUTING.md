# 贡献指南

欢迎提交 PR！以下是贡献方式。

## 可以贡献什么

### 案例
在 `references/case-library.md` 中添加新案例，格式：

```markdown
### 案例N：事件名称（年份）
- **事件：** 一句话概述
- **涉及维度：** 哪些维度
- **各方反应：** 各方怎么说
- **结果：** 最终怎样
- **教训：** 学到什么
```

要求：
- 事件来自公开信息
- 不包含真实个人隐私
- 教训要具体可执行，不要"注意舆情"这种废话

### 话术
在 `references/attack-patterns.md` 中添加新话术，格式：

| 话术 | 含义 | 触发场景 | 应对建议 |

### 行业场景
在 `references/risk-dimensions.md` 的各维度触发场景表中补充新行业。

### 防守/攻击策略
在 `references/defense-strategies.md` 或 `references/offense-playbook.md` 中补充新策略。

## 提交规范

- 一个 PR 只做一件事
- commit message 写清楚改了什么
- 涉及具体品牌的案例，确保信息来自公开渠道

## 不接受什么

- 包含内部/机密数据的内容
- 针对特定个人的攻击话术
- 无法验证来源的案例
