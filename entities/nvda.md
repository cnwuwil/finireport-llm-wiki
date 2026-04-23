---
title: 英伟达（NVIDIA）
type: entity
domain: invest
tags: [NVIDIA, NVDA, GPU, CUDA, AI算力, Blackwell, Hopper, CoWoS, AI加速器, 数据中心]
aliases: [英伟达, NVIDIA, NVDA]
created: 2026-04-23
updated: 2026-04-23
---

# 英伟达（NVIDIA）

**股票代码**：NVDA（纳斯达克）  
**行业**：AI 加速器 / GPU / 数据中心  
**总部**：美国加利福尼亚州圣克拉拉  

## 一句话定位

AI 算力时代的核心基础设施供应商，GPU + CUDA 生态形成双重护城河；架构持续演进（Hopper → Blackwell → Rubin → Feynman）驱动数据中心光通信规格升级和先进封装需求。

## 架构路线图与光通信影响

| 架构 | 代表芯片 | GPU 层速率 | Leaf/Spine 速率 | 1.6T per GPU | CoWoS 需求 |
|---|---|---|---|---|---|
| Hopper | H100/H200 | 400G | 800G | — | 已量产 |
| **Blackwell** | GB200/GB300 | 400G→**800G** | 800G→**1.6T** | 3.0（GB300） | 2026 主力 |
| Rubin | — | 800G/1.6T | **3.2T** | 6.0 | 2027E |
| Feynman | — | 1.6T | 3.2T | 6.0 | 2028E |

## 核心竞争优势（UBS 分析）

- **模型架构多样化有利 GPU**：从 Transformer → MoE → SSM 持续演化，通用计算优于固定功能 ASIC
- **CUDA 护城河**：内部建模/仿真/基准测试竞争架构的能力被大多数投资者低估
- **供应链关系**：NVDA 正成为 TSMC、光学器件等关键系统组件的**最大客户**，本身构成竞争优势
- **系统级协同设计**：相比 AI ASIC 毛利率 ~65%，NVDA 70%+，且系统级优势还在扩大

## 竞争格局

| 竞争对手 | 类型 | 状态 |
|---|---|---|
| AMD（MI450/Helios） | 自研 GPU | Venice 服务器 CPU 领先，但 GPU 估值已反映预期 |
| Broadcom / Google TPU / AWS Trainium | AI ASIC | 2028E ASIC 占比 55%，长期分流 NVDA 份额 |
| Intel TeraFab | 铸造代工 | 进展缓慢，管理层认为短期内不威胁 NVDA 客户 |
| 中国 GPU（华为 Ascend） | 国内替代 | 出口限制反而加速中国软件栈独立 |

## Blackwell 供需（2026）

- B200 GPU 租赁价格：$5.47/hour（2026-03），单月 +23.5%（JPM 追踪）
- B200/H100 价格比：2.07x（2026-03），从 Sep-25 的 2.63x 压缩后反转
- 供应紧张：N5 以下 TSMC 稼动率 100%+（JPM）

## Vera Rubin 平台（2027E）

- NVL144 机架，功率 10 GW 级别（与 OpenAI 大型项目绑定）
- CoWoS 需求贡献（2027E）：136k wafers/年（MS 大中华半导体数据）
- 全机架液冷（VR POD）：AVC/Fositek OW（MS）

## 矛盾 / 待解问题

- **ASIC 占比加速**（43% → 55%，2026–28E）：长期是否威胁 NVDA 主导地位？UBS 认为模型演化速度使 ASIC 风险有限，但市场分歧持续
- **中国市场出口管制**：NVDA 视 CUDA 在中国发展有战略价值，但硬件销售受限，H200 渗透 vs 国产 GPU 的份额争夺是变量
- **SOX 超涨后估值压力**（UBS，2026-04-20）：SOX 单月 +20% 历史上次月仅 +1.3%

## Sources

- 2026-04-20 · UBS · [GPU 架构 vs ASIC，WFE 超级周期](../notes/nvda-gpu-architecture-ecosystem-ubs-2026.md)
- 2026-04-20 · MS · [大中华半导体 AI 芯片全景](../notes/greater-china-semis-ai-chips-ms-2026.md)（Rubin 客户 CoWoS 数据）
- 2026-04-17 · GS · [全球光模块 800G+](../notes/global-optical-transceiver-800g-ai-gs-2026.md)（架构驱动光通信需求）

## Related

- [entities/tsmc](tsmc.md) — 制造合作伙伴（CoWoS 为 NVDA GPU 最大客户）
- [topics/advanced-packaging](../topics/advanced-packaging.md) — CoWoS 需求核心驱动
- [topics/ai-optical-networking](../topics/ai-optical-networking.md) — 架构升级驱动光通信带宽需求
- [topics/agentic-ai-infra](../topics/agentic-ai-infra.md) — Agentic AI 系统架构演进
