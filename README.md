# web-starter-autogongbang

오토공방(AutoGongbang) 팀 내부용 Claude Code 플러그인.
"웹페이지 만들어줘" 한마디로 새 웹 프로젝트를 자동 스캐폴드합니다.

---

## 무엇을 해주나요?

사용자가 Claude Code에서 다음과 같은 말을 하면 자동 발동:

- "웹페이지 만들어줘"
- "랜딩페이지 만들어줘"
- "html로 빼줘"
- "사이트 만들어줘"

그러면 이 스킬이:

1. **결과물 유형 분류** — 단일 HTML / Next.js 정적 / 풀스택 SaaS 중 무엇인지 질문
2. **핵심 의도 파악** — 톤, 타겟, 분량 등 짧은 인터뷰
3. **자동 스캐폴드** — 폴더 구조 + 시작 파일 + 디자인 토큰 + CLAUDE.md 자동 생성
4. **디자인 원칙 자동 주입** — AI 슬롭 회피 체크리스트 적용

---

## 설치 방법

Claude Code CLI에서 실행:

```bash
/plugin marketplace add opalgongbang/web-starter-autogongbang
/plugin install web-starter@autogongbang-tools
```

설치 후 Claude Code를 재시작하면 끝.

---

## 사용 방법

설치 후에는 그냥 평소처럼 말하면 됩니다:

```
> 웹페이지 하나 만들어줘
```

→ 스킬이 자동으로 발동해서 인터뷰부터 시작합니다.

---

## 포함된 디자인 토큰 프리셋

`tokens/` 폴더에 3종 톤 프리셋이 들어 있어요:

| 프리셋 | 설명 |
|--------|------|
| `neutral.css` | 무채색 차분한 톤 |
| `yellow-black.css` | 오토공방 브랜드 (노랑 + 블랙) |
| `naverblog.css` | 네이버 블로그 스타일 |

스캐폴드 시점에 어떤 톤으로 갈지 선택할 수 있습니다.

---

## 업데이트

플러그인은 GitHub에 새 커밋이 push되면 Claude Code가 자동으로 가져옵니다.
수동 업데이트가 필요하면:

```bash
/plugin update web-starter@autogongbang-tools
```

---

## 문의

오토공방 내부 플러그인 — 사용 중 문제 있으면 오공에게 직접 문의.
