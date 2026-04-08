[English](README.md)

# Gender Risk Shield 🛡️

**互联网高敏感人群模拟器** — 用最挑剔的视角扫描任何内容的性别风险。

认真用是风控工具，不认真用是乐子神器。

---

## 这是什么

一个给 AI Agent 用的 Skill（知识包），让 AI 化身互联网上最敏感的那群人，用她们的视角审视你的内容。

**核心思路：** 不是"理性分析这个内容有没有问题"，而是"如果这个内容被最挑剔的人看到，她们会怎么想"。

每个维度都以该群体中最极端敏感的用户视角来写，因为舆情永远是最敏感的那批人引爆的。

投入一段文案、一个事件、一个竞品动态，它会：

| 模式 | 功能 |
|------|------|
| **路径 A：风险分析** | 八维度扫描性别雷区，告诉你哪里会炸、谁会攻击、在哪个平台 |
| **路径 B：对冲话术** | 被攻击了，给你防守策略、话术方向和评论区脚本 |
| **路径 C：竞品攻击话术** | 找到竞品的性别弱点，给你进攻方向、伪装身份和部署方案 |

## 适用行业

游戏 · 美妆 · 汽车 · 餐饮 · 影视 · 服饰 · 科技 · 教育 · 个人IP · 体育电竞

不限于以上。任何需要面对公众的品牌/个人都能用。

## 八维度模型

每个维度 0-10 分，≥7 高危：

| 维度 | 扫描什么 |
|------|----------|
| 女权/爱女 | 物化女性、不爱女、厌女、擦边 |
| 男权 | 媚女、忽视男性用户、双标 |
| BL/腐向 | 卖腐嫌疑、CP争议、BL领地冲突 |
| BG/异性恋 | 异性恋CP被拆、被边缘化、被BL覆盖 |
| ML/代入向 | 角色→主角的情感体验被破坏、角色被"共享" |
| 乙女 | 女性代入体验是否完整、男角色是否"专一" |
| GL/百合 | 百合元素争议、GL领地冲突 |
| LGBT/跨性别 | 跨性别设计、非二元性别、政策风险 |

权重按行业自动调整。美妆品牌女权维度×1.5，FPS游戏男权维度×1.5。详见 [risk-dimensions.md](references/risk-dimensions.md)

## 快速开始

### 作为 OpenClaw Skill

```bash
openclaw skill install gender-risk-shield
```

AI 会自动识别并加载。描述你的场景，选择路径即可。

### 作为知识库直接参考

不用 AI Agent 也能用。直接阅读 `references/` 下的文件，当作舆情工具书：
- [risk-dimensions.md](references/risk-dimensions.md) — 八维度评分标准
- [defense-strategies.md](references/defense-strategies.md) — 15种防守策略池
- [offense-playbook.md](references/offense-playbook.md) — 竞品攻击方法论
- [attack-patterns.md](references/attack-patterns.md) — 攻击话术全库
- [case-library.md](references/case-library.md) — 跨行业案例库
- [otome-rules.md](references/otome-rules.md) — 国乙法：41条乙女圈不成文规则

## 使用示例

**风险分析（路径A）：**
> "我们准备发一个男角色的宣传PV，目标用户以女性为主，帮我扫一下性别风险。"

**对冲话术（路径B）：**
> "我们的产品被小红书攻击'不爱女'，目前热度在涨，帮我出对冲方案。"

**竞品攻击（路径C）：**
> "竞品刚出了一个动漫联名，周边只有男角色没有女角色，用户70%是女性，帮我找攻击点。"

## Eval 效果展示

真实场景测试，展示 skill 的实际输出：

| Eval | 场景 | 路径 | 输出 |
|------|------|------|------|
| eval-01 | 游戏PV性别风险扫描 | A（风险分析） | [output-01](evals/output-01-game-pv.md) |
| eval-02 | 美妆品牌男代言人舆情对冲 | B（对冲话术） | [output-02](evals/output-02-beauty-endorsement.md) |
| eval-03 | 茶饮竞品联名性别争议攻击 | C（竞品攻击） | [output-03](evals/output-03-competitor-attack.md) |

## 文件结构

```
gender-risk-shield/
├── SKILL.md                          # 主文件：使用流程和输出格式
├── README.md                         # 英文版 README
├── README_zh.md                      # 中文版 README（本文件）
├── LICENSE                           # MIT
├── CHANGELOG.md                      # 版本记录
├── CONTRIBUTING.md                   # 贡献指南
├── clawhub.json                      # ClawHub 包配置
├── references/
│   ├── risk-dimensions.md            # 八维度评估标准
│   ├── defense-strategies.md         # 15种防守策略池
│   ├── attack-patterns.md            # 攻击话术全库（按势力分类）
│   ├── offense-playbook.md           # 竞品攻击方法论
│   ├── case-library.md               # 跨行业案例库（含翻车案例）
│   ├── platform-rules.md            # 各平台性别议题特征
│   └── otome-rules.md               # 国乙法：乙女圈不成文规则（41条雷区）
└── evals/
    ├── files/                        # 测试用例输入
    ├── output-01-game-pv.md          # Eval 1: 游戏PV风险分析
    ├── output-02-beauty-endorsement.md  # Eval 2: 美妆品牌对冲话术
    └── output-03-competitor-attack.md   # Eval 3: 茶饮竞品攻击方案
```

## 注意事项

- 本工具提供的是**分析框架和话术方向**，不是可以直接发布的成品文案
- 所有输出在发布前需经过人工审核
- 使用者需自行判断合规性和道德边界
- 案例库中的事件均来自公开信息

## 贡献

欢迎提交新案例、新话术、新行业场景。详见 [CONTRIBUTING.md](CONTRIBUTING.md)

## License

[MIT](LICENSE)
