---
title: AI基础设施的资产负债表外承诺与潜在杠杆风险（Morgan Stanley）
type: note
domain: invest
tags: [AI基础设施, 资产负债表外, 超大规模云厂商, NVDA, GOOGL, META, MSFT, AMZN, ORCL, 数据中心融资, Morgan Stanley]
created: 2026-04-22
updated: 2026-04-22
source: sources/quant-reports/AI基础设施的资产负债表外承诺与潜在杠杆风险.md
broker: Morgan Stanley
date: 2026-04-15
entities: [nvda, microsoft]
topics: [agentic-ai-infra]
---

# AI基础设施的资产负债表外承诺与潜在杠杆风险（Morgan Stanley）

**来源**：Morgan Stanley，2026-04-15

---

## 核心观点

- 超大规模云厂商+NVDA合计已签订**>$1.3T**承诺（$640bn采购 + $675bn租赁）
- 大多数承诺为**表外义务**，会计规则将负债确认延迟至交付/租赁开始/付款可能性触发时
- META承诺规模约为**~1.7x预期经营现金流**；ORCL **>7x**
- 承诺通常支撑供应商/开发商的基础设施融资，若AI需求下行，重新谈判困难

---

## 承诺类型分析

### 1. 无条件采购义务（Purchase Commitments）
- 过去一年已翻倍，5年内增长**6x**
- 适用范围：芯片（NVDA存货+采购承诺占FY27营收预期~32%）、算力、电力、数据中心土地
- 表外处理直至商品/服务交付；若无预期亏损，不做账面记录

### 2. 租赁（Leases）
- 表内租赁：$82bn融资租赁 + $175bn经营租赁（合计>$230bn）
- **未开始的租赁（表外）：>$670bn**，较一年前$240bn增加$435bn
- 常见表外例外：未开始的租赁、可变租赁付款（超出时间流逝的支付）、续租选项、剩余价值担保（RVG）、第三方担保

### 3. 电力采购协议（PPA）
- GOOGL已签订20年PPA，处理为租赁（$9.9bn未来付款）
- META与Vistra/Constellation签订20年协议，估计年花费$350-430mn，但未在财报中披露具体金额
- ORCL电力相关承诺：$11bn（截至2026年2月）

### 4. 芯片融资结构
- **合约背书贷款（SPV）**：CRWV模式，获取-或-付款合约→SPV借款→支付GPU
- **客户预付款**：超大规模云厂商预付算力合约
- **芯片租赁SPV**：私人信用+JV结构，ORCL管理层提及但尚未成规模
- 即使通过SPV结构，评级机构仍可能将其视为债务处理

---

## GOOGL租赁背书（Backstops）案例

| 开发商 | 地点 | 规模 | GOOGL背书金额 |
|--------|------|------|--------------|
| Cipher | TX | ~300MW | ~$1.733bn |
| Hut 8 | LA | 245MW | ~$7bn（含租赁义务） |
| TeraWulf | NY | 378MW | ~$3.2bn |
| Flash Compute | TX | 168MW | ~$1.3bn |

- GOOGL合计提供>$10bn租赁背书
- S&P将在租赁生效时调整GOOGL债务；$100背书可能产生~$79债务调整

---

## 重要会计规则

- 合约要构成**租赁（Lease）**需满足：识别特定资产 + 客户获得实质全部经济利益 + 客户控制使用权
- 大多数算力合约**不识别具体GPU/机架**，因此通常为表外处理
- **剩余价值担保（RVG）**：仅"可能"发生的付款纳入租赁负债；管理层判断空间大
- PPA会计处理：可为租赁/采购承诺/衍生品，取决于合约条款

---

## 关键数据

| 公司 | 承诺/NTM OCF |
|------|-------------|
| META | ~1.7x |
| ORCL | >7x |
| MSFT | 较高（已超越年度折旧） |
| GOOGL | 较高（未开始租赁快速增长） |
| AMZN | 较高（含PPA衍生品） |

---

## Related
- [[nvda-gpu-architecture-ecosystem-ubs-2026]] — 英伟达GPU架构与生态优势（UBS）
- [[cloud-semis-non-gpu-agentic-ai-ms-2026]] — 云半导体非GPU需求（MS）
- [[datacenter-watch-gpu-rental-memory-jpm-2026]] — 数据中心GPU租赁价格追踪（JPM）
