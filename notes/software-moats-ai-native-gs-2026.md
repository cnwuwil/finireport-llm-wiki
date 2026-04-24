---
title: 软件护城河再审视IV：重心转移与AI原生机遇
type: note
domain: invest
tags: [软件, SaaS, AI原生, 护城河, CRM, CRWD, GWRE, RBRK, 算力约束, 蒸馏模型, Goldman Sachs]
created: 2026-04-22
updated: 2026-04-22
source: sources/quant-reports/软件护城河再审视：重心转移与AI原生机遇.md
broker: Goldman Sachs
date: 2026-04-16
entities: [salesforce, crowdstrike, guidewire, rubrik]
topics: [agentic-ai-infra]
---

# 软件护城河再审视IV：重心转移与AI原生机遇

**来源**：Goldman Sachs（Revisiting Moats IV），2026-04-16  
**背景**：私人软件&互联网大会（4/8-4/9）+ 硅谷巴士之旅（4/13-4/14），30家私人公司 + 10家上市公司  
**上市公司覆盖**：ADSK、CRM、CRWD、GWRE、IOT、OKTA、RBRK、WDAY、ZS（+ PANW、SNOW 预安静期沟通）

---

## 七大核心结论

### 1. 软件 TAM 持续扩大
- AI 工作流正以"劳动力单元"或"生产力单元"出售 → 进入更大预算池
- 示例：Sierra（原子生产力单位 = 流程，非人）、Salesforce（Agentic Work Units）、Workday（灵活积分 = 工作单元）
- a16z：AI 不是零和游戏，创造更大 TAM；即使毛利率 60%，毛利润绝对值也大幅提升

### 2. 前沿大模型权力重新分配
- 蒸馏模型成本仅为训练父模型的 **2%**
- 厂商正构建独立于单一模型提供商的路线图：
  - Superhuman：97% API 调用通过自研 LLM 路由
  - Intercom：12 个模型混合，重排序器迁移到自研模型后**成本降 80%**
  - Writer：自进化 LLM（5轮训练后与前沿模型性能持平）
- 企业受益：更高效路由 + 更低推理成本 + 不受单一提供商涨价暴露

### 3. 算力是核心约束
- BaseTen：供需失衡远比行业认知严重，推理成本已接近员工成本的 **~10%**，可能在几个季度内达到员工成本量级
- 多云生产成为必须（非可选）：H200/GB200 供应约束 → 客户同时在多云+新云运行推理
- 推理/生产工作负载比训练工作负载更黏性 → 新云提供商收入更持久

### 4. AI 原生占领 SaaS 空白地带
- 传统 SaaS：功能孤岛（CRM、OMS、物流各自独立）
- AI 原生：以结果为中心，跨系统编排，几周内上线，POC 转化率高
- 两大 SaaS 护城河正在弱化：
  - **领域经验**：跨职能数据权限受限，SaaS 厂商缺乏端到端流程视角
  - **数据护城河**：数据属于客户，SaaS 只是托管方；防御性正转向"谁能安全地把数据转化为行动"

### 5. 安全行业：即将到来的大规模修复周期
- 未来 12-18 个月：防守方压力加大（AI 驱动攻击面扩大）
- 触发修复升级周期（类比 Y2K 或 2000 年代防火墙资本支出周期）
- 受益：**CRWD、PANW、Huntress**（SOC 自动化）；**Okta、MSFT**（Agent 身份安全）
- Zscaler：已观察到 Agentic 流量明显增加

### 6. 可观测性：加速但 TCO 压力并存
- Grafana、Datadog 云业务加速（AI 微服务增加 + 数据标注需求）
- 方向：从 Dashboard 转向搜索驱动界面；开放标准降低遥测处理成本
- Grafana 自适应追踪：客户可丢弃 **90%** 发送至基础设施监控的追踪

### 7. Applied AI 正处于 2022 年 GenAI 级别拐点
- Physical Intelligence：通用基础模型（非任务专用）；专有真实世界交互数据飞轮
- Shield AI：Hivemind 软件定义国防平台，支持蜂群级自主行为
- Locus Robotics：~17,000 台机器人部署，RaaS 模式收集真实数据

---

## 推荐标的（公开公司）

| 公司 | 态度变化 | 理由 |
|------|---------|------|
| **CRM** | 更积极 | Agentic 战略更清晰 + 开发工具即将发布 |
| **CRWD** | 更积极 | 多个模块需求改善 |
| **GWRE** | 更积极 | AI 加速云转换，纯 TAM 扩张 |
| **IOT** | 更积极 | ROI 驱动需求，数据/AI 差异化 |
| **RBRK** | 更积极 | Agent Cloud/身份安全拓展故事；韧性需求扩大 |

---

## Related
- [[citi-ai-summit-tech-invest-outlook-2026]] — Citi AI峰会：算力约束与企业采用加速
- [[agentic-ai-hardware-gc-ms-2026]] — Agentic AI 硬件需求驱动因素
