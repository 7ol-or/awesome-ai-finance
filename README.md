# Awesome AI Finance [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**English** | [한국어](README.ko.md) | [中文](README.zh.md)

> A curated list of practical, AI-powered tools for Finance that do **not** require deep ML model training.

**Focus:** LLMs · AI Agents · Advanced NLP · MCP Servers — ready to use, no data science PhD required.

**✅ Included:** Tools using LLMs, AI Agents, or NLP at their core. MCP servers for financial data/trading. Multi-agent frameworks for finance.  
**❌ Excluded:** Pure vector DBs, RL/DL training frameworks, traditional quant tools without AI, plain stock APIs, papers/courses, repos without a declared open-source license.

> All star counts and last-push dates verified via GitHub API as of **2026-06-29**.

---

## Contents

- [🔌 AI Finance Connectors \& MCP Servers](#-ai-finance-connectors--mcp-servers)
  - [Market Data](#market-data)
  - [Trading Execution](#trading-execution)
  - [Research \& Analysis](#research--analysis)
- [🧠 AI Agent Frameworks \& Platforms](#-ai-agent-frameworks--platforms)
- [📈 AI-Powered Applications](#-ai-powered-applications)
- [👥 Active Communities](#-active-communities)
- [📚 Curated Indexes](#-curated-indexes)

---

## 🔌 AI Finance Connectors & MCP Servers

MCP (Model Context Protocol) servers that plug financial data and trading APIs directly into AI assistants like Claude, Cursor, and VS Code Copilot.

### Market Data

| Project | Description | Stars | Last Push | License |
|---------|-------------|-------|-----------|---------|
| [atilaahmettaner/tradingview-mcp](https://github.com/atilaahmettaner/tradingview-mcp) | 30+ tools giving AI assistants access to TradingView — real-time market data, technical analysis, screeners, and backtesting across stocks, crypto, forex, and futures on global exchanges. | ![Stars](https://img.shields.io/github/stars/atilaahmettaner/tradingview-mcp?style=flat-square) | 2026-06-28 | MIT |
| [dgunning/edgartools](https://github.com/dgunning/edgartools) | Comprehensive SEC EDGAR Python library with 11 MCP tools and 7 prompts — every filing type (10-K, 10-Q, 8-K, S-1), no API key required; 1,800+ Smithery installs. | ![Stars](https://img.shields.io/github/stars/dgunning/edgartools?style=flat-square) | 2026-06-29 | MIT |
| [financial-datasets/mcp-server](https://github.com/financial-datasets/mcp-server) | Structured access to income statements, balance sheets, cash flows, stock prices, and market news via the Financial Datasets API. | ![Stars](https://img.shields.io/github/stars/financial-datasets/mcp-server?style=flat-square) | 2025-06-05 | MIT |
| [guangxiangdebizi/FinanceMCP](https://github.com/guangxiangdebizi/FinanceMCP) | Integrates Tushare (Chinese A-shares, funds, bonds, macro) and Binance (crypto) to give LLMs real-time global financial data. | ![Stars](https://img.shields.io/github/stars/guangxiangdebizi/FinanceMCP?style=flat-square) | 2026-05-26 | MIT |
| [TickDB/tickdb-unified-realtime-marketdata-api](https://github.com/TickDB/tickdb-unified-realtime-marketdata-api) | 13-tool MCP server providing unified real-time and historical market data across Forex, US/HK/CN stocks, and crypto via the TickDB API. | ![Stars](https://img.shields.io/github/stars/TickDB/tickdb-unified-realtime-marketdata-api?style=flat-square) | 2026-06-20 | MIT |
| [massive-com/mcp_massive](https://github.com/massive-com/mcp_massive) | Polygon.io MCP server — professional-grade real-time and historical data for stocks, forex, crypto, and options aggregates. *(Formerly `polygon-io/mcp_polygon`)* | ![Stars](https://img.shields.io/github/stars/massive-com/mcp_massive?style=flat-square) | 2026-06-11 | MIT |
| [Alex2Yang97/yahoo-finance-mcp](https://github.com/Alex2Yang97/yahoo-finance-mcp) | Comprehensive Yahoo Finance data — stock quotes, financials, options chains, and market news — as MCP tools for AI assistants. | ![Stars](https://img.shields.io/github/stars/Alex2Yang97/yahoo-finance-mcp?style=flat-square) | 2026-03-23 | MIT |
| [zwldarren/akshare-one-mcp](https://github.com/zwldarren/akshare-one-mcp) | MCP server wrapping the AKShare API for Chinese stock market data including historical prices, real-time quotes, financial reports, and news. | ![Stars](https://img.shields.io/github/stars/zwldarren/akshare-one-mcp?style=flat-square) | 2026-03-14 | MIT |
| [alphavantage/alpha_vantage_mcp](https://github.com/alphavantage/alpha_vantage_mcp) | **Official** Alpha Vantage MCP server — real-time and historical data for stocks, forex, crypto, options, and ETFs across global markets. | ![Stars](https://img.shields.io/github/stars/alphavantage/alpha_vantage_mcp?style=flat-square) | 2026-06-26 | MIT |
| [imbenrabi/Financial-Modeling-Prep-MCP-Server](https://github.com/imbenrabi/Financial-Modeling-Prep-MCP-Server) | 250+ Financial Modeling Prep API tools covering stock financials, technical indicators, insider trading, SEC filings, earnings, crypto, and forex. | ![Stars](https://img.shields.io/github/stars/imbenrabi/Financial-Modeling-Prep-MCP-Server?style=flat-square) | 2026-06-27 | Apache-2.0 |
| [kukapay/crypto-indicators-mcp](https://github.com/kukapay/crypto-indicators-mcp) | MCP server providing cryptocurrency technical analysis indicators (MACD, RSI, Bollinger Bands) and strategy signals via CCXT for AI trading agents. | ![Stars](https://img.shields.io/github/stars/kukapay/crypto-indicators-mcp?style=flat-square) | 2025-12-06 | MIT |
| [stefanoamorelli/fred-mcp-server](https://github.com/stefanoamorelli/fred-mcp-server) | Federal Reserve Economic Data (FRED) MCP server — gives AI assistants access to 800,000+ macroeconomic time series for market context and macro analysis. | ![Stars](https://img.shields.io/github/stars/stefanoamorelli/fred-mcp-server?style=flat-square) | 2026-05-16 | AGPL-3.0 |

### Trading Execution

| Project | Description | Stars | Last Push | License |
|---------|-------------|-------|-----------|---------|
| [alpacahq/alpaca-mcp-server](https://github.com/alpacahq/alpaca-mcp-server) | **Official** Alpaca MCP server — natural-language trading of US stocks, ETFs, options, and crypto with full OpenAPI coverage via FastMCP. | ![Stars](https://img.shields.io/github/stars/alpacahq/alpaca-mcp-server?style=flat-square) | 2026-06-26 | MIT |
| [krakenfx/kraken-cli](https://github.com/krakenfx/kraken-cli) | **Official** Kraken AI-native CLI with built-in MCP support — natural language access to spot trading, portfolio management, and market data on the Kraken exchange. | ![Stars](https://img.shields.io/github/stars/krakenfx/kraken-cli?style=flat-square) | 2026-04-20 | MIT |
| [ariadng/metatrader-mcp-server](https://github.com/ariadng/metatrader-mcp-server) | MCP bridge connecting AI assistants to MetaTrader 5 — natural-language trade execution, account management, and live position tracking for forex and futures. | ![Stars](https://img.shields.io/github/stars/ariadng/metatrader-mcp-server?style=flat-square) | 2026-03-28 | MIT |
| [mcpdotdirect/evm-mcp-server](https://github.com/mcpdotdirect/evm-mcp-server) | 22-tool MCP server for 60+ EVM-compatible networks (Ethereum, Arbitrum, Base, Optimism, Polygon) — token balances, smart contract interaction, and DeFi operations. | ![Stars](https://img.shields.io/github/stars/mcpdotdirect/evm-mcp-server?style=flat-square) | 2026-06-04 | MIT |
| [okx/agent-trade-kit](https://github.com/okx/agent-trade-kit) | **Official** OKX MCP server enabling AI agents to trade spot, perpetuals, and futures — full order management, market data, and portfolio tracking on OKX. | ![Stars](https://img.shields.io/github/stars/okx/agent-trade-kit?style=flat-square) | 2026-06-25 | MIT |
| [rcontesti/IB_MCP](https://github.com/rcontesti/IB_MCP) | Interactive Brokers TWS/Gateway MCP server — connects AI assistants to the world's largest online broker for live trading, account data, and market access across 150 markets. | ![Stars](https://img.shields.io/github/stars/rcontesti/IB_MCP?style=flat-square) | 2025-10-23 | MIT |
| [QuantConnect/mcp-server](https://github.com/QuantConnect/mcp-server) | **Official** QuantConnect MCP server — lets AI assistants write Python trading strategies, run cloud backtests, and deploy live algorithms on the QuantConnect platform. | ![Stars](https://img.shields.io/github/stars/QuantConnect/mcp-server?style=flat-square) | 2026-05-07 | Apache-2.0 |
| [koreainvestment/open-trading-api](https://github.com/koreainvestment/open-trading-api) | **Official** Korea Investment & Securities Open API — MCP and LLM-integrated SDK (topics: mcp, claude, llm, autotrade) for Korean equity market trading including real-time quotes, order management, and AI-assisted strategy examples. | ![Stars](https://img.shields.io/github/stars/koreainvestment/open-trading-api?style=flat-square) | 2026-06-24 | — |

### Research & Analysis

| Project | Description | Stars | Last Push | License |
|---------|-------------|-------|-----------|---------|
| [mnemox-ai/tradememory-protocol](https://github.com/mnemox-ai/tradememory-protocol) | Open-source memory MCP for AI trading agents — three-layer architecture (L1 raw trade memory, L2 pattern reflection, L3 strategy evolution) enabling agents to learn from past trades. | ![Stars](https://img.shields.io/github/stars/mnemox-ai/tradememory-protocol?style=flat-square) | 2026-06-01 | MIT |
| [wshobson/maverick-mcp](https://github.com/wshobson/maverick-mcp) | Personal stock analysis MCP server — technical indicators, earnings calendars, options flow, insider trades, and sector analysis for AI assistants. | ![Stars](https://img.shields.io/github/stars/wshobson/maverick-mcp?style=flat-square) | 2026-06-20 | MIT |
| [stefanoamorelli/sec-edgar-mcp](https://github.com/stefanoamorelli/sec-edgar-mcp) | MCP server giving AI assistants direct access to SEC EDGAR filings (10-K, 10-Q, 8-K, insider trading) for fundamental research and due diligence. | ![Stars](https://img.shields.io/github/stars/stefanoamorelli/sec-edgar-mcp?style=flat-square) | 2026-06-23 | AGPL-3.0 |
| [hbhqq9/bde-score](https://github.com/hbhqq9/bde-score) | EU AI Act Art.50 compliant multi-market stock analysis MCP server — quantitative scoring (BUY/HOLD/SELL signals) for US, HK, and CN A-shares with x402 payment integration. | ![Stars](https://img.shields.io/github/stars/hbhqq9/bde-score?style=flat-square) | 2026-07-15 | MIT |

---

## 🧠 AI Agent Frameworks & Platforms

Multi-agent and LLM orchestration frameworks built specifically for financial analysis, research, and trading workflows.

| Project | Description | Stars | Last Push | License |
|---------|-------------|-------|-----------|---------|
| [TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents) | Multi-agent LLM trading framework that mirrors a real trading firm — specialized agents for fundamentals, sentiment, technicals, risk, and portfolio management collaborate via LangGraph to reach consensus on trade decisions. | ![Stars](https://img.shields.io/github/stars/TauricResearch/TradingAgents?style=flat-square) | 2026-06-22 | Apache-2.0 |
| [AI4Finance-Foundation/FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) | Open-source financial LLM framework for fine-tuning general models (LLaMA, ChatGLM, Qwen) via LoRA/QLoRA on tasks including sentiment analysis, robo-advising, and trading signal generation. Pre-trained models available on Hugging Face without training. | ![Stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinGPT?style=flat-square) | 2026-06-01 | MIT |
| [AI4Finance-Foundation/FinRobot](https://github.com/AI4Finance-Foundation/FinRobot) | Open-source AI agent platform with a four-layer architecture for financial perception, analysis, and automated equity research report generation using LLMs. | ![Stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinRobot?style=flat-square) | 2026-05-10 | Apache-2.0 |
| [coinbase/agentkit](https://github.com/coinbase/agentkit) | **Official** Coinbase framework that gives any AI agent a crypto wallet — LangChain and CrewAI compatible, covers on-chain token transfers, DeFi protocol interaction, NFT minting, and trade execution across Base and Ethereum. | ![Stars](https://img.shields.io/github/stars/coinbase/agentkit?style=flat-square) | 2026-06-23 | — |

---

## 📈 AI-Powered Applications

Ready-to-use end-user tools: AI investment copilots, autonomous hedge fund simulators, and LLM-driven market analysis platforms.

| Project | Description | Stars | Last Push | License |
|---------|-------------|-------|-----------|---------|
| [virattt/ai-hedge-fund](https://github.com/virattt/ai-hedge-fund) | Multi-agent LLM hedge fund simulator with 18 specialized agents modeled after legendary investors (Buffett, Munger, Burry, Lynch, etc.) that debate and produce trade signals via LangGraph — includes full-stack web UI and CLI. | ![Stars](https://img.shields.io/github/stars/virattt/ai-hedge-fund?style=flat-square) | 2026-06-17 | MIT |
| [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM-powered daily analysis system for A/H/US markets that aggregates multi-source market data and real-time news, generates a buy/hold/sell decision dashboard, and pushes alerts via WeChat, Telegram, Slack, and email. | ![Stars](https://img.shields.io/github/stars/ZhuLinsen/daily_stock_analysis?style=flat-square) | 2026-06-28 | MIT |
| [anthropics/financial-services](https://github.com/anthropics/financial-services) | **Official** Anthropic financial services plugin and agent cookbook — covers DCF valuation, LBO modeling, equity research, wealth management, KYC parsing, GL reconciliation, and bond analytics; installable as Claude plugins. | ![Stars](https://img.shields.io/github/stars/anthropics/financial-services?style=flat-square) | 2026-06-26 | Apache-2.0 |
| [Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal) | Bloomberg Terminal alternative built with AI agents — advanced market analytics, AI-driven investment research, macroeconomic data exploration, and algorithmic trading tools; Python/C++/Qt desktop app. | ![Stars](https://img.shields.io/github/stars/Fincept-Corporation/FinceptTerminal?style=flat-square) | 2026-06-24 | — |
| [virattt/dexter](https://github.com/virattt/dexter) | Autonomous agent for deep financial research — reads SEC filings, earnings transcripts, analyst reports, and news to produce structured investment research; TypeScript, by the creator of ai-hedge-fund. | ![Stars](https://img.shields.io/github/stars/virattt/dexter?style=flat-square) | 2026-06-28 | — |
| [HKUDS/AI-Trader](https://github.com/HKUDS/AI-Trader) | 100% fully-automated agent-native trading system — end-to-end pipeline from market data ingestion to order execution using LLM agents; by the same team as Vibe-Trading. | ![Stars](https://img.shields.io/github/stars/HKUDS/AI-Trader?style=flat-square) | 2026-06-11 | — |
| [UFund-Me/Qbot](https://github.com/UFund-Me/Qbot) | AI-powered quantitative investment research platform with local deployment — integrates LLMs with quant strategy modules for automated signal generation, backtesting, and paper trading. | ![Stars](https://img.shields.io/github/stars/UFund-Me/Qbot?style=flat-square) | 2026-03-11 | MIT |
| [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | Personal trading agent that converts natural language strategy descriptions into backtested, executable trading code — 29 multi-agent presets, 79 finance skills, and export to TradingView Pine Script and MetaTrader 5. | ![Stars](https://img.shields.io/github/stars/HKUDS/Vibe-Trading?style=flat-square) | 2026-06-28 | MIT |
| [The-Swarm-Corporation/AutoHedge](https://github.com/The-Swarm-Corporation/AutoHedge) | Autonomous hedge fund engine using swarm-based multi-agent AI for market analysis, risk management, and trade execution — supports live Solana trading. | ![Stars](https://img.shields.io/github/stars/The-Swarm-Corporation/AutoHedge?style=flat-square) | 2026-05-11 | MIT |
| [marketcalls/openalgo](https://github.com/marketcalls/openalgo) | Open-source algorithmic trading platform with a built-in MCP server for AI agent integration — includes a visual flow strategy builder, real-time P&L tracker, multi-broker support, and Telegram alerts. | ![Stars](https://img.shields.io/github/stars/marketcalls/openalgo?style=flat-square) | 2026-06-25 | AGPL-3.0 |
| [virattt/ai-financial-agent](https://github.com/virattt/ai-financial-agent) | Self-hostable LLM financial research agent that connects to the Financial Datasets API to analyze US equity prices, financials, options activity, and insider trades; by the creator of ai-hedge-fund. | ![Stars](https://img.shields.io/github/stars/virattt/ai-financial-agent?style=flat-square) | 2025-08-19 | — |
| [Lumiwealth/lumibot](https://github.com/Lumiwealth/lumibot) | Backtestable AI trading agent framework for stocks, options, crypto, futures, and forex — built-in AI tools including SEC filings, FRED macro, technical indicators, DuckDB analytics, and Telegram notifications; supports live brokers. | ![Stars](https://img.shields.io/github/stars/Lumiwealth/lumibot?style=flat-square) | 2026-06-25 | GPL-3.0 |
| [DemonDamon/FinnewsHunter](https://github.com/DemonDamon/FinnewsHunter) | Multi-agent financial intelligence platform that crawls and analyzes real-time financial news, synthesizes market sentiment, and delivers structured investment insights via LLM pipelines. | ![Stars](https://img.shields.io/github/stars/DemonDamon/FinnewsHunter?style=flat-square) | 2026-01-13 | Apache-2.0 |
| [51bitquant/ai-hedge-fund-crypto](https://github.com/51bitquant/ai-hedge-fund-crypto) | AI-powered hedge fund framework specialized for cryptocurrency trading, using LLM agents with multi-timeframe LangGraph workflows to analyze markets and execute strategies on crypto exchanges. | ![Stars](https://img.shields.io/github/stars/51bitquant/ai-hedge-fund-crypto?style=flat-square) | 2025-09-05 | MIT |
| [ivebotunac/PrimoAgent](https://github.com/ivebotunac/PrimoAgent) | LangGraph multi-agent stock analysis system with four specialized agents (technical, fundamental, sentiment, portfolio) that produce daily trading insights and next-day price predictions. | ![Stars](https://img.shields.io/github/stars/ivebotunac/PrimoAgent?style=flat-square) | 2026-01-12 | MIT |
| [EthanAlgoX/LLM-TradeBot](https://github.com/EthanAlgoX/LLM-TradeBot) | Multi-agent AI trading system for Binance Futures — uses LLMs to generate, evaluate, and adapt strategies in real-time with a portfolio manager agent coordinating multiple specialist sub-agents. | ![Stars](https://img.shields.io/github/stars/EthanAlgoX/LLM-TradeBot?style=flat-square) | 2026-04-16 | MIT |

---

## 👥 Active Communities

Discord servers and forums where AI + finance practitioners build, share, and collaborate.

| Community | Platform | Members | Focus |
|-----------|----------|---------|-------|
| [LuxAlgo](https://discord.com/servers/luxalgo-641770286638694402) | Discord | 100,000+ | AI-powered TradingView indicator and strategy generation — "Quant" product converts plain English into backtested Pine Script via LLM; official Discord Partner |
| [AI4Finance Foundation](https://github.com/AI4Finance-Foundation) | Discord | 12,000+ | Open-source financial LLMs (FinGPT, FinRobot), financial NLP, and LLM benchmarking — join via the Discord badge in the FinGPT README. |
| [Hummingbot](https://hummingbot.org/community/discord) | Discord | Large | Algorithmic trading bot development, market making, exchange connectors, and AI-assisted strategy building; Foundation-operated with weekly podcast |
| [LLMQuant](https://llmquant.com) | Discord + GitHub | Invite-only | LLMs for quantitative research — AI agents for investment research, open-source quant tools, and MCP-integrated market data; apply via the website |

---

## 📚 Curated Indexes

High-signal aggregators for discovering more AI finance tools:

| Project | Description | Stars |
|---------|-------------|-------|
| [BlockRunAI/awesome-finance-mcp](https://github.com/BlockRunAI/awesome-finance-mcp) | Curated list of MCP servers for AI finance agents — covers Alpaca, Financial Datasets, Alpha Vantage, QuantConnect, FRED, and specialist quant tools. | ![Stars](https://img.shields.io/github/stars/BlockRunAI/awesome-finance-mcp?style=flat-square) |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | Comprehensive index of AI trading agents, MCP servers, Claude skills, and benchmarks across equities, crypto, DeFi, and prediction markets. | ![Stars](https://img.shields.io/github/stars/LLMQuant/awesome-trading-agents?style=flat-square) |
| [georgezouq/awesome-ai-in-finance](https://github.com/georgezouq/awesome-ai-in-finance) | Broad index of LLM + AI tools for financial markets including agents, MCP servers, quant infrastructure, and DeFi tools. | ![Stars](https://img.shields.io/github/stars/georgezouq/awesome-ai-in-finance?style=flat-square) |

---

## Contributing

Please read [contributing.md](contributing.md) before opening a pull request.

---

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
