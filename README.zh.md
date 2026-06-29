# Awesome AI Finance [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[English](README.md) | [한국어](README.ko.md) | **中文**

> 无需深度学习模型训练即可直接使用的实用 AI 金融工具精选列表

**专注领域：** LLM · AI 智能体 · 高级 NLP · MCP 服务器 — 开箱即用，无需数据科学博士学位。

**✅ 收录标准：** 以 LLM、AI 智能体或 NLP 为核心功能的工具。用于金融数据/交易的 MCP 服务器。面向金融领域的多智能体框架。  
**❌ 排除标准：** 纯向量数据库、RL/DL 训练框架、无 AI 的传统量化工具、普通股票 API、论文/课程、未声明开源许可证的仓库。

> 所有 Star 数量和最后推送日期均已通过 GitHub API 验证，数据截止 **2026-06-29**。

---

## 目录

- [🔌 AI 金融连接器 \& MCP 服务器](#-ai-金融连接器--mcp-服务器)
  - [市场数据](#市场数据)
  - [交易执行](#交易执行)
  - [研究与分析](#研究与分析)
- [🧠 AI 智能体框架 \& 平台](#-ai-智能体框架--平台)
- [📈 AI 驱动的应用程序](#-ai-驱动的应用程序)
- [👥 活跃社区](#-活跃社区)
- [📚 精选索引](#-精选索引)

---

## 🔌 AI 金融连接器 & MCP 服务器

MCP（模型上下文协议）服务器，可将金融数据和交易 API 直接接入 Claude、Cursor、VS Code Copilot 等 AI 助手。

### 市场数据

| 项目 | 描述 | Stars | 最近推送 | 许可证 |
|------|------|-------|----------|--------|
| [atilaahmettaner/tradingview-mcp](https://github.com/atilaahmettaner/tradingview-mcp) | 提供 30+ 工具，让 AI 助手访问 TradingView —— 覆盖全球交易所的股票、加密货币、外汇和期货的实时行情、技术分析、选股筛选器和回测功能。 | ![Stars](https://img.shields.io/github/stars/atilaahmettaner/tradingview-mcp?style=flat-square) | 2026-06-28 | MIT |
| [dgunning/edgartools](https://github.com/dgunning/edgartools) | 全面的 SEC EDGAR Python 库，提供 11 个 MCP 工具和 7 个提示词 —— 支持所有申报类型（10-K、10-Q、8-K、S-1），无需 API 密钥；Smithery 安装量超 1,800 次。 | ![Stars](https://img.shields.io/github/stars/dgunning/edgartools?style=flat-square) | 2026-06-29 | MIT |
| [financial-datasets/mcp-server](https://github.com/financial-datasets/mcp-server) | 通过 Financial Datasets API 结构化访问利润表、资产负债表、现金流量表、股票价格和市场新闻。 | ![Stars](https://img.shields.io/github/stars/financial-datasets/mcp-server?style=flat-square) | 2025-06-05 | MIT |
| [guangxiangdebizi/FinanceMCP](https://github.com/guangxiangdebizi/FinanceMCP) | 整合 Tushare（A 股、基金、债券、宏观）和 Binance（加密货币），为 LLM 提供实时全球金融数据。 | ![Stars](https://img.shields.io/github/stars/guangxiangdebizi/FinanceMCP?style=flat-square) | 2026-05-26 | MIT |
| [TickDB/tickdb-unified-realtime-marketdata-api](https://github.com/TickDB/tickdb-unified-realtime-marketdata-api) | 提供 13 个工具的 MCP 服务器，通过 TickDB API 统一访问外汇、美港中股票和加密货币的实时及历史行情数据。 | ![Stars](https://img.shields.io/github/stars/TickDB/tickdb-unified-realtime-marketdata-api?style=flat-square) | 2026-06-20 | MIT |
| [massive-com/mcp_massive](https://github.com/massive-com/mcp_massive) | Polygon.io MCP 服务器 —— 专业级股票、外汇、加密货币和期权聚合数据的实时及历史行情。*(原 `polygon-io/mcp_polygon`)* | ![Stars](https://img.shields.io/github/stars/massive-com/mcp_massive?style=flat-square) | 2026-06-11 | MIT |
| [Alex2Yang97/yahoo-finance-mcp](https://github.com/Alex2Yang97/yahoo-finance-mcp) | 以 MCP 工具形式为 AI 助手提供完整的 Yahoo Finance 数据 —— 股票报价、财务数据、期权链和市场新闻。 | ![Stars](https://img.shields.io/github/stars/Alex2Yang97/yahoo-finance-mcp?style=flat-square) | 2026-03-23 | MIT |
| [zwldarren/akshare-one-mcp](https://github.com/zwldarren/akshare-one-mcp) | 封装 AKShare API 的 MCP 服务器，提供 A 股历史价格、实时行情、财务报告和新闻数据。 | ![Stars](https://img.shields.io/github/stars/zwldarren/akshare-one-mcp?style=flat-square) | 2026-03-14 | MIT |
| [alphavantage/alpha_vantage_mcp](https://github.com/alphavantage/alpha_vantage_mcp) | **官方** Alpha Vantage MCP 服务器 —— 覆盖全球市场的股票、外汇、加密货币、期权和 ETF 实时及历史数据。 | ![Stars](https://img.shields.io/github/stars/alphavantage/alpha_vantage_mcp?style=flat-square) | 2026-06-26 | MIT |
| [imbenrabi/Financial-Modeling-Prep-MCP-Server](https://github.com/imbenrabi/Financial-Modeling-Prep-MCP-Server) | 250+ Financial Modeling Prep API 工具，涵盖股票财务、技术指标、内幕交易、SEC 申报、财报、加密货币和外汇。 | ![Stars](https://img.shields.io/github/stars/imbenrabi/Financial-Modeling-Prep-MCP-Server?style=flat-square) | 2026-06-27 | Apache-2.0 |
| [kukapay/crypto-indicators-mcp](https://github.com/kukapay/crypto-indicators-mcp) | 通过 CCXT 为 AI 交易智能体提供加密货币技术分析指标（MACD、RSI、布林带）和策略信号的 MCP 服务器。 | ![Stars](https://img.shields.io/github/stars/kukapay/crypto-indicators-mcp?style=flat-square) | 2025-12-06 | MIT |
| [stefanoamorelli/fred-mcp-server](https://github.com/stefanoamorelli/fred-mcp-server) | 美联储经济数据（FRED）MCP 服务器 —— 让 AI 助手访问 80 万+ 宏观经济时间序列数据，用于市场背景和宏观分析。 | ![Stars](https://img.shields.io/github/stars/stefanoamorelli/fred-mcp-server?style=flat-square) | 2026-05-16 | AGPL-3.0 |

### 交易执行

| 项目 | 描述 | Stars | 最近推送 | 许可证 |
|------|------|-------|----------|--------|
| [alpacahq/alpaca-mcp-server](https://github.com/alpacahq/alpaca-mcp-server) | **官方** Alpaca MCP 服务器 —— 通过 FastMCP 以自然语言交易美股、ETF、期权和加密货币，完整覆盖 OpenAPI。 | ![Stars](https://img.shields.io/github/stars/alpacahq/alpaca-mcp-server?style=flat-square) | 2026-06-26 | MIT |
| [krakenfx/kraken-cli](https://github.com/krakenfx/kraken-cli) | **官方** Kraken AI 原生 CLI，内置 MCP 支持 —— 以自然语言访问 Kraken 交易所的现货交易、投资组合管理和行情数据。 | ![Stars](https://img.shields.io/github/stars/krakenfx/kraken-cli?style=flat-square) | 2026-04-20 | MIT |
| [ariadng/metatrader-mcp-server](https://github.com/ariadng/metatrader-mcp-server) | 将 AI 助手连接到 MetaTrader 5 的 MCP 桥接器 —— 支持外汇和期货的自然语言下单、账户管理和实时持仓追踪。 | ![Stars](https://img.shields.io/github/stars/ariadng/metatrader-mcp-server?style=flat-square) | 2026-03-28 | MIT |
| [mcpdotdirect/evm-mcp-server](https://github.com/mcpdotdirect/evm-mcp-server) | 覆盖 60+ EVM 兼容网络（Ethereum、Arbitrum、Base、Optimism、Polygon）的 22 工具 MCP 服务器 —— 代币余额、智能合约交互和 DeFi 操作。 | ![Stars](https://img.shields.io/github/stars/mcpdotdirect/evm-mcp-server?style=flat-square) | 2026-06-04 | MIT |
| [okx/agent-trade-kit](https://github.com/okx/agent-trade-kit) | **官方** OKX MCP 服务器，让 AI 智能体交易现货、永续合约和期货 —— 完整的订单管理、行情数据和 OKX 投资组合追踪。 | ![Stars](https://img.shields.io/github/stars/okx/agent-trade-kit?style=flat-square) | 2026-06-25 | MIT |
| [rcontesti/IB_MCP](https://github.com/rcontesti/IB_MCP) | 盈透证券 TWS/Gateway MCP 服务器 —— 将 AI 助手连接至全球最大在线券商，覆盖 150 个市场的实盘交易、账户数据和行情访问。 | ![Stars](https://img.shields.io/github/stars/rcontesti/IB_MCP?style=flat-square) | 2025-10-23 | MIT |
| [QuantConnect/mcp-server](https://github.com/QuantConnect/mcp-server) | **官方** QuantConnect MCP 服务器 —— 让 AI 助手在 QuantConnect 平台编写 Python 交易策略、运行云端回测并部署实盘算法。 | ![Stars](https://img.shields.io/github/stars/QuantConnect/mcp-server?style=flat-square) | 2026-05-07 | Apache-2.0 |
| [koreainvestment/open-trading-api](https://github.com/koreainvestment/open-trading-api) | **官方** 韩国投资证券 Open API —— 集成 MCP 和 LLM 的 SDK（标签：mcp、claude、llm、autotrade），支持韩国股票市场实时行情、订单管理和 AI 辅助策略示例。 | ![Stars](https://img.shields.io/github/stars/koreainvestment/open-trading-api?style=flat-square) | 2026-06-24 | — |

### 研究与分析

| 项目 | 描述 | Stars | 最近推送 | 许可证 |
|------|------|-------|----------|--------|
| [mnemox-ai/tradememory-protocol](https://github.com/mnemox-ai/tradememory-protocol) | 面向 AI 交易智能体的开源记忆 MCP —— 三层架构（L1 原始交易记忆、L2 模式反思、L3 策略演化），让智能体从历史交易中持续学习。 | ![Stars](https://img.shields.io/github/stars/mnemox-ai/tradememory-protocol?style=flat-square) | 2026-06-01 | MIT |
| [wshobson/maverick-mcp](https://github.com/wshobson/maverick-mcp) | 个人股票分析 MCP 服务器 —— 为 AI 助手提供技术指标、财报日历、期权流向、内幕交易和行业分析。 | ![Stars](https://img.shields.io/github/stars/wshobson/maverick-mcp?style=flat-square) | 2026-06-20 | MIT |
| [stefanoamorelli/sec-edgar-mcp](https://github.com/stefanoamorelli/sec-edgar-mcp) | 让 AI 助手直接访问 SEC EDGAR 申报文件（10-K、10-Q、8-K、内幕交易）的 MCP 服务器，用于基本面研究和尽职调查。 | ![Stars](https://img.shields.io/github/stars/stefanoamorelli/sec-edgar-mcp?style=flat-square) | 2026-06-23 | AGPL-3.0 |

---

## 🧠 AI 智能体框架 & 平台

专为金融分析、研究和交易工作流构建的多智能体与 LLM 编排框架。

| 项目 | 描述 | Stars | 最近推送 | 许可证 |
|------|------|-------|----------|--------|
| [TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents) | 模拟真实交易公司的多智能体 LLM 交易框架 —— 基本面、情绪、技术、风险和投资组合专项智能体通过 LangGraph 协作，对交易决策达成共识。 | ![Stars](https://img.shields.io/github/stars/TauricResearch/TradingAgents?style=flat-square) | 2026-06-22 | Apache-2.0 |
| [AI4Finance-Foundation/FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) | 开源金融 LLM 框架，通过 LoRA/QLoRA 微调通用模型（LLaMA、ChatGLM、Qwen），用于情感分析、智能投顾和交易信号生成；HuggingFace 提供预训练模型，无需自行训练。 | ![Stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinGPT?style=flat-square) | 2026-06-01 | MIT |
| [AI4Finance-Foundation/FinRobot](https://github.com/AI4Finance-Foundation/FinRobot) | 开源 AI 智能体平台，四层架构设计，支持金融感知、分析和使用 LLM 自动生成股票研究报告。 | ![Stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinRobot?style=flat-square) | 2026-05-10 | Apache-2.0 |
| [coinbase/agentkit](https://github.com/coinbase/agentkit) | **官方** Coinbase 框架，为任意 AI 智能体提供加密钱包 —— 兼容 LangChain 和 CrewAI，支持链上代币转账、DeFi 协议交互、NFT 铸造以及 Base 和 Ethereum 上的交易执行。 | ![Stars](https://img.shields.io/github/stars/coinbase/agentkit?style=flat-square) | 2026-06-23 | — |

---

## 📈 AI 驱动的应用程序

开箱即用的终端工具：AI 投资助手、自主对冲基金模拟器和 LLM 驱动的市场分析平台。

| 项目 | 描述 | Stars | 最近推送 | 许可证 |
|------|------|-------|----------|--------|
| [virattt/ai-hedge-fund](https://github.com/virattt/ai-hedge-fund) | 多智能体 LLM 对冲基金模拟器，18 个专项智能体模拟传奇投资者（巴菲特、芒格、伯里、林奇等），通过 LangGraph 辩论并产生交易信号 —— 含完整 Web UI 和 CLI。 | ![Stars](https://img.shields.io/github/stars/virattt/ai-hedge-fund?style=flat-square) | 2026-06-17 | MIT |
| [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM 驱动的 A/H/美股每日分析系统，聚合多源行情数据和实时新闻，生成买入/持有/卖出决策看板，并通过微信、Telegram、Slack 和邮件推送提醒。 | ![Stars](https://img.shields.io/github/stars/ZhuLinsen/daily_stock_analysis?style=flat-square) | 2026-06-28 | MIT |
| [anthropics/financial-services](https://github.com/anthropics/financial-services) | **官方** Anthropic 金融服务插件与智能体示例集 —— 涵盖 DCF 估值、LBO 建模、股权研究、财富管理、KYC 解析、总账对账和债券分析，可作为 Claude 插件安装。 | ![Stars](https://img.shields.io/github/stars/anthropics/financial-services?style=flat-square) | 2026-06-26 | Apache-2.0 |
| [Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal) | Bloomberg 终端替代品，内置 AI 智能体 —— 高级市场分析、AI 驱动的投资研究、宏观经济数据探索和量化交易工具；Python/C++/Qt 桌面应用。 | ![Stars](https://img.shields.io/github/stars/Fincept-Corporation/FinceptTerminal?style=flat-square) | 2026-06-24 | — |
| [virattt/dexter](https://github.com/virattt/dexter) | 深度金融研究自主智能体 —— 读取 SEC 申报、财报转录、分析师报告和新闻，生成结构化投资研究；TypeScript，由 ai-hedge-fund 创作者开发。 | ![Stars](https://img.shields.io/github/stars/virattt/dexter?style=flat-square) | 2026-06-28 | — |
| [HKUDS/AI-Trader](https://github.com/HKUDS/AI-Trader) | 100% 全自动智能体原生交易系统 —— 从行情数据摄取到订单执行的端到端 LLM 智能体流水线；与 Vibe-Trading 同一团队出品。 | ![Stars](https://img.shields.io/github/stars/HKUDS/AI-Trader?style=flat-square) | 2026-06-11 | — |
| [UFund-Me/Qbot](https://github.com/UFund-Me/Qbot) | 支持本地部署的 AI 量化投资研究平台 —— 将 LLM 与量化策略模块集成，实现自动化信号生成、回测和模拟交易。 | ![Stars](https://img.shields.io/github/stars/UFund-Me/Qbot?style=flat-square) | 2026-03-11 | MIT |
| [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 将自然语言策略描述转化为可回测、可执行交易代码的个人交易智能体 —— 29 种多智能体预设、79 个金融技能，支持导出 TradingView Pine Script 和 MetaTrader 5。 | ![Stars](https://img.shields.io/github/stars/HKUDS/Vibe-Trading?style=flat-square) | 2026-06-28 | MIT |
| [The-Swarm-Corporation/AutoHedge](https://github.com/The-Swarm-Corporation/AutoHedge) | 基于群体多智能体 AI 的自主对冲基金引擎，用于市场分析、风险管理和交易执行 —— 支持 Solana 实盘交易。 | ![Stars](https://img.shields.io/github/stars/The-Swarm-Corporation/AutoHedge?style=flat-square) | 2026-05-11 | MIT |
| [marketcalls/openalgo](https://github.com/marketcalls/openalgo) | 内置 MCP 服务器的开源量化交易平台 —— 包含可视化流程策略构建器、实时盈亏追踪器、多券商支持和 Telegram 提醒。 | ![Stars](https://img.shields.io/github/stars/marketcalls/openalgo?style=flat-square) | 2026-06-25 | AGPL-3.0 |
| [virattt/ai-financial-agent](https://github.com/virattt/ai-financial-agent) | 可自托管的 LLM 金融研究智能体，连接 Financial Datasets API 分析美股价格、财务数据、期权活动和内幕交易；由 ai-hedge-fund 创作者开发。 | ![Stars](https://img.shields.io/github/stars/virattt/ai-financial-agent?style=flat-square) | 2025-08-19 | — |
| [Lumiwealth/lumibot](https://github.com/Lumiwealth/lumibot) | 可回测的 AI 交易智能体框架，支持股票、期权、加密货币、期货和外汇 —— 内置 SEC 申报、FRED 宏观、技术指标、DuckDB 分析和 Telegram 通知等 AI 工具，支持实盘券商。 | ![Stars](https://img.shields.io/github/stars/Lumiwealth/lumibot?style=flat-square) | 2026-06-25 | GPL-3.0 |
| [DemonDamon/FinnewsHunter](https://github.com/DemonDamon/FinnewsHunter) | 多智能体金融情报平台，通过 LLM 流水线抓取和分析实时金融新闻、综合市场情绪并输出结构化投资洞察。 | ![Stars](https://img.shields.io/github/stars/DemonDamon/FinnewsHunter?style=flat-square) | 2026-01-13 | Apache-2.0 |
| [51bitquant/ai-hedge-fund-crypto](https://github.com/51bitquant/ai-hedge-fund-crypto) | 专注加密货币交易的 AI 对冲基金框架，使用 LLM 智能体和多时间框架 LangGraph 工作流分析市场并在加密交易所执行策略。 | ![Stars](https://img.shields.io/github/stars/51bitquant/ai-hedge-fund-crypto?style=flat-square) | 2025-09-05 | MIT |
| [ivebotunac/PrimoAgent](https://github.com/ivebotunac/PrimoAgent) | LangGraph 多智能体股票分析系统，四个专项智能体（技术、基本面、情绪、投资组合）每日生成交易洞察和次日价格预测。 | ![Stars](https://img.shields.io/github/stars/ivebotunac/PrimoAgent?style=flat-square) | 2026-01-12 | MIT |
| [EthanAlgoX/LLM-TradeBot](https://github.com/EthanAlgoX/LLM-TradeBot) | 面向 Binance 期货的多智能体 AI 交易系统 —— 使用 LLM 实时生成、评估和调整策略，由投资组合管理智能体协调多个专项子智能体。 | ![Stars](https://img.shields.io/github/stars/EthanAlgoX/LLM-TradeBot?style=flat-square) | 2026-04-16 | MIT |

---

## 👥 活跃社区

AI + 金融从业者共同构建、分享和协作的 Discord 服务器与论坛。

| 社区 | 平台 | 成员数 | 专注领域 |
|------|------|--------|---------|
| [LuxAlgo](https://discord.com/servers/luxalgo-641770286638694402) | Discord | 100,000+ | AI 驱动的 TradingView 指标和策略生成 —— "Quant" 产品通过 LLM 将纯文字描述转化为经回测的 Pine Script；Discord 官方合作伙伴 |
| [AI4Finance Foundation](https://github.com/AI4Finance-Foundation/FinGPT) | Discord | 12,000+ | 开源金融 LLM（FinGPT、FinRobot）、金融 NLP 和 LLM 基准测试 —— 通过 FinGPT README 中的徽章加入 |
| [Hummingbot](https://hummingbot.org/community/discord) | Discord | 较大 | 量化交易机器人开发、做市、交易所连接器和 AI 辅助策略构建；基金会运营，每周播客 |
| [LLMQuant](https://llmquant.com) | Discord + GitHub | 邀请制 | LLM 量化研究 —— 投资研究 AI 智能体、开源量化工具和 MCP 集成行情数据；通过官网申请加入 |

---

## 📚 精选索引

发现更多 AI 金融工具的高质量聚合资源：

| 项目 | 描述 | Stars |
|------|------|-------|
| [BlockRunAI/awesome-finance-mcp](https://github.com/BlockRunAI/awesome-finance-mcp) | AI 金融智能体 MCP 服务器精选列表 —— 涵盖 Alpaca、Financial Datasets、Alpha Vantage、QuantConnect、FRED 和专业量化工具。 | ![Stars](https://img.shields.io/github/stars/BlockRunAI/awesome-finance-mcp?style=flat-square) |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | AI 交易智能体、MCP 服务器、Claude 技能和跨股票、加密货币、DeFi、预测市场基准的综合索引。 | ![Stars](https://img.shields.io/github/stars/LLMQuant/awesome-trading-agents?style=flat-square) |
| [georgezouq/awesome-ai-in-finance](https://github.com/georgezouq/awesome-ai-in-finance) | 金融市场 LLM + AI 工具广泛索引，包含智能体、MCP 服务器、量化基础设施和 DeFi 工具。 | ![Stars](https://img.shields.io/github/stars/georgezouq/awesome-ai-in-finance?style=flat-square) |

---

## 贡献指南

欢迎提交 PR。提交前请确认：

1. **AI 优先：** 工具以 LLM、AI 智能体或高级 NLP 为核心功能，而非附带提及
2. **范围内：** 金融 = 交易 / 投资 / 投资组合管理 / 市场数据 / 量化研究。**范围外：** 内容变现工具、社交媒体自动化、通用"用 AI 赚钱"工具
3. **活跃：** GitHub `pushed_at` 在 12 个月内，或知名基金会项目
4. **无重复：** 若存在类似工具，新条目须有明显不同的用途或显著更多的 Star 数

许可证列：已声明时显示 SPDX 标识符（如 `MIT`、`Apache-2.0`）；GitHub 报告无许可证或无法识别时显示 `—`。使用 `—` 的仓库请自行判断风险。

每行一个条目：名称、聚焦 AI/LLM 功能的一句话描述、Stars 徽章、最近推送日期、许可证。

---

## 许可证

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
