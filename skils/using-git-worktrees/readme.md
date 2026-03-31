용도
- 메인 브랜치를 건드리지 않고 새 기능을 실험 할 때
- 여러 작업을 동시에 독립된 환경에서 진행하고 싶을 때

기능
1. worktree 디렉토리 자동 탐지 (.worktrees/ > worktrees/ > CLAUDE.md > 사용자 질문)
2. .gitignore 포함 여부 안전 검증
3. 프로젝트 타입 자동 감지 후 의존성 설치
4. 베이스라인 테스트 실행 및 결과 보고
5. executing-plans, subagent-driven-development 스킬과 연동