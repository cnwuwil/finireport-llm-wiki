# LLM Wiki — Claude 操作指南

这是一个个人 LLM Wiki，遵循 [Karpathy LLM Wiki 模式](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)。

> **核心哲学**：wiki 是**持续复利的合成物**，不是笔记堆。每次 ingest 的重点不是"写新 note"，而是**把来源整合进已有的实体/主题/概念页**——更新数据、标注矛盾、补交叉引用。Note 只是源的摘要卡片；知识本身活在 entity / concept / topic 页上。
>
> 如果一次 ingest 只产出 1 个 note、没更新任何其他页面 —— **没做对，重做。**

## 工作规则

1. **始终先读 [SCHEMA.md](SCHEMA.md)** ——单一真实来源，含页面模板、摄入 checklist、Lint checklist
2. **始终先读 [index.md](index.md)** ——掌握已有实体/主题，避免重复创建
3. Ingest 必须走完 SCHEMA.md 的 **强制 checklist**（通常触达 5–15 个页面）
4. 页面内容用**中文**，文件名用**英文/拼音小写**
5. 不改动 `sources/` 目录（原始来源只读）

## 快速操作

| 用户说 | Claude 动作 |
|---|---|
| "ingest `<文件>`" | 走 SCHEMA.md 的 7 步 checklist |
| "问 `<问题>`" | 先读 index → 读 topic/entity 合成页 → 必要时下钻到 note |
| "lint wiki" | 按 SCHEMA.md Lint checklist 扫描并汇报 |
| "新建 topic / entity `<名>`" | 按 SCHEMA.md 模板创建 |

## 四种页面类型（速览）

- **entity**（公司/人/工具）—— 活的合成，随来源滚动更新
- **concept**（方法/技术）—— 相对静态的解释
- **topic**（主题/叙事）—— ★ 多源横向合成，最有价值
- **note**（单源摘要）—— 短、必须回链实体/主题

详细模板与字段见 [SCHEMA.md](SCHEMA.md)。

## 领域标签

- `quant` — 量化交易
- `ai` — AI / LLM
- `invest` — 投资研究
- `eng` — 技术工程
- `meta` — 跨领域

## Ingest 后的自检

收尾前问自己：
- [ ] 是否至少更新了 1 个已有 entity 页？
- [ ] 是否识别/更新了至少 1 个 topic 页？
- [ ] Note 的 frontmatter 是否填了 `entities:` 和 `topics:`？
- [ ] 被更新的 entity/topic 页底部 `## Sources` 是否追加了本次来源？
- [ ] `index.md` 和 `log.md` 是否已更新？

全部是，才算完成。
