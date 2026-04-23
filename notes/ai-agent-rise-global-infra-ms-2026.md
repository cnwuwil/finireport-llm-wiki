---
title: AI Agent崛起：全球影响与基础设施瓶颈分析（Morgan Stanley全球专题）
type: note
domain: invest
tags: [Agentic AI, CPU TAM, DRAM, ABF基板, 全球半导体, AI基础设施, 算力架构, Morgan Stanley]
created: 2026-04-22
updated: 2026-04-22
source: sources/quant-reports/AI Agent崛起：全球影响与基础设施瓶颈分析.md
broker: Morgan Stanley
date: 2026-04-19
entities: [tsmc]
topics: [agentic-ai-infra, memory-supercycle-2026]
---

# AI Agent崛起：全球影响与基础设施瓶颈分析（Morgan Stanley全球专题）

**来源**：Morgan Stanley（全球技术研究团队），2026-04-19  
引用：Jensen Huang GTC 2026（2026-03-16）："The CPU is no longer simply supporting the model; it's driving it."

---

## 核心主题

- AI从"生成式"转向"自主行动"的**Agent阶段**，GPU需求不减但围绕GPU的系统协调需求大增
- **CPU成为多步骤工作流和系统编排的控制平面**
- Agentic AI将AI算力支出扩展至超出加速器的更广范围：CPU、内存、网络、存储

---

## 关键量化框架

### CPU TAM
- Agentic AI中CPU端处理占总工作负载时间**50-90%**
- 增量CPU TAM 2030E：**$32.5-60bn**（总服务器CPU TAM：$82.5-110bn+）
- 集群级CPU:GPU比例随AI从推理向行动演进而上升

### DRAM
- Agentic AI驱动增量DRAM需求2030E：**15-45 EB**（占2027年年度DRAM供应的26-77%）
- 关键机制：
  - Agent并发+工具I/O驱动更大CPU端工作集
  - KV-cache卸载到DRAM（vLLM等）→ DRAM成为HBM的功能性扩展
- Vera CPU平台：每CPU LPDDR最高1.5TB；AMD EPYC最高8TB+（含CXL）

### ABF基板
- ABF价值增长CAGR：2025-30E **17.9%**（无Agentic增量则为16.1%）
- AI相关应用（GPU/ASIC/CPU/网络）占ABF市场：2024年~50%→ 2030E **75%+**
- Agentic AI使ABF供应缺口从~7%扩大至**~15%**（2030年）→ 推动定价和利润率上行
- 首选：Unimicron、Samsung Electro-Mechanics、Nan Ya PCB；最差：Ibiden（估值偏高）

---

## 全球受益标的矩阵

| 层级 | 标的 |
|------|------|
| CPU | NVDA、Intel、AMD、Arm |
| DRAM | Samsung、Hynix、Micron |
| NAND | Kioxia、SanDisk |
| HDD | Seagate、WDC、TDK |
| Foundry | TSMC |
| IC设计服务 | GUC、Egis |
| PCB/基板/CCL | SEMCO、Unimicron、Nan Ya PCB、Ibiden、Nittobo |
| BMC/内存接口 | Aspeed、Renesas、Montage、WPG |
| MLCC/CPU Socket | Murata、TDK、Yageo、FIT Hon Teng、Lotes |
| ODM/设备 | Wiwynn、Hon Hai |
| 半导体设备 | ASML、ASMi、AMAT、BeSi、KLAC、Tokyo Electron |

---

## 与相关报告对比

- 本报告是全球专题研究（65页），覆盖CPU/DRAM/ABF/设备/大中华半导体全链路
- 与`agentic-ai-hardware-gc-ms-2026`（大中华硬件）、`cloud-semis-non-gpu-agentic-ai-ms-2026`（云半导体）同期发布，互为补充

---

## Related
- [[agentic-ai-hardware-gc-ms-2026]] — Agentic AI驱动CPU TAM扩张：ABF缺口扩至15%（MS）
- [[cloud-semis-non-gpu-agentic-ai-ms-2026]] — 云半导体：非GPU服务器需求增长，Aspeed BMC（MS）
- [[datacenter-watch-gpu-rental-memory-jpm-2026]] — 数据中心GPU租赁价格+内存合约价追踪（JPM）
