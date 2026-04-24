---
title: AI 光通信网络升级：800G → 1.6T → 3.2T + CPO + OCS
type: topic
domain: invest
tags: [光通信, 光模块, 800G, 1.6T, 3.2T, CPO, OCS, 硅光子, SiPh, InnoLight, TFC, VPEC, AI数据中心]
status: active
created: 2026-04-23
updated: 2026-04-24
---

# AI 光通信网络升级：800G → 1.6T → 3.2T + CPO + OCS

## Thesis（当前论点）

AI 算力密度的爆炸式增长（GPU 架构从 GB200 → GB300 → Rubin → Feynman）持续推高数据中心互联带宽需求，光通信市场正同步经历规格升级、新技术导入（CPO/OCS/SiPh）和 TAM 持续扩张的三重浪潮。GS 估算光网络 TAM 将扩大 9 倍至 **US$154B**；ASIC 占比提升（43% → 55%，2026–28E）进一步加速铜转光、可插拔转 CPO 的迁移节奏。

## 关键数据点

- 全球光模块 TAM：$34.2B（2025A）→ **$50.9B（2026E）→ $72.6B（2027E）**（GS）
- 800G+ 占比：39%（2025A）→ 63%（2026E）→ **81%（2028E）**（GS）
- OCS 市场：~$4 亿（2025）→ **>$25 亿（2029E）**，CAGR 58%（Nomura）
- 光模块/光引擎 TAM 扩张倍数：scale-out → CPO scale-up = **13x**（GS）
- SiPh 渗透率：800G 60%（2026E）→ 77%（2028E）；1.6T 80%（2026E）→ 100%（2028E）
- ASIC 占 AI 芯片比例：43% → 50% → 55%（2026–28E，GS）
- 光网络 TAM 解锁路径：$17B（当前）→ **$154B**（AI scale-up + CPO 全部实现）（GS 720）

## 技术层级与速率路线图

### 速率升级路径

| NVIDIA 架构 | GPU 层速率 | Leaf/Spine 速率 | 1.6T per GPU |
|---|---|---|---|
| GB200（当前主流） | 400G | 800G | — |
| **GB300**（2026 放量） | 800G | **1.6T** | 3.0 |
| Rubin（2027） | 800G/1.6T | **3.2T** | 6.0 |
| Feynman（2028） | 1.6T | 3.2T | 6.0 |

### 技术架构

| 技术 | 场景 | 关键特性 | 代表厂商 |
|---|---|---|---|
| **可插拔（Pluggable）** | Scale-out（机架间） | 当前主流，成本最低 | Innolight、TFC、Eoptolink |
| **CPO**（共封装光学） | Scale-up（机架内高速） | 能耗降至 48pJ/bit | Innolight/TeraHop、RoboTechnik（设备） |
| **OCS**（光路交换） | Scale-across（跨集群） | 延迟 10-100ns，功耗 1/5 电交换 | InnoLight/TeraHop、Accelink、TFC |
| **CPO + OCS 组合** | 完整光架构 | 能耗 31pJ/bit（vs 可插拔 83pJ/bit）| NVIDIA 下一代架构 |

## 各家观点

| 机构 | 日期 | 核心判断 | 首选标的 | 来源 |
|---|---|---|---|---|
| GS | 2026-04-17 | 800G+ 出货量上调 14-33%；SiPh 渗透 60-100%；ASIC 扩张加速铜转光 | Innolight（Buy）、TFC、VPEC、Landmark、RoboTechnik | [全球光模块 800G](../notes/global-optical-transceiver-800g-ai-gs-2026.md) |
| GS | 2026-04-17 | 光网络 TAM 扩至 $154B；1.6T → 3.2T 升级；Innolight TP +50% | Innolight TP Rmb1,187 | [GS 720 摘要](../notes/gs-720-digest-optical-robotaxi-mediatek-2026.md) |
| GS | 2026-04-17 | CPO 设备初始覆盖；RoboTechnik 精度 5nm 运动控制护城河；三家平均 CAGR +66% | RoboTechnik Buy Rmb688；YJ Semi/YOFC Neutral | [AI 光网络](../notes/optical-networking-cpo-ocs-gs-2026.md) |
| Nomura | 2026-04 | OCS 市场 2025–29E CAGR 58%；InnoLight/TFC 是早期布局者 | InnoLight Buy、TFC Buy | [OCS AI 网络](../notes/ocs-ai-network-china-optics-nomura-2026.md) |

## 受益矩阵

### 光模块 / 光引擎

| 公司 | 定位 | 评级/目标价 | 关键数据 | 来源 |
|---|---|---|---|---|
| **Innolight（300308）** | 光模块/CPO/OCS（TeraHop 子公司） | GS Buy Rmb1,187（TP +50%）；Nomura Buy | 连续 8 季度 GM 扩张；TeraHop SiPh 64x64 + 300x300 OCS 展示 | [GS 720](../notes/gs-720-digest-optical-robotaxi-mediatek-2026.md)、[Nomura OCS](../notes/ocs-ai-network-china-optics-nomura-2026.md) |
| **TFC Optical（300394）** | 光纤准直阵列（FAU，OCS 核心元件）+ 光模块 | GS Buy；Nomura Buy | OCS FAU 是 MEMS 方案关键元件 | [GS 光模块](../notes/global-optical-transceiver-800g-ai-gs-2026.md)、[Nomura OCS](../notes/ocs-ai-network-china-optics-nomura-2026.md) |
| VPEC | SiPh 激光器 | GS Buy | 1.6T SiPh 渗透受益 | [GS 光模块](../notes/global-optical-transceiver-800g-ai-gs-2026.md) |
| Landmark | CW 激光器 / 外延片 | GS Buy | SiPh 1.6T 模块成本 $15-20 vs EML $160 | [GS 光模块](../notes/global-optical-transceiver-800g-ai-gs-2026.md) |
| Eoptolink | 光模块 + OCS（MEMS 整机） | GS Buy；NC（Nomura） | NX200/NX300 展示（140/320 端口 OCS） | [GS 光模块](../notes/global-optical-transceiver-800g-ai-gs-2026.md)、[Nomura OCS](../notes/ocs-ai-network-china-optics-nomura-2026.md) |

### 设备层

| 公司 | 定位 | 评级 | 关键数据 | 来源 |
|---|---|---|---|---|
| **RoboTechnik（300757）** | CPO 耦合与测试设备；精度 5nm 运动控制 | GS Buy Rmb688（+42.7%） | 营收 CAGR 2025-28E +69%；2027E CPO 占收入 29% | [GS AI 光网络](../notes/optical-networking-cpo-ocs-gs-2026.md) |

### 系统 / 平台层

| 公司 | 定位 | 来源 |
|---|---|---|
| NVIDIA | Dragonfly 架构 + CPO+OCS 组合方案 | [Nomura OCS](../notes/ocs-ai-network-china-optics-nomura-2026.md) |
| Google | Apollo MEMS OCS 平台（降本 30%、降耗 40%）；最大 OCS 客户 | [Nomura OCS](../notes/ocs-ai-network-china-optics-nomura-2026.md) |
| Meta / Microsoft | 2026 年小批量 OCS 测试 | [Nomura OCS](../notes/ocs-ai-network-china-optics-nomura-2026.md) |
| Ruijie | 数据中心交换机 | [GS 光模块](../notes/global-optical-transceiver-800g-ai-gs-2026.md) |

## 矛盾 / 待解问题

- **CPO 大规模商用时间线**：GS/Nomura 均描述 CPO 2026–2027E "起量"，但 Citi 在大立光报告中指出"CPO 1–2 年内不会落地"（指大立光的 CPO 机遇），口径存在出入——可能是 AI 数据中心 CPO（起量）vs 手机/消费级 CPO（延迟）的不同场景
- **OCS SiPh 损耗问题**：SiPh OCS 理论切换最快但插入损耗高（6dB vs MEMS <3dB），限制了规模应用；Innolight/TeraHop 的路径是否能解决此问题未有确认
- **Scale-out vs Scale-up 比例**：铜缆和可插拔模块短期内不会消失，GS TAM $154B 需要 CPO 全面落地；实际渗透节奏决定时间窗口
- **Innolight 双重覆盖（GS+Nomura）**：两家均给 Buy，但目标价方法和时间表有差异，需确认是否一致

## Sources

- 2026-04-17 · GS · [全球光模块 800G+ TAM 更新](../notes/global-optical-transceiver-800g-ai-gs-2026.md)
- 2026-04-17 · GS · [GS 720 摘要：光网络 TAM $154B](../notes/gs-720-digest-optical-robotaxi-mediatek-2026.md)
- 2026-04-17 · GS · [AI 光通信 CPO/OCS 初始覆盖](../notes/optical-networking-cpo-ocs-gs-2026.md)
- 2026-04 · Nomura · [OCS 光路交换：AI 网络核心](../notes/ocs-ai-network-china-optics-nomura-2026.md)
- 2026-04-15 · Citi · [大立光 CPO/iPhone 短期业绩](../notes/largan-cpo-iphone-citi-2026.md)

## Related

- [topics/advanced-packaging](advanced-packaging.md) — CPO 是先进封装下游（All Ring CPO 设备）
- [topics/agentic-ai-infra](agentic-ai-infra.md) — AI Agent 算力增长驱动光通信带宽需求
- [topics/ai-capex-2026](ai-capex-2026.md) _(待建)_ — CSP Capex 是光模块采购的上游
