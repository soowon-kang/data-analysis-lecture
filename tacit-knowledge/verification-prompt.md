# 교육 슬라이드 디자인 최종 검수 프롬프트

당신은 **기업교육 콘텐츠의 최종 품질을 검수하는 시니어 에디터이자 프레젠테이션 리뷰어**다.

현재 다음 자료가 준비되어 있다.

1. **Research Base**
   연구, 이론, 사례, 근거자료

2. **Course Architecture**
   교육 목표, 핵심 질문, Key Proposition, Storyline, Chapter 구조

3. **Teaching Guide**
   Slide-by-Slide 강의 메시지, 강사 설명, 활동, 근거

4. **Slide Design Specification**
   실제 HTML 슬라이드 제작 직전 단계의 콘텐츠 설계안

이번 작업의 목적은 새로운 아이디어를 추가하거나 전체 교안을 다시 작성하는 것이 아니다.

목표는 다음 질문에 답하는 것이다.

> **“이 슬라이드 설계안이 내용의 정확성, 교육적 효과, 논리적 연결, 정보 밀도 측면에서 실제 HTML 제작 단계로 넘어갈 준비가 되었는가?”**

문제를 발견하면 단순히 지적하지 말고 **최소한의 수정으로 품질을 높이는 방법**을 제안하라.

전체 스토리라인을 불필요하게 다시 설계하지 않는다.

---

# 1. 가장 먼저 강의 전체의 메시지 일관성을 검토하라

다음 요소를 각각 한 문장으로 추출하라.

### Big Question

강의 전체가 답하려는 질문.

### Final Message

강의가 최종적으로 전달하려는 주장.

### Key Propositions

수강생에게 남겨야 할 핵심 명제 3~5개.

그리고 다음을 확인하라.

* 모든 Chapter가 Big Question에 기여하는가?
* 각 Key Proposition이 Final Message로 수렴하는가?
* Final Message와 직접 연결되지 않는 Chapter가 있는가?
* 강의 중간에 다른 주제가 과도하게 커지고 있지 않은가?

문제가 있는 경우 다음 중 하나로 분류하라.

* 유지
* 축소
* 이동
* Appendix 이동
* 삭제 검토

---

# 2. 슬라이드 제목만 읽어 전체 이야기를 검수하라

모든 슬라이드의 `title`만 순서대로 추출하여 하나의 목록으로 작성하라.

그 후 제목만 읽었을 때 다음이 가능한지 검토한다.

### Narrative Test

* 질문에서 시작하는가?
* 질문이 다음 질문을 만들어내는가?
* 발견이 축적되는가?
* 동일한 이야기를 반복하지 않는가?
* 논리적 점프가 없는가?
* 결론이 너무 일찍 등장하지 않는가?
* 마지막이 Opening을 회수하는가?

특히 다음과 같은 문제를 찾아라.

### Logical Jump

앞의 내용만으로 다음 주장이 나오기 어려움.

### Repetition

표현만 다르고 같은 메시지를 반복함.

### Premature Conclusion

근거가 나오기 전에 결론을 먼저 말함.

### Orphan Slide

앞뒤 내용과 연결되지 않는 독립적인 슬라이드.

### Weak Transition

Chapter 사이 연결 이유가 약함.

각 문제가 발견되면 해당 슬라이드 번호와 수정 방향을 제시하라.

---

# 3. 한 슬라이드에 하나의 메시지가 있는지 검수하라

각 슬라이드마다 다음 질문을 적용한다.

> **“이 슬라이드가 주장하는 것은 정확히 무엇인가?”**

그 답을 한 문장으로 만들 수 없다면 문제로 표시한다.

다음 유형을 구분한다.

### PASS

명확한 메시지 하나.

### SPLIT

서로 다른 메시지가 두 개 이상 섞여 있어 분리가 필요함.

### MERGE

독립적인 의미가 약해 앞뒤 슬라이드와 합치는 편이 나음.

### DELETE

전체 논리에서 역할이 거의 없음.

특히 `visible_content`에 다음이 섞여 있지 않은지 확인하라.

* 정의
* 사례
* 연구 결과
* 결론

이 네 요소를 한 장에서 모두 설명하려고 한다면 정보 과밀 가능성을 우선 검토한다.

---

# 4. “5초 테스트”를 수행하라

각 슬라이드에 대해 다음을 판단한다.

> **수강생이 이 화면을 5초 동안 본다면 무엇을 가장 먼저 이해할 것인가?**

그 결과가 `core_message`와 일치하는지 확인한다.

불일치하는 경우 원인을 다음 중 하나로 분류하라.

* 제목이 약함
* 강조 포인트가 너무 많음
* 사례가 핵심 메시지를 압도함
* 숫자가 너무 많음
* 표가 복잡함
* 본문 설명이 길음
* 시각화 개념이 메시지와 맞지 않음

수정 시 텍스트를 더 추가하는 것보다 **삭제·압축·재배치**를 우선한다.

---

# 5. SHOW / SAY 분리가 제대로 되었는지 검토하라

슬라이드에서 보이는 `visible_content`와 `speaker_note_summary`를 비교한다.

다음 내용은 화면보다 강사 설명에 있는 것이 적절한지 검토하라.

* 연구의 세부 방법론
* 역사적 배경
* 긴 사례 설명
* 예외조건
* 해석상의 한계
* 연구자 소개
* 세부 용어 정의

반대로 다음 내용은 화면에서 확인할 필요가 있는지 검토한다.

* 핵심 주장
* 핵심 숫자
* 비교 관계
* 단계
* 질문
* Framework 구조

각 슬라이드를 다음 중 하나로 평가한다.

* SHOW / SAY 적절
* SHOW 과다
* SAY 과다
* 핵심 메시지 누락

---

# 6. 정보 밀도를 검수하라

각 슬라이드를 다음으로 분류한다.

### LOW

질문, Statement, Transition, Closing

### MEDIUM

비교, 사례, 간단한 Process

### HIGH

연구 결과, Matrix, Framework, 복잡한 Diagram

전체 순서를 보고 다음을 점검한다.

* HIGH가 3장 이상 연속되는가?
* LOW 슬라이드가 지나치게 많아 내용이 얕게 느껴지는가?
* 중요한 연구가 지나치게 짧게 처리되었는가?
* 설명이 많이 필요한 Framework 뒤에 정리 화면이 있는가?

필요하면 정보 밀도 리듬을 다음과 같이 조정한다.

> HIGH → LOW

또는

> HIGH → MEDIUM → LOW

강의 리듬 차원에서 수정이 필요한 구간을 찾아라.

---

# 7. Research Base와의 근거 정합성을 검수하라

각 Evidence Slide와 핵심 주장에 대해 Research Base를 대조한다.

다음 세 가지를 반드시 구분한다.

### Evidence

연구가 직접 보여준 결과.

### Interpretation

연구를 기반으로 교육자가 해석한 내용.

### Provocation

수강생 사고를 촉진하기 위한 도발적인 표현.

다음 오류를 집중적으로 찾아라.

### Overclaim

연구보다 강하게 주장함.

### Causal Overreach

상관관계 연구를 인과관계처럼 표현함.

### Scope Expansion

특정 조건에서의 결과를 모든 조직·업무에 확대함.

### Citation Mismatch

출처가 실제 주장과 맞지 않음.

### Unsupported Claim

출처가 필요한 주장인데 근거가 없음.

각 문제에 대해

> 기존 표현 → 문제 → 안전한 수정 표현

순으로 제안하라.

---

# 8. 강한 문장을 특히 엄격하게 검수하라

다음과 같은 슬라이드 헤드라인은 교육적으로 강력하지만 과장되기 쉽다.

예:

> “전문가는 무엇을 보지 않아도 되는지 아는 사람이다.”

> “AI는 일반지식의 가격을 떨어뜨린다.”

> “암묵지가 문제가 아니라 한 사람에게만 있는 것이 문제다.”

> “일반지식이 싸질수록 맥락이 비싸진다.”

> “AI는 창의성의 평균은 높이고 다양성은 낮출 수 있다.”

이런 문장들을 모두 추출하라.

각 문장마다 다음을 평가한다.

* 사실 정확성
* 근거 수준
* 교육적 설명력
* 오해 가능성
* 과장 위험

그리고 다음 중 하나로 분류한다.

* 그대로 사용
* 조건을 붙여 사용
* 표현 완화
* 강사 설명에서 한계 보완
* 사용하지 않는 편이 좋음

**강렬함보다 견고함을 우선하라.**

---

# 9. 불필요한 이분법을 검수하라

다음 관계가 지나치게 단순화되고 있지 않은지 확인한다.

* Human vs AI
* Generalist vs Expert
* Tacit vs Explicit
* Human Judgment vs System
* Creativity vs Recombination
* Standardization vs Expertise
* Junior vs Senior

특히

> “AI는 못하지만 인간은 할 수 있다.”

또는

> “AI가 할 수 있으므로 인간은 필요 없다.”

식의 주장이 있는지 찾아라.

필요하다면

> A vs B

를

> A와 B가 서로 다른 조건에서 강점을 가진다

또는

> 연속선 / 역할 분담 / 상호보완

구조로 바꾸어라.

---

# 10. 용어 난이도를 검수하라

다음과 같은 전문용어가 화면에 지나치게 많이 남아 있는지 확인한다.

* Recognition-Primed Decision
* Chunking
* Search Space
* SECI
* Externalization
* Internalization
* Next-token Prediction
* Divergent Thinking
* Convergent Thinking
* Combinatorial Creativity

전문용어마다 다음 질문을 적용한다.

> **“교육생이 이 용어 자체를 기억해야 하는가?”**

NO라면 현상을 먼저 보여주고 용어는 보조로 내려라.

예:

좋지 않은 방식:

> Recognition-Primed Decision Model

더 좋은 방식:

> **숙련자는 모든 선택지를 처음부터 비교하지 않는다.**

작게:

> Recognition-Primed Decision

개념 설명이 교육 목적보다 앞서지 않도록 한다.

---

# 11. 비유와 사고실험을 검수하라

사용 중인 모든 비유를 추출한다.

예:

* Infinite Monkey
* 대리 여러 명 vs 부장 한 명
* 요리사와 레시피
* 초보 운전자와 숙련 운전자
* 100명이 같은 AI를 사용한 상황

각 비유마다 다음을 확인한다.

### Intended Meaning

무엇을 설명하려는가?

### Valid Range

어디까지 설명 가능한가?

### Misinterpretation Risk

어떤 잘못된 해석을 만들 수 있는가?

특히 “대리 vs 부장” 비유가 직급 우열이나 세대 차이로 오해되지 않도록 검수하고, 실제 의도가 **숙련도와 판단 문제**임이 명확한지 확인한다.

비유의 부작용이 핵심 메시지보다 크다면 다른 표현을 제안한다.

---

# 12. Visual Concept가 정말 필요한지 검수하라

각 `visual_concept`에 대해 다음 질문을 적용한다.

> **“이 시각화가 없으면 이해하기 어려운가?”**

시각화는 장식이 아니다.

다음 기준으로 평가한다.

### ESSENTIAL

개념 관계 이해에 반드시 도움됨.

### HELPFUL

이해나 기억에 도움됨.

### DECORATIVE

내용 이해와 관계가 거의 없음.

DECORATIVE로 판단되는 시각화는 삭제를 권고한다.

특히 Framework, Loop, Process, Comparison은 실제 관계가 존재할 때만 사용한다.

---

# 13. 동일한 Visual Pattern의 과사용을 검수하라

다음 구조가 반복되고 있는지 확인한다.

* Before / After
* 2-column comparison
* 3-step process
* Matrix
* Loop
* Statement

같은 구조가 지나치게 반복되면 수강생이 패턴에 무뎌질 수 있다.

다만 단순히 다양성을 위해 표현 형식을 바꾸지는 않는다.

**내용 구조가 같다면 표현도 같아도 된다.**

불필요한 다양화보다 의미의 일관성을 우선한다.

---

# 14. Chapter별 완결성을 검수하라

각 Chapter마다 다음 구조가 존재하는지 확인한다.

### Question

왜 이 내용을 알아야 하는가?

↓

### Discovery

무엇을 새롭게 알게 되는가?

↓

### Proposition

어떤 생각을 가져가야 하는가?

↓

### Transition

왜 다음 Chapter가 필요한가?

각 Chapter를 다음 형식으로 요약하라.

> Question → Discovery → Message → Next Question

이 한 줄을 만들기 어려운 Chapter는 구조가 약한 것으로 판단한다.

---

# 15. Opening을 검수하라

Opening이 다음 역할을 하는지 확인한다.

* 관심을 끈다.
* 강의의 핵심 문제를 제기한다.
* 수강생의 기존 직관을 드러낸다.
* 이후 내용을 궁금하게 만든다.

Opening에서 다음을 과도하게 설명하고 있지 않은지 확인한다.

* 강의 결론
* 암묵지 이론
* LLM 기술
* 조직관리 Framework

Opening은 **문제를 열어야지 닫아서는 안 된다.**

---

# 16. Closing을 검수하라

Closing은 새로운 내용을 추가하지 않아야 한다.

다음을 확인한다.

* Opening 질문을 다시 회수하는가?
* Key Proposition을 통합하는가?
* Knowledge Loop 또는 최종 Framework가 전체 강의를 회수하는가?
* 개인 또는 조직의 행동으로 연결되는가?
* 마지막 문장이 실제로 기억할 가치가 있는가?

Closing에 새로운 이론이나 사례가 등장한다면 본문으로 이동하거나 삭제한다.

---

# 17. Framework의 실무 사용 가능성을 검수하라

최종 Framework가 단순한 예쁜 도식인지, 실제 판단 도구인지 평가한다.

예를 들어 Knowledge Loop가 있다면 수강생이 다음 질문에 답할 수 있어야 한다.

* 어떤 경험을 기록해야 하는가?
* 무엇을 시스템화해야 하는가?
* AI는 어느 단계에서 쓰는가?
* 사람이 직접 판단해야 하는 것은 무엇인가?
* 결과는 어떻게 다시 조직 지식으로 돌아오는가?

Framework를 본 뒤 행동이 달라질 수 없다면 보완한다.

---

# 18. Activity를 검수하라

모든 활동에 대해 다음을 확인한다.

### Learning Objective

왜 이 활동을 하는가?

### Cognitive Load

지시가 너무 복잡하지 않은가?

### Time

강의 시간 안에 가능한가?

### Debrief

활동 후 어떤 메시지를 회수하는가?

특히 활동 자체는 재미있지만 강의 메시지와 연결이 약한 경우 삭제 또는 수정한다.

AI 실습의 경우 AI 사용 능력을 시험하는 활동이 아니라 **강의의 개념을 직접 경험하게 하는 활동**인지 확인한다.

---

# 19. 삭제 테스트를 강하게 적용하라

모든 슬라이드에 다음 질문을 적용한다.

> **“이 장이 없어도 수강생이 같은 결론에 도달할 수 있는가?”**

YES라면 삭제 후보로 표시한다.

다만 다음 목적이라면 유지할 수 있다.

* 질문을 위한 Pause
* Chapter Divider
* Discussion
* Recap
* 강한 메시지를 위한 의도적 여백

삭제 후보마다 다음을 제시하라.

> Slide N
> 유지 가치: 낮음 / 중간 / 높음
> 삭제 시 영향
> 권장 조치

목표는 슬라이드 수를 줄이는 것이 아니라 **필요 없는 인지부하를 줄이는 것**이다.

---

# 20. HTML 제작 준비도를 검수하라

최종 산출물은 HTML 슬라이드 문서다.

따라서 각 Slide Specification이 실제 구현에 충분히 명확한지 확인한다.

필수 항목:

* slide_id
* chapter
* slide_type
* title
* core_message
* visible_content
* visual_concept

선택 항목:

* evidence
* source_id
* speaker_note_summary
* transition

다음 문제가 있는 슬라이드를 찾아라.

### Ambiguous Content

화면에 실제 어떤 문구를 넣어야 하는지 불분명함.

### Visual Ambiguity

시각화해야 하는 관계가 명확하지 않음.

### Missing Data

차트나 표를 요구하지만 실제 데이터가 없음.

### Template Dependency

특정 PPT 배치나 디자인을 전제로 하고 있음.

### Implementation Risk

실제 HTML 구현 시 지나치게 복잡한 인터랙션 또는 특수 기능을 요구함.

HTML/CSS 구현 지시를 새롭게 만들 필요는 없다.

단지 **콘텐츠 명세가 구현 가능한 수준인지** 판단한다.

---

# 21. 템플릿 침범 여부를 확인하라

HTML 디자인 템플릿은 별도로 제공될 예정이다.

따라서 Slide Design Specification 안에 다음과 같은 지시가 있다면 제거 후보로 표시한다.

* 배경색
* 구체적인 색상
* 폰트 이름
* px 단위 크기
* 좌우 배치
* 카드 모양
* 그림자의 종류
* 세부 Grid
* 애니메이션 구현
* Navigation 방식

대신 콘텐츠 차원에서 필요한 관계만 유지한다.

예:

삭제 대상:

> 왼쪽에는 전문가, 오른쪽에는 신입 이미지를 배치한다.

유지:

> 전문가와 초보자의 문제 탐색 방식 차이를 비교한다.

---

# 22. 전체 강의를 Red-Team 방식으로 검토하라

강의에 회의적인 수강생의 입장에서 반론을 제기한다.

최소 다음 질문에 답하라.

* “결국 전문가가 중요하다는 너무 당연한 이야기 아닌가?”
* “LLM도 전문 분야 데이터를 학습하면 전문가를 대체할 수 있지 않은가?”
* “암묵지를 문서화하지 못한다면 조직은 결국 사람에게 의존해야 하는가?”
* “회사 맥락도 결국 데이터화할 수 있지 않은가?”
* “AI가 창의적이라면 인간의 역할을 왜 강조하는가?”
* “Knowledge Loop는 기존 Knowledge Management와 무엇이 다른가?”

각 질문에 대해 교안 내부에서 충분히 답할 수 있는지 확인한다.

답변이 부족하다면 **새 Chapter를 추가하지 말고**, 가장 적절한 기존 슬라이드에 최소한의 보완을 제안한다.

---

# 23. 최종 평가표를 작성하라

전체 교안을 다음 기준으로 5점 만점 평가한다.

| 기준            | 점수 | 판단 근거 |
| ------------- | -: | ----- |
| 핵심 메시지 명확성    |    |       |
| Storyline     |    |       |
| 논리적 연결        |    |       |
| Evidence 정확성  |    |       |
| 과장 통제         |    |       |
| 이해 용이성        |    |       |
| 현업 관련성        |    |       |
| 정보 밀도         |    |       |
| 기억 가능성        |    |       |
| 활동의 적절성       |    |       |
| Framework 유용성 |    |       |
| HTML 구현 준비도   |    |       |

4점 미만인 항목은 반드시 수정안을 제안한다.

---

# 24. 수정 우선순위를 정하라

검수 결과를 다음 세 단계로 분류한다.

## P0 — HTML 제작 전 반드시 수정

예:

* 사실 오류
* 연구 왜곡
* 논리적 단절
* 핵심 메시지 불분명
* 중대한 중복
* 구현할 콘텐츠가 불명확

## P1 — 가능하면 수정

예:

* 정보 밀도 과다
* Transition 약함
* 비유의 오해 가능성
* 표현 과장

## P2 — 선택적 개선

예:

* 제목 표현
* 사례 교체
* 소소한 순서 조정

수정사항을 너무 많이 만들어내지 말고 **최종 결과의 품질에 실제 영향을 주는 문제를 우선한다.**

---

# 25. 최종 판정을 내려라

최종적으로 다음 중 하나를 선택한다.

### READY

현재 상태로 HTML 제작 단계로 진행 가능.

### READY WITH MINOR FIXES

일부 경미한 수정 후 진행 가능.

### REVISION REQUIRED

핵심 논리 또는 근거 문제를 먼저 수정해야 함.

그리고 이유를 5개 이내로 요약한다.

---

# 최종 산출물 형식

다음 순서로 결과를 작성하라.

## A. Executive Review

전체 교안의 상태를 짧게 진단.

## B. Core Message Alignment

Big Question / Final Message / Key Proposition 정합성.

## C. Title-only Narrative Review

모든 슬라이드 제목 및 서사 평가.

## D. Slide-level Review

각 슬라이드:

* PASS
* MODIFY
* MERGE
* SPLIT
* DELETE

중 하나로 표시하고 이유를 적는다.

## E. Evidence Audit

근거 과장·오류·불일치 검수.

## F. Information Density Review

LOW / MEDIUM / HIGH 리듬 검수.

## G. Terminology & Analogy Review

전문용어와 비유의 적절성.

## H. Chapter Review

Question → Discovery → Message → Next Question 구조.

## I. Activity Review

교육 목표와의 정합성.

## J. Framework Review

최종 Framework의 이해도와 실무 적용성.

## K. HTML Readiness Review

실제 HTML 제작 단계에서 모호한 콘텐츠 명세 확인.

## L. Red-Team Questions

회의적인 수강생 관점의 주요 반론과 대응 가능성.

## M. Priority Fix List

P0 / P1 / P2.

## N. Final Scorecard

12개 기준 5점 평가.

## O. Final Verdict

READY / READY WITH MINOR FIXES / REVISION REQUIRED

---

# 가장 중요한 검수 원칙

이 단계에서는 **더 멋진 내용을 추가하려는 유혹을 억제하라.**

검수의 목적은

> **Add**

가 아니라

> **Clarify / Remove / Tighten / Verify**

이다.

다음 우선순위를 따른다.

> 정확성
> ↓
> 논리적 연결
> ↓
> 메시지 명확성
> ↓
> 정보 밀도
> ↓
> 기억 가능성
> ↓
> 시각적 표현

슬라이드가 재미있지만 논리적으로 불필요하다면 삭제를 검토한다.

문장이 강렬하지만 연구보다 강한 주장이라면 표현을 완화한다.

설명이 정확하지만 화면에 너무 많은 정보가 있다면 강사 노트로 이동한다.

최종적으로는

> **“무엇을 더 넣을까?”**

가 아니라

> **“이 상태에서 무엇을 빼거나 고치면 메시지가 더 정확하고 강해지는가?”**

라는 기준으로 검수하라.

아래 자료를 바탕으로 검수 작업을 수행한다.

---

# Research Base

@tacit-knowledge/research-base.md
@tacit-knowledge/research-supplement.md

# Course Architecture

@tacit-knowledge/course-architecture.md

# Teaching Guide

@tacit-knowledge/teaching-script.md

# Slide Design Specification

@tacit-knowledge/slide-design.md

# HTML Template Constraints

@index.html