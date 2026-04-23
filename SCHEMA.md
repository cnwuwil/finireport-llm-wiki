# Wiki Schema

LLM Wiki 操作规范（单一真实来源）。LLM 负责所有维护，人类负责投喂来源与提问。

## 核心哲学

> **Wiki 是持续复利的合成物，不是笔记堆。**
>
> 每新增一份来源，**大多数工作不是写新 note，而是更新已有的实体/主题/概念页**——合成新观点、标注与旧数据的矛盾、补充交叉引用。Note 只是源的 1-to-1 摘要，**知识本身活在 entity / concept / topic 页上**。

如果下一次 ingest 只产出一个 note、没有任何其他页面被更新，那说明没做对。

---

## 领域标签

- **quant** — 量化交易（策略、回测、数据、执行）
- **ai** — 人工智能 / LLM（模型、技术、工具、论文）
- **invest** — 投资研究（宏观、行业、公司、资产）
- **eng** — 技术工程（编程、架构、系统设计）
- **meta** — 跨领域 / 元信息

---

## 目录结构

```
wiki/
├── SCHEMA.md       # 本文件：操作规范（单一真实来源）
├── CLAUDE.md       # 简化入口：工作流摘要，指向本文件
├── index.md        # 导航目录（按 Topic → Entity → Concept → Note 分组）
├── log.md          # 操作时间线（追加式）
├── sources/        # 原始来源（只读，人类放入）
│   └── quant-reports/
│       └── raw-pdf/    # 原始 PDF 归档
├── topics/         # ★ 主题/叙事合成页（N 份来源 → 1 页横向综述）
├── entities/       # 实体页（公司、人物、工具、机构…随来源滚动更新）
├── concepts/       # 概念页（方法、技术、思想、框架）
└── notes/          # 单来源摘要（精简，指向 entities/topics/source）
```

---

## 四种页面类型

### 对比表

| 类型 | 定位 | 一句话 | 何时创建 | 何时更新 |
|---|---|---|---|---|
| **entity** | 具体可命名对象 | TSMC、NVDA、Apple、Jim Simons、CUDA、Palantir | 一个实体在 ≥2 份来源中出现 | 每次有新来源提及该实体 |
| **concept** | 静态的思想/方法/技术 | CoWoS 封装、RLHF、均值回归、数据仓库分层 | 一个概念值得独立解释 | 新来源带来新细节/数据 |
| **topic** | 动态的主题叙事 / 演化中的论点 | Agentic AI 全景、2026 存储超级周期、AI 光通信升级 | ≥3 份来源共谈一个主题 | 每份新来源必回写 |
| **note** | 单来源摘要 | "JPM 2026-04-17 TSMC Leading Edge 报告摘要" | 每份来源各一份 | 极少更新（只在勘误时） |

### 判定原则

- **不要把主题写成 concept** — concept 相对静态（"什么是 CoWoS"），topic 是演化的（"2026 年 CoWoS 产能扩张与定价展望"）
- **不要为单实体做 topic 页** — TSMC 的合成属于 `entities/tsmc.md`；`topics/advanced-packaging.md` 则横跨 TSMC/ASE/All Ring/GPTC 多家
- **note 永远不做合成** — 合成一定落在 entity/concept/topic 页；note 只是"这份 PDF 说了什么 + 链到哪几个页"

---

## 页面模板

所有页面都用 YAML frontmatter。字段见下。

### 通用 frontmatter

```yaml
---
title: 页面中文标题
type: entity | concept | topic | note
domain: quant | ai | invest | eng | meta
tags: [tag1, tag2, ...]
created: YYYY-MM-DD
updated: YYYY-MM-DD
---
```

### Entity 模板（`entities/<name>.md`）

```markdown
---
title: 公司/对象名（含代码）
type: entity
domain: invest
tags: [代码, 中文名, 英文名, 所在行业, 关键主题]
aliases: [别名 1, 别名 2]
created: YYYY-MM-DD
updated: YYYY-MM-DD
---

# <实体名>

**代码 / 行业 / 市值 / 总部**（一行基本面）

## 一句话定位

（LLM 自己写的一句话画像，随认知更新）

## 业务结构

（分业务线的简介）

## 当前论点 / 合成视图

（把最近 N 份来源的共识与分歧合成，**这是 entity 页的核心**）

## 关键指标（合成）

| 指标 | 数值 | 来源 |
|---|---|---|

## 分析师覆盖一览

| 机构 | 日期 | 评级 | 目标价 | 关键观点 | 来源 |
|---|---|---|---|---|---|
| Goldman Sachs | 2026-04-16 | Buy | NT$2,750 | GM 66.2% 超预期… | [note](../notes/tsmc-1q26-earnings-review-gs-2026.md) |

## 矛盾 / 待解问题

- （例：4 家 broker 2027 Capex 预测区间 US$60B-70B，差异来源未明）

## Sources

按时间倒序，**每次 ingest 必须追加一行**：

- 2026-04-16 · GS · [TSMC 1Q26 Review](../notes/tsmc-1q26-earnings-review-gs-2026.md)
- 2026-04-16 · Nomura · [TSMC 1Q26 Guidance Raise](../notes/tsmc-1q26-guidance-raise-nomura-2026.md)

## Related

- [[topics/advanced-packaging]]
- [[topics/ai-capex-2026]]
```

### Concept 模板（`concepts/<name>.md`）

```markdown
---
title: 概念名
type: concept
domain: quant | ai | invest | eng
tags: [...]
created: YYYY-MM-DD
updated: YYYY-MM-DD
---

# <概念名>

## 定义

（一段简明定义）

## 原理 / 机制

## 应用场景

## 常见坑点 / 误区

## Sources

（引用该概念的来源，每次新来源提及时追加）

## Related

- [[相关概念]]
- [[相关实体]]
```

### Topic 模板（`topics/<slug>.md`）——★ 核心

```markdown
---
title: 主题标题
type: topic
domain: invest | ai | quant | eng
tags: [...]
status: active | settled | dormant
created: YYYY-MM-DD
updated: YYYY-MM-DD
---

# <主题>

## Thesis（当前论点）

（一段话概括，随来源演化——这是主题页最有价值的部分）

## 关键事实 / 数据点

- CPU TAM +$32.5–60bn（MS 2026-04-19）
- DRAM 需求增量 +15–45 EB（MS 2026-04-19）
- …

## 各家观点

| 机构 | 日期 | 观点 | 来源 |
|---|---|---|---|

## 受益 / 受损矩阵

| 公司 | 关系 | 来源 |
|---|---|---|
| [[Celestica]] | 受益：Google TPU + AMD Helios | [note](...) |

## 矛盾 / 待解问题

## Sources

（按时间倒序，每次 ingest 必须追加）

## Related

- [[topic 或 entity]]
```

### Note 模板（`notes/<slug>.md`）

**原则**：短、可扫读，只记关键数据点和 ★ 回链。合成观点写在 entity/topic 里而不是这里。

```markdown
---
title: 来源标题
type: note
domain: ...
tags: [...]
source: sources/quant-reports/xxx.md
broker: Goldman Sachs
date: YYYY-MM-DD
entities: [tsmc, nvda]          # ★ 必填：此 note 触及的 entity slug
topics: [advanced-packaging]     # ★ 必填：此 note 触及的 topic slug
rating: Buy
pt: NT$2,750
created: YYYY-MM-DD
updated: YYYY-MM-DD
---

# <来源标题>

**来源** · **机构** · **日期** · **评级 / 目标价**

## 核心结论

（3-5 个 bullet，原文的关键论点）

## 关键数据

（表格或 bullet，能让后续的 entity/topic 合成取用）

## 与既有观点的关系

- 强化 / 补充 / 矛盾于 [[entities/tsmc]] 中的 <某条>
- 关联 [[topics/advanced-packaging]]

## 原文

[sources/quant-reports/<filename>.md](...)
```

---

## 命名规范

- 文件名：**全小写**，英文或拼音，用 `-` 分隔
- 实体：公司用 ticker 或通用名（`tsmc.md`、`nvda.md`、`jentech.md`）
- 主题：描述性 slug（`agentic-ai-infra.md`、`advanced-packaging.md`、`memory-supercycle-2026.md`）
- Note：`<主语>-<事件>-<broker>-<year>.md`（`tsmc-1q26-earnings-review-gs-2026.md`）

---

## 交叉引用规范

**链式规则**：
- Note 链向 ≥1 个 entity/topic；绝不孤立存在
- Entity/Topic/Concept 页底部有 `## Sources` 回链到相应 notes
- 页间引用用 `[[slug]]` 或 `[显示名](path/file.md)`

**一致性要求**：
- 如果某个公司被 note A 引用但 `entities/<name>.md` 的 Sources 没出现 A → 是 lint 漏洞
- 反向亦然：entity Sources 列了 X，X 的 note frontmatter `entities:` 必须包含该实体

---

## 核心操作

### 1) Ingest（摄入新来源）— **强制 Checklist**

每份来源必须严格按顺序走完：

1. **读来源**：`sources/<path>/<file>.md`（PDF 先 MinerU 转 md，原始 PDF 归档到 `sources/quant-reports/raw-pdf/`）
2. **列实体**：扫描来源中所有具名公司/人/工具
   - 对每个：`entities/<slug>.md` 存在？
     - 存在 → 追加 `## Sources`、更新"分析师覆盖"表、更新"当前论点"段、标注矛盾
     - 不存在且出现 ≥2 次或为主要标的 → 新建 entity 页（按模板）
3. **识别主题**：来源属于哪些现有 topic？或开启新 topic？
   - 追加 topic 的 Sources、Thesis 段、受益矩阵
   - ≥3 份来源共同指向且还没页 → 新建 topic 页
4. **更新 concept**（若涉及新技术/方法）
5. **写 note**：按 note 模板，`entities` 和 `topics` frontmatter 必填，正文精简（<300 行）
6. **更新 `index.md`**：新建的 entity/topic/concept/note 条目
7. **追加 `log.md`**：`## [YYYY-MM-DD] ingest | <标题>`，列出所有被触达的页面

**验收标准**：一份来源的 ingest 通常会触达 **5–15 个页面**。如果只新建了 1 个 note、没更新任何现有页——重做。

### 2) Query（查询）

1. 读 `index.md` 定位相关 topic/entity
2. 优先读 **topic/entity 合成页**（已经是多源合成，省 token）
3. 需要细节时再下钻到 note → source
4. 若回答本身有长期价值（新的对比/分析/连接）→ 作为新 topic 或写入现有 entity 的合成段；不要留在对话里

### 3) Lint（健康检查）

按以下 checklist 扫描：

- [ ] **孤儿 note**：note frontmatter `entities:` 和 `topics:` 均为空 → 补回链或合并
- [ ] **缺失实体**：某名字在 ≥3 个 note 中出现但无 `entities/<name>.md` → 新建
- [ ] **缺失主题**：≥3 个 note 共享关键词/tag 但无对应 topic 页 → 新建
- [ ] **Sources 双向对齐**：entity/topic 页的 Sources vs note 的 frontmatter 应一致
- [ ] **过期**：entity/topic 页 `updated` 早于最近相关 note 的 `date` → 回填
- [ ] **矛盾未标注**：同实体不同 broker 目标价相差 >20% 但 entity 页未列 → 补 "矛盾 / 待解问题" 段
- [ ] **frontmatter 完整性**：`type` / `domain` / `created` / `updated` 齐备
- [ ] **命名一致**：文件名、slug、frontmatter title 对齐

---

## log.md 格式

```markdown
## [YYYY-MM-DD] ingest | <来源标题>
- 来源：<broker>，<报告日期>
- 新建 note: notes/<slug>.md
- 更新 entity: entities/tsmc.md（追加 Sources，更新分析师覆盖表）
- 更新 topic: topics/advanced-packaging.md（追加 thesis bullet）
- 更新 index.md（Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/
```

## index.md 结构（摘要）

```markdown
# Wiki Index

## Topics（主题合成页）
- [[agentic-ai-infra]] — …
- [[advanced-packaging]] — …

## Entities（实体库）
### 半导体 & 硬件
- [[tsmc]]、[[nvda]]、[[asml]]、…
### 软件 & 互联网
…

## Concepts（方法/技术）
- [[quant-data-infra]]、[[cowos-packaging]]、…

## Notes（按领域 / 时间倒序）
…

## Sources（原始来源索引）
（默认折叠 / 只列最近 30 条，完整列表见 sources/ 目录）
```
