---
title: Topics 目录说明
type: meta
domain: meta
created: 2026-04-23
updated: 2026-04-23
---

# Topics 目录

**主题合成页**：跨多份来源的横向叙事与论点沉淀。

与其他页面的区别：
- **entity** = 一家公司（TSMC）；**topic** = 一个主题叙事（2026 年先进封装扩张）
- **concept** = 静态解释（什么是 CoWoS）；**topic** = 演化中的论点（2026 CoWoS 产能/定价/份额走势）
- **note** = 单来源摘要；**topic** = 多来源合成

详细模板与流程见 [../SCHEMA.md](../SCHEMA.md)。

---

## Phase 3 候选清单（待 Sonnet 回填）

基于 56 份现有 notes 抽取的高频主题，按优先级排序：

### 半导体 / 硬件

- [ ] **advanced-packaging** — CoWoS / SoIC / 先进封装（TSMC、All Ring、GPTC、ASE 等，≥8 份来源）
- [ ] **ai-optical-networking** — AI 驱动光通信升级（800G、CPO、OCS、SiPh；Innolight、TFC、YOFC、VPEC 等，≥5 份来源）
- [ ] **memory-supercycle-2026** — DRAM / HBM / NAND / NOR 上升周期（Sandisk、Macronix、SK Hynix、Samsung；≥5 份来源）
- [ ] **pcb-ccl-ai-upgrade** — PCB/CCL 材料升级与涨价（WUS、Delton、Shengyi、EMC、TUC、GCE、ZDT；≥3 份来源）
- [ ] **ai-thermal-cooling** — AI 液冷 TAM 扩张（AVC、Fositek、Jentech；≥3 份来源）
- [ ] **semis-testing-upcycle** — 半导体测试结构性上升（Hon Precision、MPI、WinWay；≥2 份来源）

### AI 算力与基础设施

- [ ] **agentic-ai-infra** — Agentic AI 对 CPU/DRAM/ABF 的需求拉动（MS 全球专题 + GC 系列，≥4 份来源）
- [ ] **ai-capex-2026** — 云厂商 Capex 与 AI 基础设施投入（含表外承诺，≥3 份来源）
- [ ] **nvda-gpu-vs-asic** — NVDA GPU 架构 vs 自研 ASIC 叙事（≥2 份来源）

### 软件 / 应用

- [ ] **ai-native-software** — 软件护城河重塑、AI 原生 SaaS（GS Moats IV、Bernstein、MS 开发重塑；≥3 份来源）
- [ ] **ai-observability** — AI 时代可观测性平台（DT、ESTC、Datadog；≥1 份来源）

### 自动驾驶 / 汽车

- [ ] **av-robotaxi-sdv** — Robotaxi / SDV / E2E（Waymo、WeRide、PonyAI、丰田；≥3 份来源）

### 中国互联网 / 电商

- [ ] **china-internet-ai-2026** — 中国互联网 AI 模型竞争、电商、即时零售（≥4 份来源）
- [ ] **china-industrial-ai-embodied** — AI 基础设施 + 具身 AI 哑铃策略（≥1 份来源）

### 宏观 / 跨主题

- [ ] **ai-labor-productivity** — AI 对劳动生产率/就业结构的影响（≥1 份来源）

---

## Phase 3 执行规则

回填时 Sonnet 需要：

1. 读 `topics/README.md`（本文件）选一个候选
2. 用 `grep` 或扫 `index.md`，列出所有涉及该主题的 notes
3. 按 SCHEMA.md 的 **Topic 模板** 生成合成页
4. 回写每一个被引用 note 的 frontmatter（追加 `topics:` 字段）
5. 若合成过程识别到新的重要 entity → 同步建 entity 页
6. 更新 `index.md` 的 Topics 区块
7. 追加 `log.md`：`## [YYYY-MM-DD] topic-synthesis | <topic slug>`

验收：topic 页至少整合 **≥3 份来源**，有 Thesis、关键数据、各家观点矩阵、受益/受损矩阵、Sources 回链。
