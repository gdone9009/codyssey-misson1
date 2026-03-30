# 🚀 코디세이 미션 1: 개발 워크스테이션 구축

## 📝 학습 기록 (2026-03-30)
오늘의 주요 성과는 로컬 환경과 GitHub을 연결하는 인증 벽을 넘은 것입니다.

### 🛠️ 트러블슈팅: GitHub 인증 오류 (Authentication Failed)
- **문제**: `git push` 시 ID/PW를 입력해도 인증 실패 발생.
- **원인 가설**: GitHub의 보안 정책 변경으로 인해 일반 비밀번호 사용이 중단됨.
- **확인**: 터미널 에러 로그 및 공식 문서 확인.
- **해결**: 
  1. macOS 키체인 접근에서 기존 GitHub 정보 삭제.
  2. GitHub에서 Personal Access Token(Classic) 생성 (repo 권한 부여).
  3. 비밀번호 대신 토큰(`ghp_...`)을 입력하여 인증 성공.
- **결과**: `readme.md` 최초 Push 성공!
