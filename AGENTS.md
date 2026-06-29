# AGENTS.md — Research Methodology & Curation Criteria

이 문서는 `awesome-ai-finance` 리스트를 구성하기 위해 AI 에이전트가 수행한 검색 전략, 데이터 수집 방법, 품질 검증 기준을 기록합니다.

---

## 1. 검색 파이프라인 개요

```
Layer 1: 키워드 매트릭스 검색 (병렬 15개 쿼리)
    ↓
Layer 2: GitHub Topics 크롤링
    ↓
Layer 3: MCP 레지스트리 파싱 (Smithery, Glama)
    ↓
Layer 4: GitHub API 검증 (실측 star수, 커밋일, 라이선스)
    ↓
Layer 5: 큐레이션 필터 적용
    ↓
README.md 반영
```

총 **8회 병렬 배치**, **약 60개+ GitHub API 직접 호출**, **55개 후보 레포** 평가 후 최종 **37개 레포** 선정 (커뮤니티 4 + 인덱스 3 포함 시 44개 항목).

---

## 2. 검색 전략 (Search Strategy)

### 2-1. Multi-Layered Keyword Matrix

단순 단일 키워드 검색이 아닌, 3개 레이어의 조합으로 15개 이상의 쿼리를 생성해 실행했습니다.

| Layer A (기술 스택) | Layer B (금융 도메인) | Layer C (플랫폼 한정자) |
|---|---|---|
| `"langgraph"` / `"crewai"` / `"autogen"` | `"trading"` / `"quant"` / `"portfolio"` | `site:github.com` |
| `"llm-agent"` / `"ai-agent"` | `"financial analysis"` / `"alpha"` | `"open source"` |
| `"mcp-server"` / `"smolagents"` | `"crypto"` / `"defi"` / `"algorithmic"` | `in:readme` / `in:description` |

**실행된 쿼리 예시:**
```
"langgraph" "trading" site:github.com
"crewai" "portfolio" OR "finance" site:github.com
"autogen" "alpha generation" OR "portfolio" site:github.com
"mcp-server" "portfolio" OR "crypto" site:github.com
"financial agent" "LangChain" OR "LlamaIndex" site:github.com
"smolagents" "finance" OR "trading" site:github.com
```

### 2-2. GitHub Topics 크롤링

GitHub의 커뮤니티 태그 기반 집계 페이지를 직접 파싱했습니다:

- `https://github.com/topics/mcp-server` → `finance`, `trading`, `portfolio` 키워드 필터
- `https://github.com/topics/ai-agent` → `trading`, `quant`, `financial` 필터
- `https://github.com/topics/algorithmic-trading` → LLM/GPT/Claude 언급 여부 확인
- GitHub Advanced Search: `stars:>200 pushed:>2026-01-01 "financial agent"`

### 2-3. MCP 레지스트리 파싱

표준 구글 검색으로는 발견하기 어려운 MCP 서버들을 레지스트리에서 직접 추출했습니다:

- **Smithery.ai** — `/search?q=finance`, `/search?q=trading`, `/search?q=crypto`, `/search?q=portfolio` 탐색
- **Glama.ai** — `Finance`, `Data`, `Crypto`, `Business` 카테고리 필터
- **PulseMCP** — finance/trading 키워드로 install count 기준 정렬, SEC/EDGAR 특화 서버 추출 (edgartools 1,847 installs 발견)
- **TensorBlock/awesome-mcp-servers** — GitHub에서 관리되는 큐레이션 목록, finance 섹션에서 알파벤티지·FRED·EVM 서버 발굴
- **BlockRunAI/awesome-finance-mcp** — finance MCP 전용 큐레이션 목록
- **LLMQuant/awesome-trading-agents** — trading agent + MCP 종합 인덱스 (60개+ 후보 일괄 수집)
- mcp.so: HTTP 403 차단으로 접근 불가 → TensorBlock 우회 활용
- 각 서버의 `sourceUrl` 또는 `repository` 필드에서 GitHub URL 역추적
- GitHub URL이 없는 순수 호스티드 서버(marketflux-mcp, korean-stocks, bitquery-mcp)는 공개 오픈소스가 아님을 확인 후 제외

### 2-4. 커뮤니티 마이닝

Reddit 및 개발자 커뮤니티에서 실사용 프로젝트 수집:

- `r/algotrading` — `"llm agent" OR "ai agent" finance github` 쿼리 실행
- `r/LocalLLaMA` — `finance OR trading github` 쿼리 실행
- `r/ClaudeAI`, `r/WebAfterAI` — LLM 금융 도구 공유 포스트 추출
- `r/wallstreetbets` (13M 멤버) — GitHub 프로젝트 포스팅 없음 확인 (DD 포스트가 주를 이루며 원본 개발 도구 링크는 거의 없음)
- HackerNews Show HN: `"Show HN" "trading" OR "finance" "LLM" OR "AI agent"` 실행
- dev.to: `"AI finance" OR "MCP trading" 2025` 키워드 스캔 → tradememory-protocol 발견

---

## 3. 데이터 검증 방법

### 3-1. GitHub API 직접 호출 (핵심 원칙)

검색 스니펫의 수치를 **절대 신뢰하지 않고** 모든 후보 레포에 대해 GitHub REST API를 직접 호출했습니다:

```
GET https://api.github.com/repos/{owner}/{repo}
```

추출 필드:
- `stargazers_count` — 실제 스타 수
- `pushed_at` — 마지막 커밋 날짜
- `license.spdx_id` — 라이선스 식별자
- `archived` — 아카이브(읽기전용) 여부
- `fork` — 포크 여부

### 3-2. STALE 판정 기준

```
pushed_at < 2024-12-28  →  STALE (6개월 기준, 기준일: 2026-06-29)
```

STALE로 판정된 레포는 원칙적으로 제외하되, 학술적 가치가 높은 경우 별도 주석 처리.

### 3-3. 의심 레포 플래그 (SUSPICIOUS)

스타 증가 속도가 비정상적으로 빠른 경우 플래그를 붙이고 추가 검토:

| 레포 | 스타 | 일평균 | 판정 |
|------|------|--------|------|
| `virattt/dexter` | 27,221★ | ~105/일 | ✅ License: — 로 표기 후 포함 (정책 변경) |
| `Fincept-Corporation/FinceptTerminal` | 27,617★ | ~41/일 | ❌ C++ 기반, AI 부차적 기능 → 스코프 밖 |
| `HKUDS/Vibe-Trading` | 14,126★ | ~159/일 | ✅ MIT 라이선스 + 활발한 커밋으로 포함 |
| `HKUDS/AI-Trader` | 20,227★ | ~81/일 | ✅ License: — 로 표기 후 포함 (정책 변경) |

---

## 4. 포함 기준 (Inclusion Criteria)

레포가 다음 **모든 조건**을 충족해야 포함됩니다:

### ✅ 필수 조건

| 기준 | 세부 내용 |
|------|----------|
| **AI-First** | LLM, AI 에이전트, 또는 고급 NLP가 핵심 기능. 단순히 README에서 언급되는 것은 불인정 |
| **Finance 스코프** | trading / investing / portfolio / market data / quant research. 콘텐츠 수익화·SNS 자동화 제외 |
| **라이선스** | 선언된 라이선스 있으면 SPDX ID 표기; `null` / `NOASSERTION`은 License 열에 `—` 표기 후 포함 |
| **활성 유지** | `pushed_at` ≥ 2024-12-28 (6개월 이내) 또는 높은 명성의 재단 프로젝트 |
| **비아카이브** | `archived: false` |

### ✅ 권장 기준 (우선순위에 영향)

- 스타 수가 높을수록 우선 배치
- 동일 목적의 중복 레포가 있을 경우 스타 수가 높은 것 1개만 유지
- 공식(Official) 레포 우대 (예: alpacahq 공식 MCP > 커뮤니티 구현체)

---

## 5. 제외 기준 (Exclusion Criteria)

| 제외 사유 | 예시 |
|----------|------|
| RL/DL 훈련 프레임워크 | `AI4Finance-Foundation/FinRL` (강화학습 훈련 필요) |
| Finance 스코프 밖 | `yikart/AiToEarn` (22k★, 중국 SNS 크리에이터 수익화 자동화) |
| STALE | `pipiku915/finmem-llm-stocktrading` (마지막 커밋 2024-08-18) |
| ARCHIVED | `wshobson/mcp-trader` (maverick-mcp로 대체됨) |
| 토이 프로젝트 | ★32 미만 + 공식 레포와 기능 중복 |
| 레거시 플랫폼 | `OpenBB-finance/OpenBB` (LLM-first가 아닌 범용 플랫폼) |
| 공개 GitHub 없음 | marketflux-mcp, korean-stocks (Smithery 호스티드 전용) |
| 중복 | `laukikk/alpaca-mcp` (★32, `alpacahq/alpaca-mcp-server` ★846과 동일 목적) |

---

## 6. 카테고리 분류 기준

### 🔌 AI Finance Connectors & MCP Servers
- MCP 프로토콜을 사용하는 서버
- AI 어시스턴트(Claude, Cursor 등)와 금융 데이터/API를 연결하는 레이어
- 서브카테고리: Market Data / Trading Execution / Research & Analysis

### 🧠 AI Agent Frameworks & Platforms
- 금융 워크플로우에 특화된 멀티에이전트 오케스트레이션 프레임워크
- 다른 도구/에이전트를 빌드하기 위한 플랫폼적 성격

### 📈 AI-Powered Applications
- 최종 사용자가 바로 실행할 수 있는 엔드-투-엔드 도구
- AI 투자 코파일럿, 자율 헤지펀드 시뮬레이터, LLM 기반 시장 분석 앱

### 👥 Active Communities
- GitHub 레포가 아닌 Discord/Slack/Forum 커뮤니티
- AI + 금융 실무자들이 활발히 활동 중인 곳

---

## 7. 향후 개선 과제

검색 파이프라인 실행 중 다음 항목은 완전히 수행되지 않았습니다:

| 미완료 항목 | 사유 | 제안 보완 방법 |
|------------|------|--------------|
| mcp.so 전체 파싱 | HTTP 403 차단 | 6개월 후 재시도 또는 Wayback Machine 우회 |
| smolagents 금융 레포 | 발견된 레포 없음 (블로그 포스트 수준) | 6개월 후 재탐색 |
| Composio.dev finance connectors | JS 렌더 필요로 파싱 어려움 | Playwright 기반 스크래핑 |
| HuggingFace Spaces finance | 스크리닝 미완료 | `filter=finance` Spaces 추가 탐색 |
| r/quant, r/CryptoCurrency 커뮤니티 | 우선순위 이후 | 다음 분기 검색 확장 |

---

## 8. 업데이트 주기 제안

| 항목 | 주기 | 방법 |
|------|------|------|
| 스타 수 갱신 | 자동 | GitHub Shields.io 배지 (실시간) |
| 신규 레포 발굴 | 분기 1회 | 이 AGENTS.md의 검색 전략 재실행 |
| STALE 점검 | 분기 1회 | `pushed_at` 재확인 |
| 라이선스 변경 점검 | 반기 1회 | GitHub API `license` 필드 재확인 |

---

---

## 9. 주요 제외 사례 (High-profile Exclusions)

스타 수가 높지만 기준 미달로 제외된 레포:

| 레포 | 스타 | 제외 사유 |
|------|------|---------|
| `HKUDS/AI-Trader` | 20,225★ | `license: null` — 라이선스 미선언 |
| `Fincept-Corporation/FinceptTerminal` | 27,617★ | `license: NOASSERTION` → License: — 표기 후 포함 (정책 변경) |
| `virattt/dexter` | 27,197★ | `license: null` |
| `coinbase/agentkit` | 1,255★ | `license: NOASSERTION` |
| `koreainvestment/open-trading-api` | 1,490★ | `license: null` |
| `twelvedata/mcp` | 70★ | `license: null` |
| `pipiku915/finmem-llm-stocktrading` | — | `pushed_at: 2024-08-18` (STALE) |
| `wshobson/mcp-trader` | — | ARCHIVED (maverick-mcp로 대체) |

*Last updated: 2026-06-29 | Maintained by AI agent pipeline*
