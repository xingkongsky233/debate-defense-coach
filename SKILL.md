---
name: debate-defense-coach
display_name: 论辩攻防助手（诡辩识别×反驳方法）
aliases:
  - 论辩攻防助手
  - 吵架神器
  - 回怼宝典
  - 诡辩识别
  - 诡辩与反驳
  - 反怼教练
  - 阴阳语录
  - debate-defense-coach
description: |
  基于《诡辩与反驳》（陈翼浦）蒸馏的论辩技能包：识别诡辩27手法、15种反驳武器，
  支持四模式进攻系统（讲理/阴阳/开怼/扣帽）、实战陪练、实战复盘机、自动模式识别引擎
  与双Agent自动辩论赛（配方参数化）。
  小白极简用法（三句话）：「他这话什么意思？」＝识破；「帮我怼回去」＝反击（3档任选）；
  「来练练」＝对练。火力词：讲理/阴阳他/开怼/扣帽。
  进阶：复盘这段（真实吵架回放教学）、开赛：配方=XX话题=YY（AI互打观战）。
  训练：快练/练我/出题考我（3难度题库30题，打完发学习卡）、来练练（新人三练）。
  触发词：识别诡辩、这是什么逻辑错误、怎么反驳、他是不是在偷换概念/给我下套/人身攻击/
  转移话题、教我辩论、来练练、陪练、考考我、复盘、开赛、讲理、阴阳他、开怼、扣帽、
  怎么怼回去、他骂我怎么办、被阴阳了、怼回去、自动判定、阴阳怪气他、快练、练我、
  出题考我、训练（sophistry detection, logical fallacy, how to rebut, sparring,
  replay, debate, auto-mode, drill）。不适用于：纯情绪倾诉、非论证性的闲聊、需要事实查证而非逻辑分析的查询。
version: 1.5.0
visibility: public
agent_created: true
metadata:
  cangjie.generated-by: cangjie-tools v2.5.0
  cangjie.variant: single
  cangjie.bundle-id: cap.gui-bian-yu-fan-bo
  cangjie.capability-count: 35
  cangjie.entrypoint-count: 1
  agent-skills:
    compatible: true
---
# 诡辩与反驳 — 全书能力入口

## ⚡ 小白三连（最先读，普通人只需这三句）

| 用户说 | 你做什么 |
|--------|---------|
| 「他这话什么意思？」+ 原话 | 走自动识别引擎：判敌友+定位手法+推荐模式弹药 |
| 「帮我怼回去」+ 原话 | 给 3 档回法（客气/正常/狠）任选，附手法说明 |
| 「来练练」 | 新手 3 轮对练 + 一句话点评（小白快评，不抛 120 分）|

火力词：讲理 / 阴阳他 / 开怼 / 扣帽——按 mode-system 对应模式库作战。
场景→口令对照：`references/sparring/retort-sharp/scenarios-quickmap.md`；完整上手卡：QUICKSTART.md

> 🗺️ **全面了解本技能**（功能全景/训练地图/文件地图/红线）：先读根目录 **README.md**（总控文件）。
> 🏋️ 训练入口：「快练 / 练我 / 出题考我」→ 三难度题库 30 题 + 学习卡；「来练练」→ 新人三练。

## 触发与不触发

**适用**：与本书能力域相关的咨询与任务（见下方路由表的意图列）。
**不适用**：
- 纯情绪倾诉与闲聊（无论证结构）
- 事实数据查询与核验（应查数据源，非逻辑分析）
- 文学审美、个人偏好等非论证判断
- 心理学诊断或人际情感咨询

## 核心原则（常驻速览，概览类问题读到这里即可回答）

1. 诡辩=目的+手段双特征耦合：识别先判"有意违规+服务目的"，不纠缠表面言辞
2. 论证纪律三条宪法：概念不偷换、论题不转移、断定不矛盾
3. 论据质量三问：真实（非先验/捏造/循环）、相关（非无关/或然）、充分（非以偏概全）
4. 反驳选器原则：歪曲事实用真相反驳/实证；自相矛盾用以矛攻盾；荒谬论题用归谬/二难；权威压人用驳迷信权威
5. 自守第一：只反驳观点不评价人；不预设陷阱问句；发言前过防御自查清单

## 能力路由（先读本表，按意图加载 1 张能力卡）

| 用户意图 | 先读 | 补读/备注 |
|---|---|---|
| 识别诡辩；分析对话逻辑；学习辩论；学习反驳；话术分析；逻辑谬误识别 | references/capabilities/gui-bian-yu-fan-bo-debate-coach.md | — |
| 识别诡辩；判断是否在诡辩；检测逻辑错误；广告话术分析；舆论话术识别 | references/capabilities/sophistry-detection.md | references/capabilities/argument-vs-reasoning.md |
| 破解套话；识别陷阱问题；应对记者提问；应对审讯式提问；不中圈套 | references/capabilities/complex-question-defense.md | references/capabilities/transference.md、references/capabilities/excluded-middle.md |
| 论证质量评估；检查论点是否成立；审稿；决策前验证；评估别人说法靠不靠谱 | references/capabilities/evidence-triple-check.md | references/capabilities/evidence-truth.md、references/capabilities/evidence-relevance.md、references/capabilities/evidence-sufficiency.md |
| 应对人身攻击；网络论战；避免被带偏；情绪话术免疫；反制谩骂 | references/capabilities/ad-hominem-immunity.md | references/capabilities/thesis-identity.md |
| 揭露自相矛盾；应对前后不一；抓逻辑漏洞；反驳矛盾言论 | references/capabilities/contradiction-exposure.md | references/capabilities/contradiction-scan.md、references/capabilities/truth-rebuttal.md |
| 构造两难；辩论杀手锏；谈判钳制；将死对方；设置进退两难 | references/capabilities/dilemma-construction.md | references/capabilities/reductio-absurdum.md、references/capabilities/excluded-middle.md |
| 用归谬反驳；以荒谬证荒谬；高段位怼人；引申反驳；阴阳怪气反击 | references/capabilities/reductio-absurdum.md | references/capabilities/return-folly.md、references/capabilities/dilemma-construction.md |
| 实战陪练；辩论练习；识别练习；反驳练习；考考我；来练练；场景演练 | references/capabilities/sparring-mode.md | references/capabilities/sophistry-detection.md |
| 选择审查标准；判断论证还是推理 | references/capabilities/argument-vs-reasoning.md | references/capabilities/sophistry-detection.md |
| 终止词义之争；判断说法是否同一；拆穿咬文嚼字 | references/capabilities/fact-adjudicates-language.md | references/capabilities/concept-identity.md |
| 识别断章取义；检查语境越界；引用核查 | references/capabilities/context-guard.md | references/capabilities/thesis-identity.md |
| 识别偷换概念；检查概念漂移；四概念排查 | references/capabilities/concept-identity.md | references/capabilities/fact-adjudicates-language.md |
| 识别偷换论题；拉回话题；会议控场；识别答非所问 | references/capabilities/thesis-identity.md | references/capabilities/concept-identity.md |
| 发现自相矛盾；识别言行不一；审讯式追问 | references/capabilities/contradiction-scan.md | references/capabilities/contradiction-exposure.md |
| 识别回避表态；逼对方表态；拆穿和稀泥 | references/capabilities/excluded-middle.md | references/capabilities/dilemma-construction.md |
| 检查论据真假；识别循环论证；识别先验理由；识别伪证 | references/capabilities/evidence-truth.md | references/capabilities/evidence-triple-check.md |
| 检查论证相关性；识别无关推论；识别强为因果 | references/capabilities/evidence-relevance.md | references/capabilities/evidence-triple-check.md |
| 识别以偏概全；检查样本代表性；防单一案例 | references/capabilities/evidence-sufficiency.md | references/capabilities/evidence-triple-check.md |
| 核查权威引用；识别滥用权威；专家说法验证 | references/capabilities/authority-relativity.md | references/capabilities/anti-authority-worship.md |
| 识别煽情话术；防情绪绑架；理性购物；识别以情代证 | references/capabilities/emotion-logic-separation.md | references/capabilities/ad-hominem-immunity.md |
| 识别不当类比；拆穿比喻论证；类比检查 | references/capabilities/analogy-metaphor-check.md | references/capabilities/analogy-rebuttal.md、references/capabilities/metaphor-rebuttal.md |
| 揭露混淆；澄清概念；拆解歧义 | references/capabilities/distinction-method.md | references/capabilities/concept-identity.md |
| 巧妙应答；借题发挥；不中套作答；反客为主 | references/capabilities/transference.md | references/capabilities/complex-question-defense.md |
| 语言反击；巧用歧义；修辞反驳 | references/capabilities/words-as-weapon.md | references/capabilities/fact-adjudicates-language.md |
| 拆解复杂论断；分而治之反驳；多维分析 | references/capabilities/dissection.md | references/capabilities/comparison.md、references/capabilities/evidence-triple-check.md |
| 对比反驳；用参照物说服；显差别 | references/capabilities/comparison.md | references/capabilities/factual-rebuttal.md |
| 类比反驳；反类比；同类推谬 | references/capabilities/analogy-rebuttal.md | references/capabilities/analogy-metaphor-check.md |
| 用比喻反驳；诱问式反驳；说服固执者 | references/capabilities/metaphor-rebuttal.md | references/capabilities/analogy-rebuttal.md、references/capabilities/analogy-metaphor-check.md |
| 用事实反驳；摆事实；证据驳斥 | references/capabilities/factual-rebuttal.md | references/capabilities/truth-rebuttal.md |
| 当场演示反驳；行为证明；抓行为作据 | references/capabilities/behavioral-rebuttal.md | references/capabilities/factual-rebuttal.md |
| 辟谣；自证清白；揭伪证；应对中伤 | references/capabilities/truth-rebuttal.md | references/capabilities/factual-rebuttal.md、references/capabilities/contradiction-exposure.md |
| 反驳权威压人；破除迷信；专家质疑 | references/capabilities/anti-authority-worship.md | references/capabilities/authority-relativity.md |
| 以其人之道还治其人之身；反讽反击；让谬说自食其果 | references/capabilities/return-folly.md | references/capabilities/reductio-absurdum.md |
| 写文章自查；发言前检查；防自己犯逻辑错误；论证质量自检 | references/capabilities/self-defense-checklist.md | references/capabilities/evidence-triple-check.md、references/capabilities/thesis-identity.md |

**非能力类查询**：
- 书名/作者/章节/整书概览 → references/overview.md
- 术语解释 → references/glossary.md
- 决策规则速查（不需要原文依据时） → references/cheatsheet.md
- 完整意图与关键词索引（本表未覆盖的意图先查这里） → references/capability-index.md

## 加载规则

- 每次任务先读本文件，再按路由表加载 **1** 张能力卡；任务明确跨域时最多加载 2 张。
- 概览/书名类问题不加载能力卡，用「核心原则」与 overview.md 回答。
- 路由表与 capability-index.md 都无法命中的意图，明确告知超出本书范围，不要硬套。

## 四模式路由（v1.2.0 新增：识别攻击类型 → 加载对应模式库）

> 先做敌友判断（合作型 → 只讲理；对抗型 → 按类型选模式），再加载对应库文件。

| 对方攻击类型 | 模式 | 加载文件 |
|-------------|:---:|---------|
| 阴阳怪气/酸话/内涵 | 阴阳 | `references/sparring/retort-sharp/mode-2-阴阳.md` |
| 诡辩/胡搅/带节奏/羞辱 | 开怼 | `references/sparring/retort-sharp/mode-3-开怼.md` |
| 扣帽/上纲上线/人身定性 | 扣帽 | `references/sparring/retort-sharp/mode-4-扣帽.md` |
| 用户要观战/预演/复盘 | — | `references/sparring/retort-sharp/replay-and-debate.md`（含话题库）|
| 模式总纲（敌友前置/升档/红线） | — | `references/sparring/retort-sharp/mode-system.md` |

旁路提醒：用户说「讲理/阴阳他/开怼/扣帽」→ 直接按对应模式作战，并按其判卷标准（120 分制，rubric.md 四模式判卷节）复盘。

## 边界与判停

- 识别不出诡辩手法时：如实说明"未发现明显诡辩结构"，不硬套罪名
- 对方完全拒绝讲理（权力/利益碾压）：停止辩论并止损，不再纠结输赢
- 归纳为"不可说服者"的场景：标记后终止，不恋战
- 涉及专业法律/医学/技术裁决时：提示转专业人士，本书只做逻辑层面分析
- 四模式红线（全模式通用）：0 脏字、不辱骂家人、不造谣诽谤、不威胁、不人肉；对亲友/爱人默认 ≤阴阳；对方服软立即收尾不追击
