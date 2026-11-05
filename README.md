# MARCH BE

MARCH의 계정·저장 API와 작업 실행을 담당합니다. [프로젝트 기획·디자인](https://github.com/hodomaroo/FE) · [AI](https://github.com/hodomaroo/AI) · [개발 흐름](CONTRIBUTING.md)

## 책임

- 인증·세션, 사용자별 URL 접수·검색·편집·삭제, Instagram Webhook과 연결 승인.
- DB의 사용자 격리, 중복 저장 방지, 작업 lease, 삭제 후 늦게 도착한 결과 차단.
- 권한 있는 원문을 AI 경계로 전달하고, 분석 예산 예약과 실제 사용량 정산.

현재 파일럿은 FastAPI·SQLite·독립 Python Worker로 실행됩니다. 이 저장소에는 개발 흐름과 담당 범위를 먼저 배치했습니다. 코드를 옮길 때는 API와 인증 계약을 FE와 맞추고, HTTP·재시작·사용자 격리 검사를 CI에 연결합니다.
