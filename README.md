# debate-defense-coach —— 论辩攻防助手

> **识别诡辩 → 破解陷阱 → 选择反驳武器。** 一部从《诡辩与反驳》（陈翼浦著）蒸馏出的随身方法论技能，装进任意 AI 应用就能用。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.1.1-blue)]()
[![Capabilities](https://img.shields.io/badge/capabilities-35-green)]()
[![Distilled](https://img.shields.io/badge/distilled-cangjie%20v2.5-orange)]()

## 📌 这是什么

**论辩攻防助手**是一套完整的逻辑攻防方法论技能包：上篇教你**识别** 27 种诡辩手法（偷换概念、复杂问语、以偏概全、人身攻击、道德绑架……），下篇教你**使用** 15 种反驳武器（以矛攻盾、二难法、归谬、实证、真相反驳……）。

它服务的场景只有一个：**别人跟你胡搅蛮缠的时候，你能一眼看穿套路，并说出可直接出口的反击话术。**

与一般"逻辑学教科书"不同：它不是让你读书，而是让 AI 掌握这本书的方法论——你只需提问，它按"识别 → 拆解 → 给话术 → 对照案例"四步回答，还能陪你实战演练（AI 出招你接招，按 5 维评分判卷复盘）。

## ✨ 功能亮点

- 🎯 **27 种诡辩手法全识别**——双特征检验（目的+手段），区分"无意谬误"与"有意诡辩"
- ⚔️ **15 种反驳武器全库**——每张能力卡含原文原理、触发条件、操作步骤、边界纪律
- 🥊 **陪练模式**——AI 扮演诡辩对手出招，你实战接招，按 5 维评分卡判卷复盘，从入门练到大师
- 🧰 **35 张六段式能力卡**——R/I/A1/A2/E/B 结构：原文说/I 理解/书内案例/触发边界/步骤/反例
- 📖 **25 条术语词典 + 速查表**——作者用法与常识的差异一目了然（如"转移法 vs 转移论题"）
- 🚫 **边界纪律内置**——识别到"不讲逻辑+权力碾压"型对手时，止损优先不恋战

## 🚀 快速开始

**前置**：任意支持 AgentSkills 规范（agentskills.io）的 AI 应用。本技能为标准 SKILL.md 格式，**一次编写、到处运行**——以下平台全部可直接安装使用：

| 应用 | 技能目录 | 发现机制 |
|------|---------|---------|
| Claude Code | `~/.claude/skills/` | 启动自动扫描 |
| OpenClaw | `~/.openclaw/skills/` 或项目内 `.openclaw/skills/` | 启动自动扫描 |
| OpenAI Codex CLI | `~/.codex/skills/` | 启动自动扫描 |
| ChatGPT | `/home/oai/skills/` | 自动发现 |
| GitHub Copilot / VS Code | `.agents/skills/`（项目级）| 自动发现 |
| WorkBuddy | `~/.workbuddy/skills/`（Windows: `C:\Users\<你>\.workbuddy\skills\`）| 启动自动扫描 |
| Cursor | `.cursor/skills/`（项目级）| 规则形式 |
| Gemini CLI / Amp / Goose / Manus 等 | 各平台对应 skills 目录 | 兼容标准格式 |

```bash
# 以 WorkBuddy 为例（其他平台同理，换路径即可）：
# 1. 把整个 debate-defense-coach/ 目录复制进技能目录
# 2. 完全重启应用（技能列表在启动时扫描）
# 3. 提问即用，无需任何配置
```

> 技能描述为"触发词驱动式"（含中英文触发词），各平台的自动发现机制都能准确命中。

## 💬 使用示例（五场景实战）

### 示例一 · 识别诡辩（职场）

> 你：同事说"领导都同意了你还反对？"——这话算不算诡辩？
>
> AI：算。手法=滥用权威（借领导压人）+ 以情代证（用服从文化替代论证）。
> 破解话术：「咱们讨论的是方案本身，不是谁点头了。请拿出方案依据，我们再谈。」

### 示例二 · 男女关系（概念守卫）

> 你：女朋友说"你爱我就要无条件包容我，我弟找工作你也得包了"。
>
> AI：手法=偷换概念（把"爱情里的爱护"换成"无条件顺从的义务"）+ 责任转移（弟弟的事变成你的义务）。
> 破解话术：「爱你是真的，'无条件满足所有要求'是另一回事。帮你弟我分两种帮：引荐、陪他准备面试，我随时在；"包工作"不承诺——我挣的钱，属于咱们这个小家庭。我家的责任田和你家的责任田，可以互相借种子，但不能要求我把收成全搬过去。」

### 示例三 · 家庭催婚（为你好拆解）

> 你：我妈说"妈都是为你好！再过两年你就嫁不出去了，老了一个人死在家里都没人发现！"
>
> AI：手法=以情代证（"为你好"阻断论证）+ 年龄恐吓（用恐惧替代理由）+ 以偏概全。
> 破解话术：「妈，您的好意我收到了——但"嫁不出去"和"孤独终老"是恐吓，不是事实。我身边四十多岁结婚过得很好的不是一两个。您担心我，我领情；吓唬我，我不吃。要不我把我的规划跟您讲讲？」

### 示例四 · 亲戚借钱（摆账分层）

> 你：堂哥说"你哥我真难，老婆病着侄子要交学费，就差三万周转一下，都是自家兄弟！"
>
> AI：手法=以情代证（凄惨叙事）+ 认亲绑架（亲情替代论证）。
> 破解话术：「哥，家里有难处我听得进。先摆账：缺口具体多少？用途哪几项？您现在的收支情况？账摆开，我看能帮什么。三万我没有，我能承担的是五千以内、救急、不用还；超过这个数得和我对象商量——这是两个人的钱，不是我一个人的面子。」

### 示例五 · 网络互骂（举证责任）

> 你：网友骂我"你就是收钱带节奏的水军！截图都在这，大家看！"
>
> AI：手法=诬蔑动机（攻击动机替代论证）+ 断章取义（截图无上下文）。
> 破解话术：「"收钱"的证据发我——没有证据，这话已经踩到诽谤的线了，造谣的举证责任在指控方。截图欢迎，请带上下文：原帖全文链接在这，谁断章取义大家自己看。要谈事实我在这，要打骂战我不奉陪——本层内容我已截图存档。」

> 每个示例都可以继续追问："还有其他手法吗？""如果是反过来他这么怼我怎么办？""来练练这个场景"——技能会按需加载对应能力卡。

## 🎮 陪练模式

说"**来练练 / 陪练 / 考考我**"即可开练：

- **场景自选**：职场 / 网络 / 家庭 / 谈判 / 亲密关系（20 情境）
- **难度阶梯**：入门（亮手法名）→ 进阶（隐藏手法）→ 大师（理中客设套）→ 大师加码（连环换招）
- **对手人格**：喷子型 / 数据包装型 / 情感投资型 / 理中客型 / 让步绑架型
- **判卷复盘**：识别精度 / 破解正确 / 武器选择 / 边界纪律 / 表达力 五维 ×20 分，附升级建议

## 📦 包内结构（48 文件 · 与本仓库一一对应）

```text
debate-defense-coach/
├── SKILL.md                        ← 技能入口：触发词/路由表/核心原则/边界
├── README.md                       ← 本文件（使用说明）
├── LICENSE                         ← MIT 协议
└── references/                     ← 45 个能力与知识文件
    ├── capability-index.md         ← 意图 → 能力卡 路由总索引
    ├── cheatsheet.md               ← 决策规则速查表
    ├── glossary.md                 ← 25 条术语词典（含与常识差异）
    ├── overview.md                 ← 整书理解（结构/术语底稿/批判）
    ├── DIGEST.md                   ← 精华长文（27 诡辩 + 15 反驳全景）
    ├── capabilities/               ← 35 张能力卡（识别 17 + 反驳 15 + 入口/陪练 3）
    │   ├─ 识别类 17（防）：
    │   │   sophistry-detection           诡辩识别双特征
    │   │   complex-question-defense      复杂问语破解
    │   │   argument-vs-reasoning         论证/推理二分
    │   │   fact-adjudicates-language     以实辨言
    │   │   context-guard                 语境限定核查
    │   │   concept-identity              概念同一性守卫
    │   │   thesis-identity               论题同一性守卫
    │   │   contradiction-scan            矛盾扫描
    │   │   excluded-middle               排中律检验
    │   │   evidence-truth                论据真实性审查
    │   │   evidence-relevance            论据相关性审查
    │   │   evidence-sufficiency          论据充分性审查
    │   │   evidence-triple-check         论据质量三问总则
    │   │   authority-relativity          权威相对性检查
    │   │   emotion-logic-separation      情理分离检验
    │   │   analogy-metaphor-check        类推/比喻有效性检查
    │   │   ad-hominem-immunity           人身攻击免疫
    │   ├─ 反驳类 15（攻）：
    │   │   contradiction-exposure        以矛攻盾（揭露自相矛盾）
    │   │   dilemma-construction          二难法
    │   │   reductio-absurdum             归谬法
    │   │   distinction-method            区别法
    │   │   transference                  转移法（借题而发）
    │   │   words-as-weapon               言辞为术
    │   │   dissection                    剖析法
    │   │   comparison                    比较法
    │   │   analogy-rebuttal              类推反驳
    │   │   metaphor-rebuttal             喻法反驳
    │   │   factual-rebuttal              实证法
    │   │   behavioral-rebuttal           行为反驳
    │   │   truth-rebuttal                真相反驳
    │   │   anti-authority-worship        驳迷信权威
    │   │   return-folly                  以谬治谬
    │   ├─ 入口/陪练/自查 3：
    │   │   gui-bian-yu-fan-bo-debate-coach  入口路由卡
    │   │   sparring-mode                  陪练模式总则
    │   │   self-defense-checklist         发言前防御自查清单
    └── sparring/                     ← 陪练模块（5 件套）
        ├── scenarios.md            ←   20 情境场景库（职场/网络/家庭/谈判/法庭）
        ├── scripts.md              ←   27 手法 × 81 句对手话术库
        ├── scripts-network.md      ←   全网话术增量 25 句
        ├── rubric.md               ←   5 维评分卡 + 复盘模板
        └── templates.md            ←   75 条可直接出口的金句模板
```

## 🌐 跨平台兼容

本技能遵循 **AgentSkills 开放标准**（Anthropic 发起，agentskills.io，OpenClaw / Codex / Copilot 等 20+ 应用采用）：

- frontmatter 使用标准字段 `name` + `description`（description 为触发词驱动式，适配各平台自动发现）
- 指令正文为纯 Markdown，引用均为相对路径（`references/...`），无平台专属语法
- 平台扩展字段（display_name / aliases / metadata 等）为可选增强，其他平台自动忽略，不影响加载

## ⚖️ 使用边界

- 技能只做**逻辑分析**，不替代法律 / 心理 / 医学专业意见
- 反方话术（scripts 中的对手视角）仅为演练靶材，不构成现实攻击建议
- 对"不讲逻辑 + 权力碾压"型对手：止损优先，不恋战
- 本项目为方法论蒸馏产物，书中案例与人物均为公开出版物内容

## 🤝 贡献

欢迎一切对本技能有价值的贡献：

- **报告问题**：提 Issue，说明触发场景与你期望的输出
- **新增金句/话术**：按 `references/sparring/templates.md` 格式追加，注明适用对手类型
- **新增场景**：按 `scenarios.md` 的 5 场景结构扩展情境库
- **提交方式**：Fork → 修改 → Pull Request，commit message 说明改动内容

## 📄 协议与致谢

- **协议**：[MIT License](LICENSE) —— 可自由使用 / 修改 / 商用 / 再分发，需保留版权声明
- **原著**：《诡辩与反驳》陈翼浦 著
- **蒸馏流水线**：cangjie-skill v2.5.0（RIA-TV++ 五阶段：整书理解 → 并行提取 → 三重验证 → 能力卡 → 压力测试）

*Generated by cangjie distillation pipeline · 2026-09-25*
