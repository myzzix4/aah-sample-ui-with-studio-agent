# Sample #2 — UI + Studio Agent

| 차원 | 선택 |
|---|---|
| **UI** | ✅ 직접 개발 Flask |
| **Agent** | ✅ AAH Agent Studio 산출물 (baked ARN) |

UI 만 1 서비스. AAH Agent Studio 에서 만들고 컨테이너 배포(READY)한 Agent 의 ARN을
`AGENT_RUNTIME_ARN` env 로 박으면 끝.

## 배포 절차

1. AAH `/agents` 에서 Agent 빌드 + 컨테이너 배포 → ARN 발급 대기 (READY)
2. `/develop/code-deploy` → 샘플 #2 카드 → Studio Agent 드롭다운에서 선택 → 배포

## 차이 vs #1

- #1: agent도 직접 코드. 2 services
- #2: agent는 Studio 결과물 호출. 1 service. UI 만들기에만 집중

UI templates/static 은 #1 과 동일 (삼성생명 mockup).
