---
title: Agentic AI 基础设施：算力架构重塑与全链条受益
type: topic
domain: invest
tags: [Agentic AI, CPU TAM, DRAM, ABF基板, Aspeed, BMC, AI Agent, 算力架构, 数据中心, 基础设施]
status: active
created: 2026-04-23
updated: 2026-04-24
---

# Agentic AI 基础设施：算力架构重塑与全链条受益

## Thesis（当前论点）

AI 从"生成式"到"自主行动（Agentic）"的转型，**不仅仅是软件层面的升级，更是硬件架构的重组**。GPU 仍是核心算力单元，但多步骤 Agent 工作流要求大量任务协调、工具调用和上下文管理，CPU 成为控制平面——**Jensen Huang 原话："The CPU is no longer simply supporting the model; it's driving it."**

结果：AI 资本支出从单一加速器 chip 扩散至整个服务器系统（CPU、DRAM、ABF 基板、BMC、MLCC、PCB），受益面远比"GPU 概念股"宽。

## 关键量化框架（Morgan Stanley 2026-04-19）

| 维度 | 当前 | 2030E 增量 | 来源 |
|---|---|---|---|
| CPU TAM 增量 | — | **$32.5–60B** | MS 全球专题 |
| 总数据中心 CPU TAM | — | **$82.5–110B+** | MS 全球专题 |
| DRAM 增量需求 | — | **15–45 EB**（占 2027 供应 26–77%） | MS 全球专题 |
| ABF 缺口（无 Agentic） | 7% | 7%（2030E） | MS 大中华 |
| ABF 缺口（含 Agentic） | 7% | **15%**（2030E） | MS 大中华 |
| ABF 市场 CAGR 2025-30E | — | 17.9%（含）vs 16.1%（不含） | MS 大中华 |
| Agentic 工作负载中 CPU 占比 | — | **50–90%** 工作时间 | MS 全球 |

## 各家观点

| 机构 | 日期 | 关键判断 | 来源 |
|---|---|---|---|
| MS（全球专题） | 2026-04-19 | CPU TAM +$32.5-60B；DRAM +15-45 EB；ABF 缺口扩至 15% | [MS AI Agent 全球](../notes/ai-agent-rise-global-infra-ms-2026.md) |
| MS（大中华硬件） | 2026-04-19 | ABF 缺口扩至 15%；Unimicron CPU 增 10-15M → 营收+2-3% | [GC 硬件 Agentic](../notes/agentic-ai-hardware-gc-ms-2026.md) |
| MS（云半导体） | 2026-04-19 | Aspeed BMC 是"CPU 服务器最大 Capex 效率受益者"；EPS 高于共识 20-23% | [云半导体非 GPU](../notes/cloud-semis-non-gpu-agentic-ai-ms-2026.md) |
| Citi AI 峰会 | 2026-04-17 | 算力约束至 2029 年；Physical AI 是最共识主题；网络安全受益 | [Citi AI 峰会](../notes/citi-ai-summit-tech-invest-outlook-2026.md) |

## 受益 / 受损矩阵

### 基础设施芯片

| 公司 | 定位 | 关键数据 | 来源 |
|---|---|---|---|
| Aspeed（5274.TWO） | CPU 服务器 BMC 市占率 **~70%**；AST2700 ASP +40-50% | PT NT$15,555，EPS 超共识 23%/20% | [云半导体](../notes/cloud-semis-non-gpu-agentic-ai-ms-2026.md) |
| Montage | 内存缓冲芯片，CPU 服务器每台 ~$100 | CPU 服务器增长直接受益 | [云半导体](../notes/cloud-semis-non-gpu-agentic-ai-ms-2026.md) |
| WPG / WT Micro | 半导体分销；WT Micro 为 TPU 主要分销商 | 网络交换机采购滞后 1-2Q → 2H26 受益 | [云半导体](../notes/cloud-semis-non-gpu-agentic-ai-ms-2026.md) |
| NVDA | CPU+GPU 控制平面（Grace Blackwell）| CPU 仍需要 GPU 赋能 | [MS AI Agent](../notes/ai-agent-rise-global-infra-ms-2026.md) |
| Intel / AMD / Arm | 传统服务器 CPU TAM 扩张受益 | TAM +$32.5-60B | [MS AI Agent](../notes/ai-agent-rise-global-infra-ms-2026.md) |

### 基板 / PCB / 被动元件

| 公司 | 定位 | 关键数据 | 来源 |
|---|---|---|---|
| Unimicron（3037） | ABF 基板主要供应商；CPU +10-15M → 营收 +2-3% | ABF 缺口 15% 推动定价上行 | [GC 硬件](../notes/agentic-ai-hardware-gc-ms-2026.md) |
| Lotes（3533） + FIT（6088） | CPU 插槽合计市占率 **70-80%** | Lotes 全年指引有上调空间 | [GC 硬件](../notes/agentic-ai-hardware-gc-ms-2026.md) |
| Yageo（2327） | MLCC/电阻/电感/钽电容全覆盖 | CPU TAM +10-15M → MLCC 市场价值 +2-3% | [GC 硬件](../notes/agentic-ai-hardware-gc-ms-2026.md) |
| SEMCO（三星电机） | MLCC 全球龙头；ABF 基板 | MLCC 上行周期 + ABF 受益 | [MS AI Agent](../notes/ai-agent-rise-global-infra-ms-2026.md) |
| Shengyi（600183） | CCL 基材；2H26 AI 平台换代机遇 | AI 规格升级至 6+N+6 HDI | [GC 硬件](../notes/agentic-ai-hardware-gc-ms-2026.md) |

### 软件 / 应用层（Citi 峰会视角）

| 公司 | 定位 | 来源 |
|---|---|---|
| GOOGL（Google Cloud） | 算力 + Agent 编排平台 | [Citi 峰会](../notes/citi-ai-summit-tech-invest-outlook-2026.md) |
| AMZN（AWS） | Trainium3 + Agent 平台 | [Citi 峰会](../notes/citi-ai-summit-tech-invest-outlook-2026.md) |
| PANW / CRWD | AI 驱动网络安全需求爆发（Mythos 级别攻击面扩大） | [Citi 峰会](../notes/citi-ai-summit-tech-invest-outlook-2026.md) |
| Equinix / Digital Realty | 企业推理工作负载 → 数据中心托管需求 | [Citi 峰会](../notes/citi-ai-summit-tech-invest-outlook-2026.md) |

## 矛盾 / 待解问题

- **CPU TAM 增量预测幅度很宽**（$32.5–60B）：取决于 Agentic 工作流中 CPU 侧处理的最终比例（50–90%区间），实际落地节奏有较大不确定性
- **ABF 定价谈判**：MS 认为 Unimicron 1Q26 利润率有下行惊喜风险（涨价由成本驱动非供不应求），与"缺口 15%"的供需判断存在内在张力
- **Citi 峰会的 Mythos 影响**：Anthropic 不公开发布，意味着商业化路径延迟；但 6–9 个月内开源模型会到同等级别——网络安全需求高度确定，但企业软件影响时间表不明
- **CoreWeave 3GW 签约 vs 实际部署**：电力合同签约 ≠ 机架部署，算力约束到 2029 年的预测是否准确待验证

## Sources

- 2026-04-19 · MS · [AI Agent 崛起：全球专题](../notes/ai-agent-rise-global-infra-ms-2026.md)
- 2026-04-19 · MS · [大中华硬件 Agentic AI 受益者](../notes/agentic-ai-hardware-gc-ms-2026.md)
- 2026-04-19 · MS · [云半导体非 GPU 需求](../notes/cloud-semis-non-gpu-agentic-ai-ms-2026.md)
- 2026-04-17 · Citi · [第四届 AI 峰会纪要](../notes/citi-ai-summit-tech-invest-outlook-2026.md)
- 2026-04-20 · Citi · [Dell & SMCI AI 基础设施需求加速](../notes/dell-smci-ai-infra-citi-2026.md)
- 2026-04-20 · MS · [Microsoft 3Q26 前瞻：Azure/Copilot/Capex](../notes/microsoft-3q26-preview-copilot-azure-ms-2026.md)
- 2026-04-23 · JPM · [ServiceNow 1Q26 AI 应用超越客服](../notes/servicenow-1q26-ai-broadening-jpm-2026.md)
- 2026-04-21 · JPM · [SEMCO MLCC/基板双升周期](../notes/samsung-electro-mechanics-mlcc-upcycle-jpm-2026.md)
- 2026-04-16 · MS · [大中华科技硬件：宏观不确定性与 AI 硬件](../notes/greater-china-tech-hardware-macro-ai-ms-2026.md)
- 2026-04-15 · MS · [AI 液冷 TAM 扩大：Vera Rubin POD](../notes/thermal-solutions-liquid-cooling-ai-ms-2026.md)
- 2026-04-15 · MS · [AI 基础设施表外承诺与杠杆风险](../notes/ai-infra-off-balance-sheet-leverage-ms-2026.md)
- 2026-04-20 · MS · [AI 与劳动生产率：产出增长而非裁员](../notes/ai-labor-productivity-output-growth-ms-2026.md)
- 2026-04-23 · Citi · [中国工业 AI 基础设施与具身 AI](../notes/china-industrials-ai-infra-embodied-ai-citi-2026.md)
- 2026-04-23 · GS · [PCB/CCL 涨价与 AI 需求驱动](../notes/pcb-ccl-price-hike-ai-demand-gs-2026.md)
- 2026-04-23 · Jefferies · [PCB/CCL AI 受益初始覆盖](../notes/pcb-ccl-ai-beneficiaries-initiation-jefferies-2026.md)
- 2026-04-16 · GS · [软件护城河 IV：AI 原生机遇](../notes/software-moats-ai-native-gs-2026.md)
- 2026-04-14 · Bernstein · [GenAI 全球软件行业 5 年展望](../notes/genai-global-software-future-bernstein-2026.md)
- 2026-04-16 · MS · [AI 重塑软件开发格局](../notes/ai-software-development-reshape-ms-2026.md)
- 2026-04-15 · UBS · [GitLab AI 叙事拐点](../notes/gitlab-ai-narrative-inflection-ubs-2026.md)
- 2026-04-21 · GS · [Dynatrace/Elastic 可观测性与搜索平台](../notes/dynatrace-elastic-observability-ai-gs-2026.md)
- 2026-04-20 · GS · [日本 IT 服务业 AI 招聘策略](../notes/japan-it-services-ai-hiring-strategies-gs-2026.md)
- 2026-04-15 · GS · [GS 私人软件互联网会议纪要](../notes/private-software-internet-conf-gs-2026.md)

## Related

- [topics/advanced-packaging](advanced-packaging.md) — CoWoS/SoIC（Agentic AI 驱动算力密度需求）
- [topics/memory-supercycle-2026](memory-supercycle-2026.md) — DRAM/HBM 需求端驱动之一
- [topics/pcb-ccl-ai-upgrade](pcb-ccl-ai-upgrade.md) _(待建)_ — PCB/CCL/ABF 上行周期
- [entities/tsmc](../entities/tsmc.md) — TSMC（CPU 工艺节点 N2/A14 关键受益）
