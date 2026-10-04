# Solution-First Starter

처음부터 가능한 해결 경로를 넓게 확인하고, **PC-only / 수동-only / 불가능** 결론을 너무 일찍 내리지 않도록 하는 재사용형 작업 스타터킷입니다.

## 누구를 위한 건가
- ChatGPT / Claude / Codex와 같이 개발·운영 작업을 하는 사람
- 다른 PC나 다른 개발자가 이어받아도 같은 시행착오를 줄이고 싶은 팀
- 웹사이트, 배포, API, 자동화, 리다이렉트, 운영도구 작업을 자주 하는 사람

## 가장 쉬운 사용법
1. 이 저장소에서 **Use this template** → **Create a new repository**를 누릅니다.
2. 자기 GitHub 계정에 새 프로젝트를 만듭니다.
3. 새 프로젝트를 ChatGPT / Claude / Codex / 개발자에게 열어줍니다.
4. 첫 지시는 이렇게 합니다.

> 먼저 START_HERE.md와 AGENTS.md를 읽고, 이 프로젝트의 작업규칙을 따라줘.  
> 어떤 작업을 PC-only/수동-only라고 결론 내리기 전에 CHECKLIST.md의 대체 경로를 먼저 확인해줘.

그 다음부터는 자기 프로젝트 파일을 추가하며 작업하면 됩니다.

## 들어있는 파일
- `START_HERE.md` — 처음 시작할 때 읽는 1페이지
- `AGENTS.md` — AI/개발자가 따라야 할 공통 작업 규칙
- `CHECKLIST.md` — “안 된다 / PC가 필요하다”라고 말하기 전 확인표
- `KNOWN_SOLUTIONS.md` — 재사용 가능한 검증 해결법 기록 양식
- `PROMPT_FOR_AI.md` — AI에게 복붙할 시작 프롬프트
- `examples/wix-external-redirect.md` — 실제 Wix → 외부 사이트 직통 사례

## 핵심 원칙
**목표를 먼저 정의하고, 도구는 나중에 고릅니다.**

예:
- 나쁜 정의: “집 PC에서 Wix 편집기를 열어야 한다.”
- 좋은 정의: “기존 URL과 QR은 유지하면서 방문자를 새 사이트로 바로 보내야 한다.”

좋은 정의를 한 뒤 다음 경로를 확인합니다.

**기존 성공사례 → 플랫폼 설정 → API/SDK → 코드/Embed/Redirect → 배포설정 → CLI/브라우저 자동화 → 마지막에 수동작업**

