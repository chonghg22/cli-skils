# INDEX_KR

## 한 줄 설명
실험적이지만 유용한 여러 보조 스킬을 묶어둔 실험실 성격의 컬렉션입니다.

## 언제 쓰면 되나
- 정식 기본 스킬 외에 특수한 작업 보조 도구가 필요할 때
- 코드 중복 탐지, MCP CLI 사용, tmux 기반 상호작용, Windows VM 같은 특수 목적이 있을 때
- 아직 다듬어지는 중인 기능을 시험적으로 써보고 싶을 때

## 포함된 주요 하위 스킬
- `finding-duplicate-functions`: 의미상 중복되는 함수 찾기
- `mcp-cli`: MCP 서버를 일회성으로 CLI에서 탐색/호출
- `using-tmux-for-interactive-commands`: 대화형 CLI 도구 제어
- `windows-vm`: 터미널 기반 Windows VM 준비/접속

## 이런 상황에 특히 적합
- LLM이 만든 코드베이스에서 비슷한 함수가 중복 구현된 흔적 찾기
- MCP를 정식 연결하기 전에 기능만 빠르게 시험
- `vim`, `rebase -i`, REPL 같은 상호작용 도구 자동화
- Windows 환경 재현이 필요한 테스트

## 이럴 때는 다른 폴더가 더 맞음
- 일반적인 구현 계획 실행은 `executing-plans` 또는 `subagent-driven-development`
- Git 작업 격리는 `using-git-worktrees`

## 빠른 예시
- 코드베이스 중복 함수 감사
- 일회성 MCP 호출
- 헤드리스 Windows 테스트 환경 준비

## 메모
- 실험적 성격이 있으므로 안정성보다 유연성과 확장성에 가깝습니다.
