---
title: 先进封装：CoWoS / SoIC / CPO 扩产与投资主题
type: topic
domain: invest
tags: [先进封装, CoWoS, SoIC, CoPoS, CPO, 台积电, TSMC, AI算力, 封装设备, HPC]
status: active
created: 2026-04-23
updated: 2026-04-24
---

# 先进封装：CoWoS / SoIC / CPO 扩产与投资主题

## Thesis（当前论点）

AI 算力密度的提升已超过单一芯片的物理极限，**先进封装成为算力路线图的核心瓶颈与价值创造环节**。2026–2028 年，TSMC CoWoS 产能近乎翻三倍（675k → 3,150k wafers/年），同步带动上游设备商（All Ring、GPTC）、光学互连（CPO）和 3D 堆叠（SoIC）的结构性需求爆发。市场对此主题存在强烈共识，但 CoPoS 等下一代技术的量产时间表仍有分歧。

## 技术层级

| 技术 | 定义 | 状态 | 主要受益公司 |
|---|---|---|---|
| **CoWoS**（2.5D） | GPU/Accelerator + HBM 通过 Interposer 集成 | 量产，高速扩产 | TSMC、All Ring、GPTC |
| **SoIC**（3D） | Chiplet 垂直堆叠，TSMC 版 Foveros | 量产，扩产 | TSMC、GPTC（独家清洗） |
| **CoPoS**（下一代） | 大型重构基板封装，取代 CoWoS 用于超大面积 | 试产，几年内量产 | TSMC |
| **CPO**（共封装光学） | 光学收发器直接封装到交换芯片旁 | 早期放量（2027E 起） | All Ring（AOI 设备）、Innolight、TFC |

## 关键数据点

- TSMC CoWoS 产能：**675k（2025）→ 1,275k（2026E，+89%）→ 2,490k（2027E，+95%）→ 3,150k（2028E，+27%）** wafers/年（GS 2026-04-16 更新）
- CoWoS 需求来源（2027E，各客户贡献）：
  - NVIDIA Vera Rubin NVL144：136k wfpm
  - AMD Helios（MI455）：55k wfpm
  - Broadcom TPU v7/v8ax：52k wfpm
  - AWS Trainium3：15k wfpm
- All Ring 在 CoWoS underfill dispenser 和 TIM heatsink attach 市占率：**接近 100%**
- GPTC 在 CoWoS 湿法清洗市占率：**50%**；在 SoIC 湿法清洗：**独家供应商**
- 光模块/光引擎 TAM：scale-out → CPO scale-up 扩大 **13x**（GS 2026-04-17）

## 各家观点

| 机构 | 日期 | 观点 | 关键数据 | 来源 |
|---|---|---|---|---|
| GS | 2026-04-16 | CoWoS 2027E 产能 2,490k，上调 7.8%；AI/ASIC 双需求扩量 | All Ring TP NT$1,800（+125%），GPTC TP NT$4,500（+29%） | [All Ring & GPTC](../notes/all-ring-gptc-advanced-packaging-gs-2026.md) |
| GS | 2026-04-16 | N3 GM 预计 2H26 超越公司均线 | CoWoS 占 Capex 10-20% | [TSMC 1Q26 GS](../notes/tsmc-1q26-earnings-review-gs-2026.md) |
| Citi | 2026-04-16 | CoPoS 试产线已建，N2 GM 结构性高于 N3 | 先进封装/测试占 Capex 10-20% | [TSMC 1Q26 Citi](../notes/tsmc-1q26-earnings-review-citi-2026.md) |
| Nomura | 2026-04-16 | CoWoS 产能紧张，OSAT 合作补充；CoPoS 几年内量产 | 2027F Capex US$70B（含先进封装） | [TSMC 1Q26 Nomura](../notes/tsmc-1q26-guidance-raise-nomura-2026.md) |
| MS | 2026-04-16 | Intel EMIB 竞争长期，TSMC 开放计算芯片给第三方封装（扩 TAM） | CoWoS + SoIC + SoW 满足大光罩设计需求 | [TSMC 1Q26 MS](../notes/tsmc-1q26-earnings-review-ms-2026.md) |
| MS | 2026-04-20 | TSMC SoIC 产能同步扩张；DeepSeek 触发推理需求爆发 | 头部 4 CSP 4Q25 Capex +64% YoY | [大中华半导体](../notes/greater-china-semis-ai-chips-ms-2026.md) |
| GS | 2026-04-17 | CPO 开始进入 AI 数据中心 scale-across，光模块 TAM 扩 13x | RoboTechnik（CPO 设备）CAGR +69% | [AI 光网络](../notes/optical-networking-cpo-ocs-gs-2026.md) |

## 受益 / 受损矩阵

| 公司 | 关系 | 关键数据 | 来源 |
|---|---|---|---|
| [TSMC](../entities/tsmc.md) | 核心受益：CoWoS/SoIC 量产；定价权强 | CoWoS 3 年产能翻 4.6x | 5 份报告 |
| All Ring（6187.TWO） | 直接受益：CoWoS 设备垄断地位 | 2027E EPS +232%，TP NT$1,800 | [GS](../notes/all-ring-gptc-advanced-packaging-gs-2026.md) |
| GPTC（3131.TWO） | 直接受益：SoIC 独家 + CoWoS 50% | 2027E EPS +183%，TP NT$4,500 | [GS](../notes/all-ring-gptc-advanced-packaging-gs-2026.md) |
| ASE（3711.TW） | 受益：OSAT 伙伴补充 CoWoS 产能缺口 | MS OW | [大中华半导体](../notes/greater-china-semis-ai-chips-ms-2026.md) |
| RoboTechnik（300757） | 受益：CPO 耦合与测试设备领跑 | 2026-28E 营收 CAGR +69% | [GS 光网络](../notes/optical-networking-cpo-ocs-gs-2026.md) |
| Intel | 受损/竞争噪音：EMIB 量产壁垒高 | 管理层："No Shortcuts" | [TSMC 1Q26 MS](../notes/tsmc-1q26-earnings-review-ms-2026.md) |

## 矛盾 / 待解问题

- **CoPoS 量产时间线**：TSMC 称"几年内"，无明确年份；若提前可能影响 CoWoS 设备商的订单节奏
- **CPO 渗透节奏**：All Ring CPO 收入占比 2026E 仅 3%，2027E 跳升至 29%——假设较激进，下行风险不小
- **OSAT 市场份额**：若 CoWoS 供应持续紧张，ASE / Amkor 是否获得更多外包份额存在不确定性
- **CoWoS 产能数据跨来源差异**：GS vs MS 的 2027E 数据（2,490k vs "大幅增加"）口径一致，但 JPM 未单独量化

## Sources

- 2026-04-21 · GS · [All Ring & GPTC 先进封装设备](../notes/all-ring-gptc-advanced-packaging-gs-2026.md)
- 2026-04-17 · GS · [AI 光通信 CPO/OCS（含 CPO 背景）](../notes/optical-networking-cpo-ocs-gs-2026.md)
- 2026-04-17 · JPM · [TSMC 先进制程供应紧张至 2027](../notes/tsmc-leading-edge-supply-tight-jpm-2026.md)
- 2026-04-16 · GS · [TSMC 1Q26 业绩点评](../notes/tsmc-1q26-earnings-review-gs-2026.md)
- 2026-04-16 · Citi · [TSMC 1Q26 业绩点评](../notes/tsmc-1q26-earnings-review-citi-2026.md)
- 2026-04-16 · MS · [TSMC 1Q26 业绩点评](../notes/tsmc-1q26-earnings-review-ms-2026.md)
- 2026-04-16 · Nomura · [TSMC 1Q26 指引上调](../notes/tsmc-1q26-guidance-raise-nomura-2026.md)
- 2026-04-20 · MS · [大中华半导体 AI 芯片全景](../notes/greater-china-semis-ai-chips-ms-2026.md)
- 2026-04-21 · JPM · [Jentech AI GPU 散热器价值量提升](../notes/jentech-ai-gpu-heat-spreader-jpm-2026.md)
- 2026-04-21 · JPM · [SEMCO MLCC/基板双升周期](../notes/samsung-electro-mechanics-mlcc-upcycle-jpm-2026.md)
- 2026-04-17 · JPM · [半导体 1Q26 前瞻](../notes/semis-1q26-preview-jpm-2026.md)
- 2026-04-16 · MS · [半导体测试结构性上升周期](../notes/semis-testing-structural-upcycle-ms-2026.md)
- 2026-04-16 · GS · [ASML EUV 产能与 AI 需求](../notes/asml-euv-ai-demand-gs-2026.md)
- 2026-04-23 · GS · [PCB/CCL 涨价与 AI 需求驱动](../notes/pcb-ccl-price-hike-ai-demand-gs-2026.md)
- 2026-04-23 · Jefferies · [PCB/CCL AI 受益初始覆盖](../notes/pcb-ccl-ai-beneficiaries-initiation-jefferies-2026.md)
- 2026-04-23 · Citi · [中国工业 AI 基础设施与具身 AI](../notes/china-industrials-ai-infra-embodied-ai-citi-2026.md)

## Related

- [entities/tsmc](../entities/tsmc.md) — 台积电实体页（含 5 家 broker 目标价对比）
- [topics/ai-optical-networking](ai-optical-networking.md) — 光通信升级（CPO/OCS 是先进封装下游）
- [topics/agentic-ai-infra](agentic-ai-infra.md) — Agentic AI 驱动算力需求（CoWoS 上游驱动力）
- [topics/ai-capex-2026](ai-capex-2026.md) _(待建)_ — AI Capex 与数据中心
