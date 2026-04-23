# Wiki Log

_append-only，最新在最上_

---

## [2026-04-23] phase3-synthesis | 首批 topics + entities 回填

- 新建 entity: entities/tsmc.md（合成 5 份 broker 报告：GS/Citi/MS/Nomura/JPM；含分析师覆盖对比表、CoWoS 产能路径、节点路线图）
- 新建 entity: entities/nvda.md（UBS + GS + MS；架构升级路线图 + 竞争格局）
- 新建 entity: entities/apple.md（GS + MS F2Q26；毛利率分歧分析）
- 新建 entity: entities/celestica.md（BofA；AMD Helios/Google TPU/数字原生三线）
- 新建 topic: topics/advanced-packaging.md（8 份来源；CoWoS 产能路径、All Ring/GPTC/ASE 受益矩阵）
- 新建 topic: topics/agentic-ai-infra.md（4 份来源；MS 全球专题；CPU TAM/DRAM/ABF 量化框架）
- 新建 topic: topics/memory-supercycle-2026.md（5 份来源；DRAM/NAND/NOR/HBM 全线受益矩阵）
- 新建 topic: topics/ai-optical-networking.md（4 份来源；800G→3.2T 路线图；OCS CAGR 58%；Innolight/TFC/RoboTechnik）
- 更新 frontmatter：16 个 notes 补填 entities:/topics: 字段（双向链接基础）
- 更新 index.md：Topics 区块填充 4 个主题页；Entities 区块新增 TSMC/NVDA/Apple/Celestica

## [2026-04-23] meta | Phase 1+2 wiki 管理规则重构
- 背景：对照 Karpathy LLM Wiki pattern，当前 wiki 偏"笔记堆"，缺少 entity/topic 合成层
- 改动：
  - 重写 `SCHEMA.md`：新增 4 种页面类型（entity/concept/topic/note）模板、摄入 7 步 checklist、Lint checklist、交叉引用双向一致性规则
  - 重写 `CLAUDE.md`：编码"复利式维护"哲学，指向 SCHEMA.md 为单一真实来源，加入 ingest 后自检清单
  - 新建 `topics/` 目录 + `topics/README.md`：列出 Phase 3 候选主题（16 个），执行规则
  - 重构 `index.md`：从 170 行平铺 → 按 Topic/Entity/Concept/Note 分层，notes 按 11 个主题分组便于 Phase 3 合成
- 范围：仅规则与骨架，不回填旧 notes；下一次 ingest 起按新规则执行
- 后续：Phase 3（Sonnet）按 `topics/README.md` 候选清单逐个合成主题页 + 回建高频 entity 页

## [2026-04-23] ingest | ServiceNow：一季度表现超预期，AI应用超越客服中心驱动增长（JPM）
- 来源：J.P. Morgan，2026-04-19/20
- 创建 note: notes/servicenow-1q26-ai-broadening-jpm-2026.md（OW PT $195/合作伙伴1Q26"出色"超预期/BFSI+制造业最强/AI许可证改革嵌入所有层级/消费型定价约20%/AI场景从客服中心扩展至IT L1-L3/HR/安全后台自动化）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-23] ingest | Sandisk：NAND供应持续紧张，ASP预期上调（BofA）
- 来源：Bank of America Global Research（Wamsi Mohan），2026-04-18
- 创建 note: notes/sandisk-nand-supply-tight-asp-bofa-2026.md（Buy PO $1,080/数据中心占比1%→15%/F3Q26E ASP +70% QoQ/GM 51%→78.5% F4Q28/2027E EPS $110.62/长期合同策略）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-23] ingest | PCB/CCL：AI浪潮核心受益者，材料升级与技术创新驱动增长（Jefferies初始覆盖）
- 来源：Jefferies，2026-04-20（推测）
- 创建 note: notes/pcb-ccl-ai-beneficiaries-initiation-jefferies-2026.md（WUS/Delton/Shengyi全部Buy/AI PCB TAM $7bn→$75bn 5年60% CAGR/AI CCL $3bn→$39bn 70% CAGR/PCB单GPU价值量升3-5x/M8→M9/10材料升级/中国大陆维持>50%生产份额）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-23] ingest | PCB/CCL行业：下半年价格有望进一步上涨，AI需求驱动产能扩张（Goldman Sachs）
- 来源：Goldman Sachs Global Investment Research，2026-04-18
- 创建 note: notes/pcb-ccl-price-hike-ai-demand-gs-2026.md（4月涨价10-40%+ QoQ/2H26-2027预计再涨/AI PCB/CCL仅占CSP Capex 0.1-1.2%→涨价阻力小/EMC PT NT$4,020/TUC PT NT$1,165/GCE PT NT$1,380/ZDT PT NT$338/AI规格2027升至6+N+6 HDI）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-23] ingest | MCU：周期触底但复苏乏力，边缘AI与内存价格是关键变量（Morgan Stanley）
- 来源：Morgan Stanley Greater China Technology Semis，2026-04-17
- 创建 note: notes/mcu-cycle-bottoming-edge-ai-ms-2026.md（L形复苏/现货价4月大涨但合同价有限/内存成本压制消费电子/Espressif OW PT Rmb175下调12%/Nuvoton UW PT NT$98上调/GigaDevice PT Rmb301/边缘AI长期机遇）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-23] ingest | Dynatrace与Elastic：AI时代可观测性与搜索平台（Goldman Sachs）
- 来源：Goldman Sachs Global Investment Research，2026-04-21
- 创建 note: notes/dynatrace-elastic-observability-ai-gs-2026.md（DT Buy $45/ESTC Neutral $50/六大可观测性主题/DPS续约重置增长算法/Palo Alto $3.35B收购Chronosphere/Databricks Lakewatch/Snowflake收购Observe $1B）
- MD已存在于sources/quant-reports/，补录index.md（Invest/Notes、Sources）
- 原始 PDF 移至 raw-pdf/

## [2026-04-23] ingest | 中国工业策略再审视：更看好AI基础设施与具身AI（Citi）
- 来源：Citi Research（Eric Lau, Jamie Wang, Alice Cai），2026-04-15
- 创建 note: notes/china-industrials-ai-infra-embodied-ai-citi-2026.md（哑铃策略/KBL+Han's Laser+Shengyi AI-infra Top Buys/Hengli+UBTech+LD具身AI/1Q26 AI+具身AI私募M&A占比17.6% vs 1Q25的9.4%/$211bn总规模/Top Sells含CRRC/Topband/Heli）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | Celestica：AMD Helios+Google TPU+数字原生客户驱动增长（BofA）
- 来源：Bank of America Global Research（Ruplu Bhattacharya），2026-04-20
- 创建 note: notes/celestica-google-tpu-digital-native-bofa-2026.md（BUY PT $430↑/AMD Helios R&D+制造→数十亿TAM+新超大规模客户/1.6T白盒交换3家超大规模全部承诺/Google TPU美国+泰国扩产/Digital Native 2027爬坡数十亿/2026E营收$17bn +38%/EPS $8.83 +46%）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | AI Agent崛起：全球影响与基础设施瓶颈（Morgan Stanley全球专题）
- 来源：Morgan Stanley，2026-04-19
- 创建 note: notes/ai-agent-rise-global-infra-ms-2026.md（CPU TAM +$32.5-60bn/DRAM +15-45EB占供应26-77%/ABF缺口扩至15%/全球受益标的矩阵/CPU占Agentic工作负载50-90%）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | AI重塑软件开发格局：更多软件与开发者需求演变（Morgan Stanley）
- 来源：Morgan Stanley，2026-04-16
- 创建 note: notes/ai-software-development-reshape-ms-2026.md（TEAM PT $290→$120/JFrog近期最受益/Agentic SDLC/AI驱动软件增量/开发者岗位从$49K→$55K/初级受压高级稳健）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | AI与劳动生产率：高AI暴露行业靠产出增长而非裁员（Morgan Stanley宏观）
- 来源：Morgan Stanley，2026-04-20
- 创建 note: notes/ai-labor-productivity-output-growth-ms-2026.md（高AI行业2025年生产率+5.7%/贡献1.7pp/数据处理+19.1%/计算机系统设计+13.2%/产出驱动非裁员/AI资本深化）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | AI液冷TAM扩大：Vera Rubin POD全机架液冷，AVC/Fositek OW（MS）
- 来源：Morgan Stanley，2026-04-15
- 创建 note: notes/thermal-solutions-liquid-cooling-ai-ms-2026.md（AVC PT NT$2,750 +20%/Fositek PT NT$2,150 +8%/VR POD全机架液冷/CPO交换机纳入液冷TAM/2Q26再创记录）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | GitLab：AI叙事拐点未至，需求前景喜忧参半（UBS）
- 来源：UBS，2026-04-15
- 创建 note: notes/gitlab-ai-narrative-inflection-ubs-2026.md（Neutral PT $24/1.8x CY27 Revs/DAP FY28+催化剂/开发者席位稳定/AI颠覆风险温和/JFrog首选）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | AI驱动光通信网络升级：初始覆盖RoboTechnik/YJ Semi/YOFC（GS）
- 来源：Goldman Sachs，2026-04-17
- 创建 note: notes/optical-networking-cpo-ocs-gs-2026.md（RoboTechnik Buy PT Rmb688/YJ Semi Neutral PT Rmb1592/YOFC Neutral PT HK$255，平均CAGR 66%，光模块TAM 13x，CPO+OCS+1.6T升级）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 半导体测试结构性上升周期：AI驱动测试强度提升（Morgan Stanley）
- 来源：Morgan Stanley，2026-04-16
- 创建 note: notes/semis-testing-structural-upcycle-ms-2026.md（初始OW覆盖Hon Precision/MPI/WinWay/KYEC/Advantest/Chroma/Leeno，CAGR 66-71%，HBM测试时长5-10x，CPO测试新机遇）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | AI基础设施表外承诺与杠杆风险（Morgan Stanley）
- 来源：Morgan Stanley，2026-04-15
- 创建 note: notes/ai-infra-off-balance-sheet-leverage-ms-2026.md（>$1.3T表外承诺/META~1.7x OCF/ORCL>7x/GOOGL>$10bn租赁背书/芯片融资SPV结构/PPA会计处理）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 中国互联网：即时零售投资趋缓，阿里AI资本再配置（Bernstein）
- 来源：Bernstein Research，Robin Zhu，2026-04-15
- 创建 note: notes/china-internet-instant-retail-ai-capex-bernstein-2026.md（即时零售RMB120bn投入趋缓/阿里AI capex RMB40bn→Alicloud+7-8%/JD 2027E PE ~7x/腾讯12.7x/BABA O PT $180/JD O PT $36）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 中国电商1Q26：行业GMV+7.5%，关注平台竞争与AI购物助手（GS）
- 来源：Goldman Sachs，2026-04-17
- 创建 note: notes/china-ecommerce-1q26-ai-competition-gs-2026.md（BABA+5%/PDD+9%/抖音Doushengsheng/AI购物助手MCP/本地服务竞争）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 云半导体：非GPU服务器需求增长，Aspeed BMC受益（Morgan Stanley）
- 来源：Morgan Stanley，2026-04-19
- 创建 note: notes/cloud-semis-non-gpu-agentic-ai-ms-2026.md（Agentic AI CPU TAM +$32.5-60B/Aspeed BMC 70%份额/AST2700 ASP+40-50%/PT NT$15,555）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 英伟达：GPU架构灵活性与生态优势巩固长期竞争力（UBS SemiBytes）
- 来源：UBS，2026-04-20
- 创建 note: notes/nvda-gpu-architecture-ecosystem-ubs-2026.md（Jensen Huang播客/GPU vs ASIC架构优势/中国五层蛋糕/SOX超涨短期风险/WFE超级周期）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 腾讯控股1Q26前瞻：游戏/广告韧性，AI投入压营业利润（Citi Research）
- 来源：Citi Research，2026-04-19
- 创建 note: notes/tencent-1q26-preview-ai-gaming-citi-2026.md（游戏+11.7%/广告+17%/Hunyuan 3.0/Yuanbao MAU 1.14亿/Agent矩阵，Buy HK$783）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 台积电1Q26点评：AI抵消智能手机/PC疲软，3年Capex US$200B（MS）
- 来源：Morgan Stanley，2026-04-16
- 创建 note: notes/tsmc-1q26-earnings-review-ms-2026.md（3年Capex模型/2027E EPS+17%/IntelEMIB竞争分析，OW NT$2,588）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 台积电1Q26点评：N2 GM高于N3，Buy NT$2,875（Citi Research）
- 来源：Citi Research，2026-04-16
- 创建 note: notes/tsmc-1q26-earnings-review-citi-2026.md（N2 GM>N3/A14节点/Capex结构分解/四家broker EPS对比）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | GS 720摘要：光网络TAM扩张/Robotaxi/MediaTek AI ASIC（Goldman Sachs）
- 来源：Goldman Sachs，2026-04-17
- 创建 note: notes/gs-720-digest-optical-robotaxi-mediatek-2026.md（光网络TAM $154B/Innolight+50%/WeRide+PonyAI Buy/MediaTek ASIC 2027E $12.3B）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 台积电先进制程供应紧张至2027，目标价升至NT$2500（J.P. Morgan）
- 来源：J.P. Morgan，2026-04-17
- 创建 note: notes/tsmc-leading-edge-supply-tight-jpm-2026.md（N5以下UTR 100%+/2027定价+4-5%/N2 2028 150k/3年Capex ~$190-200B，OW PT NT$2,500）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 台积电1Q26指引上调：上调营收/Capex，N3 GM跨越，Buy TWD2,820（Nomura）
- 来源：Nomura，2026-04-16
- 创建 note: notes/tsmc-1q26-guidance-raise-nomura-2026.md（2026>30%/2027F Capex US$70B/N2量产/A14 2028/CoPoS新方案）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 台积电1Q26业绩点评：GM 66.2%超预期，AI需求持续（Goldman Sachs）
- 来源：Goldman Sachs，2026-04-16
- 创建 note: notes/tsmc-1q26-earnings-review-gs-2026.md（GM 66.2%/2026 >30%YoY/AI CAGR高50s%/CoWoS上调/Capex趋高端，Buy NT$2,750）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 高盛私人软件互联网会议纪要：生成式AI/创作者经济/AV（Goldman Sachs）
- 来源：Goldman Sachs，2026-04-15
- 创建 note: notes/private-software-internet-conf-gs-2026.md（$7.5T基础设施/ElevenLabs $400M ARR/Agent取代SOR/May Mobility DaaS）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 数据中心观察：GPU租赁涨价+内存合约价追踪（J.P. Morgan）
- 来源：J.P. Morgan，2026-04-19
- 创建 note: notes/datacenter-watch-gpu-rental-memory-jpm-2026.md（B200+23.5%/DRAM 2Q26E +421%y/y/NAND +362%y/y）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 生成式AI对全球软件行业5年展望（Bernstein）
- 来源：Bernstein Research，2026-04-14
- 创建 note: notes/genai-global-software-future-bernstein-2026.md（AI不吃软件/IaaS TAM扩大/ERP最防御/MSFT/ORCL/SAP OPerform）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md，原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | 软件护城河IV：AI原生重塑SaaS，CRM/CRWD/GWRE/RBRK受益（Goldman Sachs）
- 来源：Goldman Sachs，2026-04-16
- 创建 note: notes/software-moats-ai-native-gs-2026.md（蒸馏成本2%/推理逼近人力成本/AI原生占白空间/安全修复周期）
- 更新 index.md（Invest/Notes、Sources）
- PDF 转 md：sources/quant-reports/软件护城河再审视：重心转移与AI原生机遇.md
- 原始 PDF 移至 raw-pdf/

## [2026-04-22] ingest | AI重塑汽车业：SDV/E2E/L4渗透率，日本整车受益分析（Bernstein）
- 来源：Bernstein Research，2026-04-15
- 创建 note: notes/ai-auto-sdv-japan-bernstein-2026.md（丰田领先/本田日产落后/L4渗透4%2035E/三大增值路径）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 人工智能技术加速与算力约束投资展望：Citi第四届AI峰会纪要
- 来源：Citi Research，2026-04-17
- 创建 note: notes/citi-ai-summit-tech-invest-outlook-2026.md（Mythos安全担忧/算力约束至2029/Physical AI/GOOGL/AMZN受益）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | AI对利润池影响分析II：全球自动驾驶交通案例研究（Goldman Sachs）
- 来源：Goldman Sachs，2026-04-17
- 创建 note: notes/ai-profit-pools-av-transport-gs-2026.md（Robotaxi 2035全球$415B/AV卡车$560B/Waymo SF 30%/GOOGL/TSLA/UBER受益）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 全球光模块市场：AI驱动800G及以上高速率需求增长（Goldman Sachs）
- 来源：Goldman Sachs，2026-04-17
- 创建 note: notes/global-optical-transceiver-800g-ai-gs-2026.md（TAM $51B/SiPh渗透60-100%/Innolight/TFC/VPEC Buy）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | ASML：强劲AI需求与EUV产能提升，重申买入（Goldman Sachs）
- 来源：Goldman Sachs，2026-04-16
- 创建 note: notes/asml-euv-ai-demand-gs-2026.md（1Q26超预期/指引上调€36-40B/2027年EUV≥80台/BUY PT €1,570）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 苹果F2Q26业绩前瞻：iPhone/Mac/毛利率均超预期（Goldman Sachs）
- 来源：Goldman Sachs，2026-04-20
- 创建 note: notes/apple-f2q26-preview-gs-2026.md（BUY PT $330/iPhone+21%/Mac+12%/GM 49%/大中华+33%）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 苹果F2Q26业绩前瞻：iPhone收入超预期，WWDC与折叠屏（Morgan Stanley）
- 来源：Morgan Stanley，2026-04-20
- 创建 note: notes/apple-f2q26-preview-iphone-wwdc-ms-2026.md（iPhone出货5%超Street/毛利率低150bps/WWDC+折叠屏催化剂/OW PT $315）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 中国互联网AI周报#35：模型密集发布与平台涨价持续（Jefferies）
- 来源：Jefferies China Internet，2026-04-20
- 创建 note: notes/china-internet-ai-weekly-35-jefferies-2026.md（BABA百炼涨价+20%/DeepSeek V4预期/Claude Sonnet 4.6 OpenRouter #1/中美差距2.7%）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 光路交换成为AI网络核心（Nomura）
- 来源：Nomura Global AI Trend Tracker，2026-04
- 创建 note: notes/ocs-ai-network-china-optics-nomura-2026.md（OCS CAGR 58%，InnoLight/TFC受益，四大技术路线，CPO+OCS降耗2.6x）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 大中华区科技硬件：Agentic AI硬件受益者（Morgan Stanley）
- 来源：Morgan Stanley Asia Pacific，2026-04-19
- 创建 note: notes/agentic-ai-hardware-gc-ms-2026.md（ABF缺口扩至15%/2030E，Unimicron/Lotes/Yageo/GCE受益，CPU TAM量化）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 大中华区科技硬件：宏观不确定性与AI硬件前景（Morgan Stanley）
- 来源：Morgan Stanley Asia Pacific，2026-04-16
- 创建 note: notes/greater-china-tech-hardware-macro-ai-ms-2026.md（Wistron/Quanta/FII OW，800VDC/PCB/CPO机遇，消费电子受内存通胀压制）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 大中华区旧存储不对称风险（Morgan Stanley）
- 来源：Morgan Stanley，2026-04-19
- 创建 note: notes/legacy-memory-asymmetric-risk-ms-2026.md（MLC NAND/NOR > DDR4，EMIB-T AP Memory 机遇，Macronix Top Pick）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 大中华半导体：聚焦AI相关芯片（Morgan Stanley）
- 来源：Morgan Stanley Asia Pacific，2026-04-20
- 创建 note: notes/greater-china-semis-ai-chips-ms-2026.md（TSMC/Alchip/Aspeed OW，CoWoS量化，CSP Capex $6850亿，DeepSeek效应）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 大立光：CPO机遇尚远，iPhone+可变光圈支撑短期（Citi）
- 来源：Citi Research，2026-04-15
- 创建 note: notes/largan-cpo-iphone-citi-2026.md（Neutral PT NT$3,060，EPS 上调 23%/24%，CPO 1-2 年内不落地）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 半导体：微处理器走强，但存储仍是首选（Morgan Stanley）
- 来源：Morgan Stanley，2026-04-20
- 创建 note: notes/semis-cpu-memory-play-ms-2026.md（Agentic AI 推动 CPU 增长，但 MU/SNDK 性价比更优；INTC PT 上调 $56，AMD EW PT $255）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-22] ingest | 半导体行业 1Q26 前瞻（J.P. Morgan）
- 来源：J.P. Morgan Semiconductors/Semi Cap Equipment，2026-04-17
- 创建 note: notes/semis-1q26-preview-jpm-2026.md（AI需求持续/HBM供应紧至CY27/WFE 20%+/XPU抢占份额）
- 更新 index.md（Invest/Notes、Sources）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-21] ingest | 日本IT服务业AI时代招聘策略（Goldman Sachs）
- 来源：Goldman Sachs Japan，2026-04-20
- 创建 note: notes/japan-it-services-ai-hiring-strategies-gs-2026.md（BayCurrent扩招/SHIFT缩招/Money Forward AI提效，三条AI适应路径）
- 更新 index.md（Invest/Notes、Sources）
- 交叉验证：SHIFT 软件测试业务受 GenAI 威胁，印证 AI 重塑软件开发格局；与本批次其他 AI 颠覆软件报告形成行业级互证

## [2026-04-21] ingest | Jentech 下一代AI GPU散热器价值量提升（J.P. Morgan）
- 来源：J.P. Morgan，2026-04-20
- 创建 note: notes/jentech-ai-gpu-heat-spreader-jpm-2026.md（OW PT NT$5,300 上调 / NVIDIA+AMD 双驱动 / EPS CAGR ~60%）
- 创建 entity: entities/jentech.md
- 更新 index.md（Invest/Notes、Entities、Sources）
- 交叉验证：TSMC CoWoS 扩产 + AI 服务器出货大增（Dell/Wistron 数据）是散热器需求基础；与 All Ring & GPTC 同为台湾先进封装供应链受益

## [2026-04-21] ingest | Dell & SMCI AI基础设施需求加速（Citi Research）
- 来源：Citi Research，2026-04-20
- 创建 note: notes/dell-smci-ai-infra-citi-2026.md（DELL Buy PT $235 上调 / SMCI Neutral High Risk PT $25 / Citi 服务器模型更新）
- 创建 entity: entities/dell.md
- 创建 entity: entities/supermicro.md
- 更新 index.md（Invest/Notes、Entities、Sources）
- 交叉验证：大五云厂商 Capex $678bn（+69% YoY）呼应 Azure capex 上修；戴尔 AI 机架出货大幅增长印证先进封装需求持续

## [2026-04-21] ingest | Microsoft 3Q26 业绩前瞻（Morgan Stanley）
- 来源：Morgan Stanley，2026-04-20
- 创建 note: notes/microsoft-3q26-preview-copilot-azure-ms-2026.md（Azure 容量约束/Copilot 平台化/Capex 上修，OW PT $650）
- 创建 entity: entities/microsoft.md
- 更新 index.md（Invest/Notes、Entities、Sources）
- 交叉验证：内存涨价（呼应 SEMCO 报告）推高 capex；TSMC/NVDA GPU 供应改善是 Azure 增长前提

## [2026-04-21] ingest | 三星电机 SEMCO MLCC 上行周期（J.P. Morgan）
- 来源：J.P. Morgan，2026-04-21
- 创建 note: notes/samsung-electro-mechanics-mlcc-upcycle-jpm-2026.md（MLCC/基板双升周期，OW PT W840k）
- 更新 index.md
- 交叉验证：AI 服务器 MLCC 需求是本轮涨价主驱动，呼应 AI 基础设施投资扩张逻辑

## [2026-04-21] ingest | All Ring & GPTC 先进封装设备（GS Research）
- 来源：Goldman Sachs，2026-04-21
- 创建 note: notes/all-ring-gptc-advanced-packaging-gs-2026.md（CoWoS/CPO/SoIC 三驱动，双 Buy 上调目标价）
- 更新 index.md
- 交叉验证：TSMC CoWoS 扩产是核心催化剂，与台积电相关报告形成上下游联动

## [2026-04-21] ingest | GS iQIYI World Conference 2026（PDF）
- 来源：Goldman Sachs 研究报告，2026-04-21
- 创建 note: notes/iq-world-conference-2026-gs.md（AI制作革命/组织转型/出海/财务）
- 创建 entity: entities/iqiyi.md
- 更新 index.md（Invest/Notes、Entities、Sources）
- 交叉验证：与 SPOT 前瞻对比，两种不同的流媒体 AI 应对路径（数据壁垒 vs IP 壁垒）
- 文件从 sources/quant-reports/report26m4w3/ 移动至 sources/quant-reports/

## [2026-04-21] ingest | GS SPOT Q1'26 Earnings Preview（PDF）
- 来源：Goldman Sachs 研究报告，2026-04-15
- 创建 note: notes/spot-q1-2026-gs-preview.md（ARPU/成本/AI/估值全拆解）
- 创建 entity: entities/spotify.md
- 更新 index.md（Invest/Notes、Entities、Sources）
- 交叉验证：报告使用 SensorTower + SimilarWeb 另类数据，呼应 quant-data-infra 中另类数据源概念

## [2026-04-20] ingest | 量化第一课：数据从哪来、怎么存？
- 来源：微信公众号文章（用户粘贴）
- 创建 source: quant-data-infra.md
- 创建 concept: quant-data-infra.md（数据来源三层、频率选择、存储分层、关键规范）
- 更新 index.md

## [2026-04-20] init | Wiki 初始化
- 创建目录结构：sources/、entities/、concepts/、notes/
- 建立 SCHEMA.md（四领域：quant / ai / invest / eng）
- 建立 index.md、log.md
- 全新开始，不迁移旧内容
