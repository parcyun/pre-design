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

---

## 트리거 조건

다음 요청에서 자동 발동:

- HTML 페이지, 랜딩페이지, 포스터, PPT/PPTX, 슬라이드
- 카드뉴스, 썸네일, 인포그래픽
- 대시보드, UI 컴포넌트, 인스타그램 카드
- "디자인해줘", "예쁘게", "감각있게", "스타일"
- `make/create/build a [visual thing]`

요청이 짧으면 30초 압축 폼으로, 길면 전체 4단계로 자동 조정.

---

## 다른 스킬과의 관계

이 스킬은 **사전 단계(pre-injection)**다. 방향이 확정되면 다음 스킬로 자동 인계:

- `parcyun studio` 선택 → `parcyun-studio` 스킬 (#FFB11A, Montserrat Light + Pretendard)
- `MDBF` 선택 → MDBF 컨텍스트 (#3364D9)
- 그 외 → 단계 2에서 확정된 토큰으로 진행

3·4단계는 **절대 스킵하지 않는다.** 이게 AI-slop과 디자이너 결과물을 가르는 선이다.

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
