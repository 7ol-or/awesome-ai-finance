[English](README.md) | **한국어** | [中文](README.zh.md)

# Awesome AI Finance [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 심층 ML 모델 학습이 **필요 없는** 실용적인 AI 금융 도구 큐레이션 목록.

**초점:** LLM · AI 에이전트 · 고급 NLP · MCP 서버 — 데이터 과학 박사 학위 없이도 바로 사용 가능.

**✅ 포함 기준:** LLM, AI 에이전트, 또는 NLP를 핵심으로 사용하는 도구. 금융 데이터/트레이딩용 MCP 서버. 금융 특화 멀티에이전트 프레임워크.  
**❌ 제외 기준:** 순수 벡터 DB, RL/DL 학습 프레임워크, AI 없는 전통적 퀀트 도구, 단순 주식 API, 논문/강의, 오픈소스 라이선스 미선언 레포.

> 모든 스타 수와 최근 푸시 날짜는 **2026-06-29** 기준 GitHub API로 직접 검증됨.

---

## 목차

- [🔌 AI 금융 커넥터 \& MCP 서버](#-ai-금융-커넥터--mcp-서버)
  - [시장 데이터](#시장-데이터)
  - [트레이딩 실행](#트레이딩-실행)
  - [리서치 \& 분석](#리서치--분석)
- [🧠 AI 에이전트 프레임워크 \& 플랫폼](#-ai-에이전트-프레임워크--플랫폼)
- [📈 AI 기반 애플리케이션](#-ai-기반-애플리케이션)
- [👥 활성 커뮤니티](#-활성-커뮤니티)
- [📚 큐레이션 인덱스](#-큐레이션-인덱스)

---

## 🔌 AI 금융 커넥터 & MCP 서버

Claude, Cursor, VS Code Copilot 같은 AI 어시스턴트에 금융 데이터와 트레이딩 API를 직접 연결하는 MCP(Model Context Protocol) 서버.

### 시장 데이터

| 프로젝트 | 설명 | 스타 | 최근 푸시 | 라이선스 |
|---------|------|------|----------|---------|
| [atilaahmettaner/tradingview-mcp](https://github.com/atilaahmettaner/tradingview-mcp) | AI 어시스턴트에 TradingView를 연결하는 30개 이상의 도구 — 글로벌 거래소의 주식·암호화폐·외환·선물에 대한 실시간 시장 데이터, 기술 분석, 스크리너, 백테스팅 제공. | ![Stars](https://img.shields.io/github/stars/atilaahmettaner/tradingview-mcp?style=flat-square) | 2026-06-28 | MIT |
| [dgunning/edgartools](https://github.com/dgunning/edgartools) | 11개 MCP 도구와 7개 프롬프트를 갖춘 종합 SEC EDGAR Python 라이브러리 — 모든 공시 유형(10-K, 10-Q, 8-K, S-1) 지원, API 키 불필요; Smithery 설치 1,800회 이상. | ![Stars](https://img.shields.io/github/stars/dgunning/edgartools?style=flat-square) | 2026-06-29 | MIT |
| [financial-datasets/mcp-server](https://github.com/financial-datasets/mcp-server) | Financial Datasets API를 통해 손익계산서, 대차대조표, 현금흐름표, 주가, 시장 뉴스에 구조화된 방식으로 접근. | ![Stars](https://img.shields.io/github/stars/financial-datasets/mcp-server?style=flat-square) | 2025-06-05 | MIT |
| [guangxiangdebizi/FinanceMCP](https://github.com/guangxiangdebizi/FinanceMCP) | Tushare(중국 A주·펀드·채권·거시경제)와 Binance(암호화폐)를 통합하여 LLM에 전 세계 실시간 금융 데이터 제공. | ![Stars](https://img.shields.io/github/stars/guangxiangdebizi/FinanceMCP?style=flat-square) | 2026-05-26 | MIT |
| [TickDB/tickdb-unified-realtime-marketdata-api](https://github.com/TickDB/tickdb-unified-realtime-marketdata-api) | TickDB API를 통해 외환·미국/홍콩/중국 주식·암호화폐의 실시간 및 과거 시장 데이터를 통합 제공하는 13개 도구 MCP 서버. | ![Stars](https://img.shields.io/github/stars/TickDB/tickdb-unified-realtime-marketdata-api?style=flat-square) | 2026-06-20 | MIT |
| [massive-com/mcp_massive](https://github.com/massive-com/mcp_massive) | Polygon.io MCP 서버 — 주식·외환·암호화폐·옵션 집계 데이터를 위한 전문가급 실시간 및 과거 데이터. *(구 `polygon-io/mcp_polygon`)* | ![Stars](https://img.shields.io/github/stars/massive-com/mcp_massive?style=flat-square) | 2026-06-11 | MIT |
| [Alex2Yang97/yahoo-finance-mcp](https://github.com/Alex2Yang97/yahoo-finance-mcp) | AI 어시스턴트를 위한 MCP 도구로 Yahoo Finance의 주식 시세·재무제표·옵션 체인·시장 뉴스를 종합 제공. | ![Stars](https://img.shields.io/github/stars/Alex2Yang97/yahoo-finance-mcp?style=flat-square) | 2026-03-23 | MIT |
| [zwldarren/akshare-one-mcp](https://github.com/zwldarren/akshare-one-mcp) | 중국 주식 시장 데이터(과거 주가, 실시간 시세, 재무제표, 뉴스)를 위한 AKShare API 래핑 MCP 서버. | ![Stars](https://img.shields.io/github/stars/zwldarren/akshare-one-mcp?style=flat-square) | 2026-03-14 | MIT |
| [alphavantage/alpha_vantage_mcp](https://github.com/alphavantage/alpha_vantage_mcp) | **공식** Alpha Vantage MCP 서버 — 글로벌 시장의 주식·외환·암호화폐·옵션·ETF 실시간 및 과거 데이터 제공. | ![Stars](https://img.shields.io/github/stars/alphavantage/alpha_vantage_mcp?style=flat-square) | 2026-06-26 | MIT |
| [imbenrabi/Financial-Modeling-Prep-MCP-Server](https://github.com/imbenrabi/Financial-Modeling-Prep-MCP-Server) | 주식 재무제표·기술 지표·내부자 거래·SEC 공시·실적·암호화폐·외환을 아우르는 250개 이상의 Financial Modeling Prep API 도구. | ![Stars](https://img.shields.io/github/stars/imbenrabi/Financial-Modeling-Prep-MCP-Server?style=flat-square) | 2026-06-27 | Apache-2.0 |
| [kukapay/crypto-indicators-mcp](https://github.com/kukapay/crypto-indicators-mcp) | AI 트레이딩 에이전트를 위해 CCXT를 통해 암호화폐 기술 분석 지표(MACD, RSI, 볼린저 밴드)와 전략 신호를 제공하는 MCP 서버. | ![Stars](https://img.shields.io/github/stars/kukapay/crypto-indicators-mcp?style=flat-square) | 2025-12-06 | MIT |
| [stefanoamorelli/fred-mcp-server](https://github.com/stefanoamorelli/fred-mcp-server) | 연방준비제도 경제 데이터(FRED) MCP 서버 — AI 어시스턴트에게 80만 개 이상의 거시경제 시계열 데이터를 제공하여 시장 컨텍스트 및 거시 분석에 활용. | ![Stars](https://img.shields.io/github/stars/stefanoamorelli/fred-mcp-server?style=flat-square) | 2026-05-16 | AGPL-3.0 |

### 트레이딩 실행

| 프로젝트 | 설명 | 스타 | 최근 푸시 | 라이선스 |
|---------|------|------|----------|---------|
| [alpacahq/alpaca-mcp-server](https://github.com/alpacahq/alpaca-mcp-server) | **공식** Alpaca MCP 서버 — FastMCP를 통해 전체 OpenAPI를 커버하며 미국 주식·ETF·옵션·암호화폐를 자연어로 트레이딩. | ![Stars](https://img.shields.io/github/stars/alpacahq/alpaca-mcp-server?style=flat-square) | 2026-06-26 | MIT |
| [krakenfx/kraken-cli](https://github.com/krakenfx/kraken-cli) | **공식** Kraken AI 네이티브 CLI(MCP 내장) — Kraken 거래소에서 현물 트레이딩, 포트폴리오 관리, 시장 데이터에 자연어로 접근. | ![Stars](https://img.shields.io/github/stars/krakenfx/kraken-cli?style=flat-square) | 2026-04-20 | MIT |
| [ariadng/metatrader-mcp-server](https://github.com/ariadng/metatrader-mcp-server) | AI 어시스턴트를 MetaTrader 5에 연결하는 MCP 브릿지 — 외환·선물의 자연어 주문 실행, 계좌 관리, 실시간 포지션 추적. | ![Stars](https://img.shields.io/github/stars/ariadng/metatrader-mcp-server?style=flat-square) | 2026-03-28 | MIT |
| [mcpdotdirect/evm-mcp-server](https://github.com/mcpdotdirect/evm-mcp-server) | 60개 이상의 EVM 호환 네트워크(Ethereum, Arbitrum, Base, Optimism, Polygon)를 위한 22개 도구 MCP 서버 — 토큰 잔액, 스마트 컨트랙트 상호작용, DeFi 운용. | ![Stars](https://img.shields.io/github/stars/mcpdotdirect/evm-mcp-server?style=flat-square) | 2026-06-04 | MIT |
| [okx/agent-trade-kit](https://github.com/okx/agent-trade-kit) | **공식** OKX MCP 서버 — AI 에이전트가 OKX에서 현물·무기한·선물 거래 가능; 전체 주문 관리, 시장 데이터, 포트폴리오 추적 지원. | ![Stars](https://img.shields.io/github/stars/okx/agent-trade-kit?style=flat-square) | 2026-06-25 | MIT |
| [rcontesti/IB_MCP](https://github.com/rcontesti/IB_MCP) | Interactive Brokers TWS/Gateway MCP 서버 — AI 어시스턴트를 세계 최대 온라인 브로커에 연결하여 150개 시장에서 실시간 트레이딩, 계좌 데이터, 시장 접근 지원. | ![Stars](https://img.shields.io/github/stars/rcontesti/IB_MCP?style=flat-square) | 2025-10-23 | MIT |
| [QuantConnect/mcp-server](https://github.com/QuantConnect/mcp-server) | **공식** QuantConnect MCP 서버 — AI 어시스턴트가 Python 트레이딩 전략을 작성하고, 클라우드 백테스트를 실행하며, QuantConnect 플랫폼에 라이브 알고리즘을 배포. | ![Stars](https://img.shields.io/github/stars/QuantConnect/mcp-server?style=flat-square) | 2026-05-07 | Apache-2.0 |
| [koreainvestment/open-trading-api](https://github.com/koreainvestment/open-trading-api) | **공식** 한국투자증권 Open API — MCP 및 LLM 통합 SDK(토픽: mcp, claude, llm, autotrade)로 국내 주식 시장 트레이딩, 실시간 시세, 주문 관리, AI 전략 예제 포함. | ![Stars](https://img.shields.io/github/stars/koreainvestment/open-trading-api?style=flat-square) | 2026-06-24 | — |

### 리서치 & 분석

| 프로젝트 | 설명 | 스타 | 최근 푸시 | 라이선스 |
|---------|------|------|----------|---------|
| [mnemox-ai/tradememory-protocol](https://github.com/mnemox-ai/tradememory-protocol) | AI 트레이딩 에이전트를 위한 오픈소스 메모리 MCP — 3계층 아키텍처(L1 원시 거래 메모리, L2 패턴 반성, L3 전략 진화)로 에이전트가 과거 거래에서 학습. | ![Stars](https://img.shields.io/github/stars/mnemox-ai/tradememory-protocol?style=flat-square) | 2026-06-01 | MIT |
| [wshobson/maverick-mcp](https://github.com/wshobson/maverick-mcp) | AI 어시스턴트를 위한 개인 주식 분석 MCP 서버 — 기술 지표, 실적 캘린더, 옵션 플로우, 내부자 거래, 섹터 분석 제공. | ![Stars](https://img.shields.io/github/stars/wshobson/maverick-mcp?style=flat-square) | 2026-06-20 | MIT |
| [stefanoamorelli/sec-edgar-mcp](https://github.com/stefanoamorelli/sec-edgar-mcp) | AI 어시스턴트에게 SEC EDGAR 공시(10-K, 10-Q, 8-K, 내부자 거래)에 직접 접근을 제공하는 MCP 서버 — 기본적 리서치 및 실사에 활용. | ![Stars](https://img.shields.io/github/stars/stefanoamorelli/sec-edgar-mcp?style=flat-square) | 2026-06-23 | AGPL-3.0 |

---

## 🧠 AI 에이전트 프레임워크 & 플랫폼

금융 분석, 리서치, 트레이딩 워크플로우에 특화된 멀티에이전트 및 LLM 오케스트레이션 프레임워크.

| 프로젝트 | 설명 | 스타 | 최근 푸시 | 라이선스 |
|---------|------|------|----------|---------|
| [TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents) | 실제 트레이딩 회사를 모방한 멀티에이전트 LLM 트레이딩 프레임워크 — 펀더멘털·감성·기술·리스크·포트폴리오 관리 전문 에이전트들이 LangGraph를 통해 거래 결정에 합의. | ![Stars](https://img.shields.io/github/stars/TauricResearch/TradingAgents?style=flat-square) | 2026-06-22 | Apache-2.0 |
| [AI4Finance-Foundation/FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) | 감성 분석·로보어드바이저·트레이딩 신호 생성 등의 태스크에서 LoRA/QLoRA로 일반 모델(LLaMA, ChatGLM, Qwen)을 파인튜닝하는 오픈소스 금융 LLM 프레임워크. 사전 학습 모델 HuggingFace 제공. | ![Stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinGPT?style=flat-square) | 2026-06-01 | MIT |
| [AI4Finance-Foundation/FinRobot](https://github.com/AI4Finance-Foundation/FinRobot) | 금융 인식·분석·자동화된 리서치 보고서 생성을 위한 4계층 아키텍처의 오픈소스 AI 에이전트 플랫폼. | ![Stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinRobot?style=flat-square) | 2026-05-10 | Apache-2.0 |
| [coinbase/agentkit](https://github.com/coinbase/agentkit) | **공식** Coinbase 프레임워크로 모든 AI 에이전트에 암호화폐 지갑 부여 — LangChain·CrewAI 호환, Base 및 Ethereum에서 온체인 토큰 전송·DeFi 프로토콜 상호작용·NFT 민팅·거래 실행 지원. | ![Stars](https://img.shields.io/github/stars/coinbase/agentkit?style=flat-square) | 2026-06-23 | — |

---

## 📈 AI 기반 애플리케이션

AI 투자 코파일럿, 자율 헤지펀드 시뮬레이터, LLM 기반 시장 분석 플랫폼 등 바로 사용 가능한 엔드투엔드 도구.

| 프로젝트 | 설명 | 스타 | 최근 푸시 | 라이선스 |
|---------|------|------|----------|---------|
| [virattt/ai-hedge-fund](https://github.com/virattt/ai-hedge-fund) | 버핏·멍거·버리·린치 등 전설적 투자자를 모방한 18개의 전문 에이전트가 LangGraph를 통해 토론하고 거래 신호를 생성하는 멀티에이전트 LLM 헤지펀드 시뮬레이터 — 풀스택 웹 UI와 CLI 포함. | ![Stars](https://img.shields.io/github/stars/virattt/ai-hedge-fund?style=flat-square) | 2026-06-17 | MIT |
| [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | A/H/미국 시장을 위한 LLM 기반 일일 분석 시스템 — 다중 소스 시장 데이터와 실시간 뉴스를 집계하고 매수/보유/매도 결정 대시보드 생성 및 WeChat·Telegram·Slack·이메일로 알림 발송. | ![Stars](https://img.shields.io/github/stars/ZhuLinsen/daily_stock_analysis?style=flat-square) | 2026-06-28 | MIT |
| [anthropics/financial-services](https://github.com/anthropics/financial-services) | **공식** Anthropic 금융 서비스 플러그인 및 에이전트 쿡북 — DCF 가치평가, LBO 모델링, 주식 리서치, 자산 관리, KYC 파싱, GL 대사, 채권 분석 포함; Claude 플러그인으로 설치 가능. | ![Stars](https://img.shields.io/github/stars/anthropics/financial-services?style=flat-square) | 2026-06-26 | Apache-2.0 |
| [Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal) | AI 에이전트로 구축된 블룸버그 터미널 대안 — 고급 시장 분석, AI 기반 투자 리서치, 거시경제 데이터 탐색, 알고리즘 트레이딩 도구; Python/C++/Qt 데스크톱 앱. | ![Stars](https://img.shields.io/github/stars/Fincept-Corporation/FinceptTerminal?style=flat-square) | 2026-06-24 | — |
| [virattt/dexter](https://github.com/virattt/dexter) | 심층 금융 리서치를 위한 자율 에이전트 — SEC 공시·실적 발표 스크립트·애널리스트 리포트·뉴스를 읽고 구조화된 투자 리서치를 생성; TypeScript, ai-hedge-fund 제작자 작품. | ![Stars](https://img.shields.io/github/stars/virattt/dexter?style=flat-square) | 2026-06-28 | — |
| [HKUDS/AI-Trader](https://github.com/HKUDS/AI-Trader) | 100% 완전 자동화된 에이전트 네이티브 트레이딩 시스템 — 시장 데이터 수집부터 주문 실행까지 LLM 에이전트를 활용한 엔드투엔드 파이프라인; Vibe-Trading과 동일 팀 제작. | ![Stars](https://img.shields.io/github/stars/HKUDS/AI-Trader?style=flat-square) | 2026-06-11 | — |
| [UFund-Me/Qbot](https://github.com/UFund-Me/Qbot) | 로컬 배포 가능한 AI 기반 퀀트 투자 리서치 플랫폼 — LLM을 퀀트 전략 모듈과 통합하여 자동 신호 생성, 백테스팅, 모의 트레이딩 지원. | ![Stars](https://img.shields.io/github/stars/UFund-Me/Qbot?style=flat-square) | 2026-03-11 | MIT |
| [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 자연어 전략 설명을 백테스팅된 실행 가능 트레이딩 코드로 변환하는 개인 트레이딩 에이전트 — 29개 멀티에이전트 프리셋, 79개 금융 스킬, TradingView Pine Script 및 MetaTrader 5 내보내기 지원. | ![Stars](https://img.shields.io/github/stars/HKUDS/Vibe-Trading?style=flat-square) | 2026-06-28 | MIT |
| [The-Swarm-Corporation/AutoHedge](https://github.com/The-Swarm-Corporation/AutoHedge) | 스웜 기반 멀티에이전트 AI로 시장 분석·리스크 관리·거래 실행을 수행하는 자율 헤지펀드 엔진 — Solana 실시간 트레이딩 지원. | ![Stars](https://img.shields.io/github/stars/The-Swarm-Corporation/AutoHedge?style=flat-square) | 2026-05-11 | MIT |
| [marketcalls/openalgo](https://github.com/marketcalls/openalgo) | AI 에이전트 통합을 위한 내장 MCP 서버를 갖춘 오픈소스 알고리즘 트레이딩 플랫폼 — 시각적 플로우 전략 빌더, 실시간 손익 추적, 멀티 브로커 지원, Telegram 알림 포함. | ![Stars](https://img.shields.io/github/stars/marketcalls/openalgo?style=flat-square) | 2026-06-25 | AGPL-3.0 |
| [virattt/ai-financial-agent](https://github.com/virattt/ai-financial-agent) | Financial Datasets API에 연결하여 미국 주식 가격·재무제표·옵션 활동·내부자 거래를 분석하는 셀프호스팅 LLM 금융 리서치 에이전트; ai-hedge-fund 제작자 작품. | ![Stars](https://img.shields.io/github/stars/virattt/ai-financial-agent?style=flat-square) | 2025-08-19 | — |
| [Lumiwealth/lumibot](https://github.com/Lumiwealth/lumibot) | 주식·옵션·암호화폐·선물·외환 백테스팅 가능한 AI 트레이딩 에이전트 프레임워크 — SEC 공시·FRED 거시경제·기술 지표·DuckDB 분석·Telegram 알림 내장 AI 도구; 실시간 브로커 연결 지원. | ![Stars](https://img.shields.io/github/stars/Lumiwealth/lumibot?style=flat-square) | 2026-06-25 | GPL-3.0 |
| [DemonDamon/FinnewsHunter](https://github.com/DemonDamon/FinnewsHunter) | 실시간 금융 뉴스를 수집·분석하고 시장 감성을 종합하여 LLM 파이프라인으로 구조화된 투자 인사이트를 제공하는 멀티에이전트 금융 인텔리전스 플랫폼. | ![Stars](https://img.shields.io/github/stars/DemonDamon/FinnewsHunter?style=flat-square) | 2026-01-13 | Apache-2.0 |
| [51bitquant/ai-hedge-fund-crypto](https://github.com/51bitquant/ai-hedge-fund-crypto) | 암호화폐 트레이딩 특화 AI 헤지펀드 프레임워크 — LLM 에이전트와 멀티타임프레임 LangGraph 워크플로우로 시장 분석 및 암호화폐 거래소에서 전략 실행. | ![Stars](https://img.shields.io/github/stars/51bitquant/ai-hedge-fund-crypto?style=flat-square) | 2025-09-05 | MIT |
| [ivebotunac/PrimoAgent](https://github.com/ivebotunac/PrimoAgent) | 기술·펀더멘털·감성·포트폴리오 4개 전문 에이전트가 일일 트레이딩 인사이트와 다음날 주가 예측을 생성하는 LangGraph 멀티에이전트 주식 분석 시스템. | ![Stars](https://img.shields.io/github/stars/ivebotunac/PrimoAgent?style=flat-square) | 2026-01-12 | MIT |
| [EthanAlgoX/LLM-TradeBot](https://github.com/EthanAlgoX/LLM-TradeBot) | Binance 선물 특화 멀티에이전트 AI 트레이딩 시스템 — LLM으로 전략을 실시간 생성·평가·적응하며 포트폴리오 매니저 에이전트가 다수의 전문 서브에이전트를 조율. | ![Stars](https://img.shields.io/github/stars/EthanAlgoX/LLM-TradeBot?style=flat-square) | 2026-04-16 | MIT |

---

## 👥 활성 커뮤니티

AI + 금융 실무자들이 함께 구축하고, 공유하며, 협업하는 Discord 서버와 포럼.

| 커뮤니티 | 플랫폼 | 멤버 수 | 초점 |
|---------|--------|--------|------|
| [LuxAlgo](https://discord.com/servers/luxalgo-641770286638694402) | Discord | 100,000+ | AI 기반 TradingView 지표 및 전략 생성 — "Quant" 제품이 일반 텍스트를 LLM을 통해 백테스팅된 Pine Script로 변환; 공식 Discord 파트너 |
| [AI4Finance Foundation](https://github.com/AI4Finance-Foundation/FinGPT) | Discord | 12,000+ | 오픈소스 금융 LLM(FinGPT, FinRobot), 금융 NLP, LLM 벤치마킹 — FinGPT README의 배지를 통해 참여 |
| [Hummingbot](https://hummingbot.org/community/discord) | Discord | 다수 | 알고리즘 트레이딩 봇 개발, 마켓 메이킹, 거래소 커넥터, AI 지원 전략 구축; 재단 운영, 주간 팟캐스트 |
| [LLMQuant](https://llmquant.com) | Discord + GitHub | 초대제 | 퀀트 리서치를 위한 LLM — 투자 리서치 AI 에이전트, 오픈소스 퀀트 도구, MCP 통합 시장 데이터; 웹사이트에서 신청 |

---

## 📚 큐레이션 인덱스

더 많은 AI 금융 도구를 발견하기 위한 고품질 집계 사이트:

| 프로젝트 | 설명 | 스타 |
|---------|------|------|
| [BlockRunAI/awesome-finance-mcp](https://github.com/BlockRunAI/awesome-finance-mcp) | AI 금융 에이전트를 위한 MCP 서버 큐레이션 목록 — Alpaca, Financial Datasets, Alpha Vantage, QuantConnect, FRED, 전문 퀀트 도구 포함. | ![Stars](https://img.shields.io/github/stars/BlockRunAI/awesome-finance-mcp?style=flat-square) |
| [LLMQuant/awesome-trading-agents](https://github.com/LLMQuant/awesome-trading-agents) | 주식·암호화폐·DeFi·예측 시장에 걸친 AI 트레이딩 에이전트, MCP 서버, Claude 스킬, 벤치마크 종합 인덱스. | ![Stars](https://img.shields.io/github/stars/LLMQuant/awesome-trading-agents?style=flat-square) |
| [georgezouq/awesome-ai-in-finance](https://github.com/georgezouq/awesome-ai-in-finance) | 에이전트·MCP 서버·퀀트 인프라·DeFi 도구를 포함한 금융 시장 LLM + AI 도구 광범위 인덱스. | ![Stars](https://img.shields.io/github/stars/georgezouq/awesome-ai-in-finance?style=flat-square) |

---

## 기여하기

PR을 환영합니다. 제출 전 다음을 확인해 주세요:

1. **AI 우선:** 도구가 LLM, AI 에이전트, 또는 고급 NLP를 각주가 아닌 핵심으로 사용해야 함
2. **스코프 내:** Finance = 트레이딩 / 투자 / 포트폴리오 관리 / 시장 데이터 / 퀀트 리서치. **스코프 외:** 콘텐츠 수익화 도구, SNS 자동화, 일반적인 "AI로 돈 벌기" 도구
3. **활성 상태:** GitHub `pushed_at`이 12개월 이내이거나 명성 높은 재단 프로젝트
4. **중복 없음:** 유사한 도구가 있다면 의미 있게 다른 목적을 갖거나 스타 수가 현저히 많아야 함

라이선스 열: 선언된 경우 SPDX 식별자(예: `MIT`, `Apache-2.0`) 표기; GitHub에서 라이선스를 감지하지 못하거나 인식 불가한 경우 `—` 표기. `—`인 레포는 사용자가 직접 판단하여 사용하세요.

행당 하나의 항목: 이름, AI/LLM 기능에 초점을 맞춘 한 문장 설명, 스타 배지, 최근 푸시 날짜, 라이선스.

---

## 라이선스

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
