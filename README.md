# 생성형 AI 강의 슬라이드 — 데이터 분석 · LLM 서비스 · 전문성과 암묵지

reveal.js 기반 강의 슬라이드 모음입니다. 각 강의는 빌드 없이 단일 `index.html`로 동작합니다.

이 저장소는 [geniuskey/vibe-coding-202607](https://github.com/geniuskey/vibe-coding-202607)
템플릿을 참고해 만들었으며, **아래 세 강의가 직접 제작한 자료**입니다.
루트 `index.html`, `context/`, `forChildren/`, `workshop/`, 실시간 Q&A 서버(`server.js`)는
원본 템플릿에서 가져온 참고 자료입니다.

## 강의 자료

### 1. 생성형 AI를 활용한 데이터 분석의 기초 — `data-analysis/`
- 슬라이드: [`data-analysis/index.html`](data-analysis/index.html)
- 대상: 데이터 분석가 · 데이터를 다루는 실무자
- 내용: 탐색적 데이터 분석(EDA) 보조, pandas·SQL·시각화 코드 생성,
  AI 분석 결과의 한계와 교차검증, 생성형 AI 도구 비교
- 구성 문서: `data-analysis/outline.md`(콘텐츠 소스), `data-analysis/slides-outline.md`(슬라이드 목차)

### 2. LLM 서비스, 업무의 무기로 — `llm-services/`
- 슬라이드: [`llm-services/index.html`](llm-services/index.html)
- 대상: LLM을 처음 접하는 비즈니스 시니어
- 내용: 기존 도구와의 비교, ChatGPT·Claude·Gemini(Enterprise) 성격 비교,
  활용 3단계 로드맵(대화 → 제작 → 위임), 실무 꿀팁
- 구성 문서: `llm-services/outline.md`(콘텐츠 소스), `llm-services/slides-outline.md`(슬라이드 목차)

### 3. 전문가는 덜 본다 — AI 시대에 사람이 하는 일 — `tacit-knowledge/`
- 슬라이드: [`tacit-knowledge/index.html`](tacit-knowledge/index.html)
- 대상: AI에 관심 있는 일반 직원
- 주제: AI가 답을 싸게 공급하는 시대에, **개인의 역량을 어떻게 조직의 능력으로 바꿀 것인가**
- 구성: 네 개의 질문으로 진행합니다.
  1. 전문가는 무엇이 다른가 — 전문성은 아는 양이 아니라 문제를 보는 방식(Chase & Simon, RPD)
  2. 그것을 꺼낼 수 있는가 — 암묵지의 3개 층위, 절차서와 실제 작업의 간극
  3. AI는 무엇을 싸게 만들었는가 — 다음 토큰 예측, 경계 안(+40%)과 밖(−23%)
  4. 그래서 조직과 나는 무엇을 관리하는가 — 지식 순환 루프와 개인 실천 3가지
- 특징: 본문 인용 23건에 모두 출처가 붙어 있고, 강의 중 **사전 과제 응답**을 두 슬라이드에
  직접 채워 넣는 구성입니다(아래 "사전 과제" 참고).

#### 제작 파이프라인 문서 (`tacit-knowledge/`)

이 강의는 조사 → 구조화 → 교안 → 슬라이드 설계 → 검수 순서로 만들었고,
각 단계의 **프롬프트와 산출물**을 함께 남겨 두었습니다.

| 단계 | 프롬프트 | 산출물 |
|------|----------|--------|
| 기초 조사 | `search-prompt.md` | `research-base.md`(연구 1~46), `research-supplement.md`(47~52) |
| 콘텐츠 구조화 | `architecture-prompt.md` | `course-architecture.md`(교육 목표·챕터·시간표·반론 대비) |
| 교안 작성 | `teaching-prompt.md` | `teaching-script.md`(슬라이드별 강사 대본) |
| 슬라이드 설계 | `design-prompt.md` | `slide-design.md`(콘텐츠 의미 구조 명세) |
| 최종 검수 | `verification-prompt.md` | `verification-report.md`, `instructional-review.md` |

#### 사전 과제 (강의 3~5일 전 발송)

Chapter 3에서 청중의 응답을 그대로 화면에 띄웁니다. 5분 이내, 익명 수집.

1. *"우리 회사의 사내 소통을 개선할 아이디어를 3가지 제안해줘."* 를 평소 쓰는 AI에 그대로
   넣고, 나온 아이디어 3개를 적어 보내기 → 겹치는 키워드를 묶어 슬라이드에 표시
2. 업무에서 **AI에게 물어봐도 제대로 된 답이 안 나올 질문 한 가지** 적기
   → "우리 조직의 맥락지식 목록"으로 Chapter 4에 연결

응답을 아직 채우지 않은 채로 슬라이드를 열면 상단에 경고 막대가 뜨고,
**「대체 데이터 사용」** 버튼으로 강사 준비 세트로 전환할 수 있습니다.
자세한 설계는 `course-architecture.md` §9.2를 보세요.

## 슬라이드 여는 법

세 강의 모두 **단일 HTML 파일**이라 빌드·설치가 필요 없습니다.

- **바로 열기**: `data-analysis/index.html`, `llm-services/index.html`,
  `tacit-knowledge/index.html`을 브라우저로 엽니다.
- **정적 호스팅**: 저장소를 GitHub Pages 등에 올린 뒤 `.../data-analysis/`,
  `.../llm-services/`, `.../tacit-knowledge/` 경로로 접속합니다.

발표 조작(reveal.js 공통): 화살표·Space 이동, `F` 전체화면, `S` 발표자 노트, `O` 개요 보기, `Esc` 슬라이드 목록.

`tacit-knowledge/`는 발표용 조작이 조금 다릅니다. 화면 우상단 도구막대에 **목차 드롭다운**과
전체화면 버튼이 있고(3초간 조작이 없으면 흐려짐), 단축키는 `F` 전체화면 · `R` 첫 슬라이드로 복귀 ·
`T` 도구막대 표시/숨김입니다. 발표자 노트 창은 쓰지 않고, 강사 대본은 `teaching-script.md`에 있습니다.

## 저장소 구조

| 경로 | 내용 | 비고 |
|------|------|------|
| `data-analysis/` | 데이터 분석 강의 | **직접 제작** |
| `llm-services/` | LLM 서비스 활용 강의 | **직접 제작** |
| `tacit-knowledge/` | 전문성·암묵지·조직지식 강의(+제작 문서 전체) | **직접 제작** |
| `index.html`(루트) | 바이브 코딩 세미나 덱 | 원본 템플릿 |
| `context/` · `forChildren/` · `workshop/` | 원본 템플릿의 부속 덱 | 원본 템플릿 |
| `server.js` · `package.json` · `test/` | 루트 덱용 실시간 Q&A 서버와 테스트 | 원본 템플릿 |

## 출처

원본 템플릿: [geniuskey/vibe-coding-202607](https://github.com/geniuskey/vibe-coding-202607)
(reveal.js 단일 파일 슬라이드 구조 참고).
