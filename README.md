# pre-design

Claude Skill — 시각 디자인 작업 전 **방향을 먼저 확정**하는 4단계 프로토콜.

> 건축에서 도면 없이 콘크리트를 붓지 않듯, 픽셀을 그리기 전에 방향을 확정한다.
> **30초의 질문이 30분의 수정을 막는다.**

---

## 무엇을 해결하는가

AI 디자인 작업에서 가장 비싼 실수는 "잘못된 방향으로 끝까지 만든 뒤 다시 시작"이다. 이 스킬은 그 비용을 사전 차단하기 위해 4가지 메커니즘을 강제 실행한다.

| 단계 | 메커니즘 | 목적 |
|---|---|---|
| 1 | **Discovery 폼** | 매체·대상·톤·브랜드·규모·제약 6개 항목 확정 |
| 2 | **방향 선택** | Editorial / Modern Minimal / Tech Utility / Brutalist / Soft Warm 중 결정론적 고정 |
| 3 | **Anti-AI-slop 가드레일** | 보라색 그라디언트, 이모지 아이콘 등 흔한 함정 차단 |
| 4 | **5차원 자기 검토** | 철학·계층·실행·기능·절제 5축 자가 채점 (평균 3.0↑ 통과) |

추가로 디자인 전에 `핵심 행동`과 `완료 기준`을 고정한다. 결과물이 보기 좋은지뿐 아니라 사용자가 무엇을 해야 하고, 무엇을 확인하면 끝인지까지 정의한다.

---

## 트리거 조건

다음 요청에서 자동 발동:

- HTML 페이지, 랜딩페이지, 포스터, PPT/PPTX, 슬라이드
- 카드뉴스, 썸네일, 인포그래픽
- 대시보드, UI 컴포넌트, 인스타그램 카드
- "디자인해줘", "예쁘게", "감각있게", "스타일"
- `make/create/build a [visual thing]`

요청이 짧으면 30초 압축 폼으로, 길면 전체 4단계로 자동 조정.

## 사용 순서

1. 이미 알려진 항목은 생략하고 Discovery에서 빠진 정보만 확인한다.
2. 브랜드가 없으면 방향 하나와 최소 토큰을 고정하고, 브랜드가 있으면 해당 브랜드 스킬로 인계한다.
3. 구현 중 Anti-AI-slop 목록과 실제 데이터·접근성·동작 제약을 확인한다.
4. 출력 직전 5차원 자기 검토를 수행한다. 평균 3점 미만이거나 기능/접근성이 2점 이하이면 수정한다.
5. 결과 보고에서 구현·검증·미검증 상태를 구분한다.

답이 없을 때는 되돌릴 수 있는 가정을 한 줄로 기록하고 진행한다. 인증, 개인정보, 결제, 배포, 삭제처럼 영향이 큰 결정은 추측하지 않는다.

---

## 다른 스킬과의 관계

이 스킬은 **사전 단계(pre-injection)**다. 방향이 확정되면 다음 스킬로 자동 인계:

- `parcyun studio` 선택 → `parcyun-studio` 스킬 (#FFB11A, Montserrat Light + Pretendard)
- `MDBF` 선택 → MDBF 컨텍스트 (#3364D9)
- 그 외 → 단계 2에서 확정된 토큰으로 진행

3·4단계는 **절대 스킵하지 않는다.** 이게 AI-slop과 디자이너 결과물을 가르는 선이다.

자세한 실행 규칙은 [`SKILL.md`](./SKILL.md)를 참조한다.

---

## 설치

Claude Desktop / Claude.ai의 Skills 폴더에 `SKILL.md`를 배치:

```
~/.claude/skills/pre-design/SKILL.md
```

또는 Anthropic Skills 시스템의 사용자 스킬 경로에 클론:

```bash
git clone https://github.com/<your-username>/pre-design.git
```

---

## 라이선스

MIT License. 자세한 내용은 [`LICENSE`](./LICENSE) 참조.

---

<sub>Designed by **parcyun studio** · [@parcyun](https://www.instagram.com/parcyun)</sub>
