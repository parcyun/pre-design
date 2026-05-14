---
name: pre-design
description: Pre-injection discovery protocol applying Open Design's 4 mechanisms (Discovery Form, Direction Picker, Anti-AI-slop Guardrails, 5-Dim Self-Review) BEFORE any visual design work. MUST auto-trigger for ANY visual deliverable request — HTML pages, landing pages, posters, PPT/PPTX decks, slides, social cards, 카드뉴스, 썸네일, 인포그래픽, dashboards, UI components, Instagram cards, portfolio pages, menu designs, lecture slides — or anything described as 디자인해줘, design, make it pretty, 예쁘게, 감각있게, 스타일, make/create/build a [visual thing]. Runs FIRST, then hands off to brand skills (parcyun-studio, MDBF) or proceeds with the selected direction. Does NOT skip — short requests get a compressed 30-second form. Cost of one wrong-direction round is one chat turn; cost of skipping discovery is a finished artifact that has to be remade.
---

# Pre-Design Protocol

디자인 작업에서 가장 비싼 실수는 "잘못된 방향으로 끝까지 만든 뒤 다시 시작"이다. 건축에서 도면 없이 콘크리트를 붓지 않듯, 픽셀 그리기 전에 방향을 확정한다. **30초의 질문이 30분의 수정을 막는다.**

이 스킬은 4단계 프로토콜이다. 디자인 작업 시작 시 1→2→3→4 순서로 실행.

---

## 단계 1 · Discovery 폼 (Turn 1, 코드 작성 금지)

질문 없이 그리지 않는다. 다음 6개 항목을 한 번에 묻는다. 이미 컨텍스트에 있는 항목은 생략하고, 빠진 부분만 짧게 물어본다.

```
1. 매체     · 무엇? (랜딩페이지 / 포스터 / 슬라이드 / 카드 / 문서)
2. 대상     · 누가 보는가? (학생 / 동료 / 클라이언트 / 대중)
3. 톤       · 어떤 인상? (전문 / 친근 / 럭셔리 / 발랄 / 미니멀)
4. 브랜드   · parcyun studio / MDBF / 외부 / 새 컨셉
5. 규모     · 페이지·슬라이드 수, 크기
6. 제약     · 마감일, 필수 색상·폰트·요소
```

답이 짧아도 OK. 라디오 버튼 속도로 받는다. 사용자가 이미 충분히 설명한 경우(예: "내 studio 스타일로 v2 수정") 1-2단계는 압축 가능하지만 **3-4단계는 항상 실행**.

---

## 단계 2 · 방향 선택 (브랜드 미지정 시에만)

단계 1에서 브랜드가 확정되면(`parcyun studio`, `MDBF` 등) 이 단계 스킵하고 해당 브랜드 스킬로 바로 인계.

브랜드가 없거나 "새 컨셉"이면 5개 학파 중 사용자가 하나 선택:

| 방향 | 무드 | 적합한 경우 |
|---|---|---|
| **Editorial** | 매거진풍, 따뜻한 잉크 톤 | 큐레이션, 갤러리, 에세이 |
| **Modern Minimal** | Linear·Vercel풍, 차가운 미니멀 | SaaS, 대시보드, 문서 |
| **Tech Utility** | 모노스페이스, 정보 밀도 | 개발자 도구, 데이터 표시 |
| **Brutalist** | 거대 타입, 그림자 없음, 강한 색 | 임팩트, 어그로, 실험 |
| **Soft Warm** | 낮은 대비, 복숭아 뉴트럴 | 교육, 헬스케어, 라이프스타일 |

선택 후 팔레트 + 폰트 스택을 **결정론적으로 고정**. AI 자유 재량 금지.

---

## 단계 3 · Anti-AI-slop 금지 목록 (작성 중 자가검열)

AI가 무의식적으로 만드는 흔한 함정. 작성 중 다음 패턴이 보이면 멈추고 다시.

**금지 패턴:**
- 보라색 그라디언트 (특히 `#667eea → #764ba2` 류 디폴트 톤)
- 일반 이모지를 UI 아이콘 대용으로 (🚀 ✨ 💎)
- 왼쪽 컬러 테두리가 있는 둥근 카드 (블로그·포트폴리오 클리셰)
- Display 폰트로서의 Inter (본문은 OK, 큰 헤드라인은 다른 폰트)
- 손으로 그린 듯한 SVG 인물 일러스트
- 허구의 지표 ("10배 빠릅니다", "98% 만족도")
- 의미 없는 글래스모피즘 남용

**대체:**
- 그라디언트 대신 단색 + 미세 텍스처 / 노이즈
- 이모지 대신 라인 아이콘 (Lucide, Heroicons, Phosphor)
- 허구 숫자 대신 `—` 또는 회색 placeholder 블록
- Display용 폰트: Space Grotesk, Cabinet Grotesk, Clash Display 등

---

## 단계 4 · 5차원 자기 검토 (출력 직전 필수)

최종 파일·아티팩트 출력 직전, 다음 5개 축에서 1-5점으로 자가 채점. **평균 3.0 미만이면 수정 후 재채점.**

| 차원 | 평가 기준 |
|---|---|
| **철학** Philosophy | 디자인 결정에 "왜"가 있는가? 일관된 미적 입장이 있는가? |
| **계층** Hierarchy | 시각적 위계 명확? 가장 중요한 것이 가장 눈에 띄는가? |
| **실행** Detail | 간격·정렬·타이포 디테일 정확? |
| **기능** Function | 사용자가 다음 행동을 취할 수 있는가? CTA 명확? |
| **절제** Restraint | 불필요한 요소 없는가? 과잉 장식 제거됐나? |

채점은 내부적으로 수행. **통과(평균 3.0 이상) 시 조용히 출력 — 채점 결과를 사용자에게 노출하지 않는다.** 미달 시에만 "한 가지 다듬을 곳이 있어 한 번 수정했어요" 정도로 짧게 알리고 출력. 인지 부하를 줄이는 게 채점의 가시성보다 우선.

---

## 다른 스킬과의 관계

이 스킬은 **사전 단계**다. 단계 2에서 브랜드가 결정되면 다음 스킬로 자동 인계:

- `parcyun studio` 선택 → `parcyun-studio` 스킬 (#FFB11A, Montserrat Light + Pretendard, Toss-Liquid)
- `MDBF` 선택 → MDBF 컨텍스트 (#3364D9)
- 그 외 방향 선택 → 단계 2에서 확정된 토큰으로 진행

순서:
```
1. pre-design 단계 1·2 → 방향 확정
2. 브랜드 스킬 또는 단계 2 토큰 → 실제 작업
3. pre-design 단계 3 (작성 중 자가검열)
4. pre-design 단계 4 (출력 직전 5차원 채점) → 완료
```

---

## 컨텍스트별 발동 강도

| 상황 | 발동 강도 |
|---|---|
| 새 디자인 요청 | 전체 1→2→3→4 실행 |
| 기존 디자인 수정 (v2, v3) | 1·2 압축 (변경점만 확인), 3·4는 실행 |
| 매우 짧은 요청 ("이거 좀 예쁘게") | 1번을 3개 항목으로 압축 (매체·톤·제약), 2는 스킵 가능, 3·4 실행 |
| 사용자가 "그냥 만들어줘" 강조 | 1·2 스킵하되 가정한 방향을 한 줄로 명시 후 진행, 3·4는 항상 실행 |

3·4단계는 **절대 스킵하지 않는다.** 이게 AI-slop과 디자이너 결과물을 가르는 선이다.
