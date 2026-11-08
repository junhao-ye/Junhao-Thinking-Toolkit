# Junhao-Thinking-Toolkit 使用手册

[繁體中文](user-guide.zh-TW.md) · **简体中文** · [English](user-guide.en.md) · [日本語](user-guide.ja.md)

[返回简体中文 README](../README.zh-CN.md)

## 安装与更新

1. 从仓库获取完整的 [`skills/junhao-thinking-toolkit`](../skills/junhao-thinking-toolkit) 文件夹，保留 `SKILL.md` 和同级的 `references/`。
2. 将整个文件夹复制到 Agent 的技能目录。以 Codex 为例，安装后应能在 `~/.codex/skills/junhao-thinking-toolkit/SKILL.md` 找到入口文件。在 Windows 中，`~` 代表你的用户主目录。
3. 打开新对话，从技能列表选择 `junhao-thinking-toolkit`，或在请求中点名。先用一小段笔记试试整理材料，确认回复包含分组和原文线索。
4. 更新时，先保留自己修改过的文件，再用新版的完整技能文件夹替换旧版，让入口文件和参考文件保持在同一版本。

## 提出第一个任务

说明你想推进什么、手头有哪些材料、限制是什么，以及希望得到什么结果。知道方法时可以点名，也可以让工具箱按目标选择。可以直接改写下面的模板。

```text
请使用 junhao-thinking-toolkit。
我想弄清 [问题]，以便 [要做的决定或行动]。
可用材料是 [笔记、数据或链接]。限制是 [时间、预算或底线]。
请交付 [表格、检查清单或逐步引导]，并用简体中文回答。
```

交互式方法每轮聚焦一个问题，回答后再进入下一步。材料已经齐备时，可以要求直接给出结果。如果要串联两种方法，先说清楚第一种方法的结果如何用于第二种。

## 方法索引

### 四个轻量入口

| 方法 | 何时使用 | 会收到什么 |
| --- | --- | --- |
| [整理材料](../skills/junhao-thinking-toolkit/references/organize-material.md) | 想整理笔记、聚焦重点或寻找重复模式 | 分组、原文依据和有待验证的线索 |
| [假设检验](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 想知道哪些前提决定方案能否成立 | 关键假设、反例、替代解释和验证条件 |
| [逐步引导](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 问题已明确，想自己参与求解 | 当前一步、完成标准和一个帮助继续求解的问题 |
| [行动规划](../skills/junhao-thinking-toolkit/references/make-decision.md) | 方向已定，需要安排执行 | 优先顺序、时间表、依赖关系、障碍和第一步 |

### 十二种核心方法

| 方法 | 何时使用 | 会收到什么 |
| --- | --- | --- |
| [苏格拉底式提问](../skills/junhao-thinking-toolkit/references/clarify-question.md) | 还没有说清真正的卡点 | 每轮一问，最后得到可以回答的问题 |
| [双层解释](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | 想先建立直觉，再理解准确的机制 | 直觉版与专业版解释、类比边界和理解检查 |
| [反向拆解](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | 想从现有成品学习做法 | 可迁移的规律、操作清单和最小练习 |
| [横纵分析](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | 想同时研究历史变化与同类对象 | 时间线、横向对比和未来路径 |
| [事实核查](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | 想验证可以查证的说法或数字 | 逐项核实结果、来源、日期和推理缺口 |
| [专家会诊](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 同一个问题需要互补的专业视角 | 各观点的理由、风险、关键分歧和综合判断 |
| [第一性原理](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 现有方案受到惯例约束 | 从基本事实和限制出发重建的选项与验证动作 |
| [跨领域借鉴](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 常用方法遇到瓶颈，想找相似机制 | 可迁移的机制、适用条件和试验 |
| [双向钢人论证／多选项比较](../skills/junhao-thinking-toolkit/references/make-decision.md) | 两个或更多选项难以取舍 | 两个方案各自最强的论据，或按相同标准比较多个方案 |
| [最小可逆实验](../skills/junhao-thinking-toolkit/references/make-decision.md) | 关键未知可以用短期、低成本行动验证 | 实验步骤、指标、继续或停止的阈值 |
| [天赋考古](../skills/junhao-thinking-toolkit/references/self-exploration.md) | 想从具体经历找出反复出现的优势 | 优势假设、经历证据和 30 天验证 |
| [人生设计](../skills/junhao-thinking-toolkit/references/self-exploration.md) | 想比较几条值得探索的未来方向 | 三个五年版本和本周可尝试的原型行动 |

## 可以直接使用的示例

### 从笔记中找模式

> 使用 junhao-thinking-toolkit 整理这 12 条客服笔记。按主题分组，重复转述的事件合并计算，为每个可能的模式附上笔记编号和例外。最后标出一条最值得查证的线索。

你会得到有原文依据的模式列表。只有少数案例时，回复应把它标为待验证线索。

### 先比较，再决定是否试验

> 使用 junhao-thinking-toolkit 比较两个客服流程。底线是回复质量，预算上限是每周 4 小时。先为两个方案分别提出最强的论据。如果取舍取决于某个可以观察的未知，再设计一个能在一周内回退的试验，写明指标和停止阈值。

先看比较结果。如果还有可能改变选择的未知，就用试验结果更新决策。

### 每轮自己完成一步

> 使用 junhao-thinking-toolkit，逐步引导我找出这份转化率计算中的错误。每轮只给当前一步、完成标准和一个问题。等我回答后再继续。

如果后来想直接看完整流程，可以请它整理已经完成的步骤，再列出剩余步骤和检查点。

## 解读结果与常见问题

- **技能没有出现在列表里。** 确认 Agent 支持 Agent Skills、当前运行环境能读取技能目录，并且 `SKILL.md` 和 `references/` 位于同一个技能文件夹。再打开新对话确认。
- **方法选错了，或者回复太长。** 说明你需要什么结果，或直接指定方法和篇幅，例如「只做假设检验，给我一张表」。对于纯摘要、翻译或简单查询，可以直接提出原任务。
- **回复中有待验证的内容。** 区分材料陈述、已核实事实、推断和价值取舍。需要查证时可要求一手来源和日期。证据不足时，把结论保留为待验证。
- **材料包含敏感信息或内嵌提示词。** 分享前先移除个人信息、凭证和其他不必要的敏感内容。在请求中写清楚如何处理附件，让其中的提示词作为引用材料来分析。
- **涉及医疗、法律、重大财务或心理健康。** 可以用工具箱梳理问题和准备资料，把专业判断交给有资质的专业人士。自我探索主要产出可验证的假设和行动。

想了解方法出处或维护方式，可查看[来源与对照](../skills/junhao-thinking-toolkit/SOURCES.md)和[技能规范](../skills/junhao-thinking-toolkit/SPEC.md)。
