# AGENTS.md — Solution-First Rules

## Before work
- 현재 저장소, 브랜치, 실행환경, 실제 대상 URL/계정을 먼저 확인한다.
- 이전 채팅 기억보다 현재 파일과 실제 상태를 우선한다.
- 같은 유형의 문제가 있었는지 `KNOWN_SOLUTIONS.md`와 `examples/`를 먼저 찾는다.

## Solution-first rule
아래 말을 하기 전에 대체경로를 먼저 확인한다.
- “PC에서 해야 합니다.”
- “직접 편집기에서 해야 합니다.”
- “수동으로만 가능합니다.”
- “원격으로는 안 됩니다.”
- “이 도구로는 불가능합니다.”

확인 순서:
1. 기존 성공사례 / handoff
2. 플랫폼 기본 설정
3. API / SDK
4. Custom code / Embed / Redirect / Routing
5. Repository / Deployment 설정
6. CLI / Browser automation
7. 마지막에만 수동 작업

## Decision rule
- 사용자의 목표를 먼저 한 문장으로 정의하고 특정 도구에 목표를 묶지 않는다.
- 기존 URL, QR, 데이터, 링크, 사용습관을 유지하는 방법을 우선한다.
- 첫 방법이 막혔다고 바로 불가능 판정을 내리지 않는다.
- 두 번째 시도에서 더 좋은 방법이 나왔다면, 첫 판단의 누락을 기록하고 재발방지 규칙으로 남긴다.

## Verification
- 실제 사용자 흐름까지 확인한다.
- 자동화 성공과 사용자 화면 결과를 별개의 증거로 취급한다.
- 확인하지 않은 것은 “완료”라고 말하지 않는다.
