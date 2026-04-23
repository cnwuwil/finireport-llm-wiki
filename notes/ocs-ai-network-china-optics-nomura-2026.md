---
title: 光路交换成为AI网络核心，中国光器件厂商受益
type: note
domain: invest
tags: [OCS, CPO, 光路交换, AI网络, InnoLight, TFC, Accelink, Eoptolink, 光通信, MEMS]
created: 2026-04-22
updated: 2026-04-22
source: sources/quant-reports/光路交换成为AI网络核心，中国光器件厂商受益.pdf
broker: Nomura
date: 2026-04
entities: []
topics: [ai-optical-networking]
---

# 光路交换成为AI网络核心，中国光器件厂商受益

**来源**：Nomura Global AI Trend Tracker，2026-04  
**核心结论**：OCS（光路交换机）正成为 AI 网络的重要组件；中国厂商（InnoLight、TFC 等）是早期布局者

---

## OCS 市场规模

- 2025 年市场规模：~USD 4 亿（Google 主导）
- 2029E 市场规模：>USD 25 亿
- CAGR：~58%（2025-2029E）
- 2026 年：Microsoft、Meta、NVIDIA 均在小批量测试阶段

---

## OCS 核心优势（vs 电交换机）

| 指标 | OCS | 传统电交换机 |
|------|-----|------------|
| 延迟 | ~10-100ns（纳秒级）| 电交换 + 包处理高延迟 |
| 功耗 | 约为同带宽电交换机的 1/5 | 高 |
| 带宽 | 协议透明，支持多种传输速率 | 受 SerDes 速率限制 |
| 光电转换 | 不需要 | 需要 |

**功耗对比（NVIDIA 数据）**：
- 可插拔光模块：83 pJ/bit
- 可插拔 + OCS：50 pJ/bit
- CPO：48 pJ/bit
- **CPO + OCS：31 pJ/bit**（比可插拔方案低 2.6×）

---

## OCS 四大技术路线

| 技术 | 代表厂商 | 端口数 | 切换时间 | 插入损耗 | 可靠性 |
|------|---------|-------|---------|---------|-------|
| MEMS | Lumentum、Accelink、Eoptolink | 大 | 中等(25ms) | 低(<3dB) | 低 |
| DLC（数字液晶） | Coherent | 大 | 慢(100ms) | 低(<3dB) | 高 |
| DLBS | Polatis | 小 | 中等 | 低(<3dB) | 高 |
| SiPh（硅光子） | iPronics、TeraHop(InnoLight子) | 小 | 快(1ms) | 高(6dB) | 高 |

- **MEMS**：当前最成熟，Google "Apollo" 平台基于 MEMS，实现降本 30%、降耗 40%
- **SiPh**：理论上达纳秒级切换，但面临高损耗和串扰挑战

---

## OCS 应用场景

- **Scale-up（纵向扩展）**：Google TPU 互联（3D Torus 拓扑），灵活分配碎片化算力
- **Scale-out（横向扩展）**：替代第 1-2 层电交换机，降低延迟和功耗
- **Scale-across（跨集群）**：多楼多园区互联，NVIDIA 下一代 Dragonfly 架构中用于跨机柜/跨集群全光交换

---

## 中国受益厂商

### 整机/系统层
| 公司 | 评级 | OCS 进展 |
|------|------|---------|
| **InnoLight（300308.CH）** | Buy | 子公司 TeraHop 已展示 SiPh 64x64 和 300x300 OCS（OFC 2026）；早期布局者 |
| Accelink | NC | MEMS 全链路能力；已展示 320x320 OCS（OFC 2026） |
| Eoptolink | NC | 展示 NX200/NX300（140/320 端口），自研 MEMS 镜阵列 |
| Advanced Fiber Resources | NC | 收购武汉 Jabil；与 Calient 合作展示 320x320 OCS |
| Taclink | NC | 硅基 OCS，已与 NVIDIA 联合开发"光子路由引擎" |

### 关键光学元件层
| 公司 | 评级 | 供应内容 |
|------|------|---------|
| **TFC/Suzhou TFC（300394.CH）** | Buy | 光纤准直阵列（FAU）——OCS 核心元件 |
| OptowideTechnologies | NC | 铒钒晶体材料（DLC 方案）+ 准直器 |
| Focuslight Technologies | NC | 镜头、V 槽、光纤耦合器/准直器 |
| Sai Microelectronics（持有 Silex Sweden） | NC | MEMS 芯片代工 |

---

## OCS 产业链结构

**上游**（核心元件）：
- MEMS 阵列、光学滤波器、光纤准直阵列（FAU）、镜头阵列
- 主要供应商：Silex（全球）、TFC/T&S/EverProX（中国）

**中游**（OCS 整机制造/代工）：
- 全球：Coherent、Lumentum、iPronics、Polatis
- 中国：Accelink、Eoptolink、InnoLight/TeraHop、Taclink

---

## OCS vs CPO 定位

- **CPO**：高速短距交换（机架/TOR/Leaf 层），主攻 scale-up
- **OCS**：拓扑重构、Spine 层、DCI，互补于 CPO 和可插拔
- NVIDIA 正开发 CPO + OCS 组合方案，两者互补而非竞争

---

## Related
- [[ai-optical-network-optics-china]] — AI 光通信产业链分析
- [[greater-china-tech-hardware-macro-ai-ms-2026]] — 大中华科技硬件：CPO/网络升级机遇
- [[largan-cpo-iphone-citi-2026]] — 大立光 CPO 机遇评估
