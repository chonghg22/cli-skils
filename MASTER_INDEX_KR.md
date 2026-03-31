# MASTER_INDEX_KR

## 목적
이 문서는 `/skils` 아래에 모아둔 여러 오픈소스 CLI skill을 한국어로 빠르게 분류해서, 어떤 상황에 어떤 폴더를 열어야 하는지 판단하기 쉽게 만든 전체 안내서입니다.

## 가장 먼저 보는 빠른 선택표

### 1. 구현 전에 방향부터 정리하고 싶다
- `brainstorming`
설계, 요구사항, 접근법 비교, 승인용 문서 정리에 적합합니다.

### 2. 이미 계획이 있고 그대로 실행하면 된다
- `executing-plans`
작성된 구현 계획을 순서대로 실행할 때 적합합니다.

### 3. 구현 계획이 있고, 독립 태스크를 병렬로 빠르게 처리하고 싶다
- `subagent-driven-development`
서브에이전트 기반 병렬 개발과 리뷰 루프에 적합합니다.

### 4. 현재 작업 공간을 건드리지 않고 안전하게 새 브랜치 작업 공간을 만들고 싶다
- `using-git-worktrees`
독립 worktree 생성, 테스트 가능한 깨끗한 시작점 확보에 적합합니다.

### 5. 코드 구조와 설계 품질 자체를 끌어올리고 싶다
- `ddd`
DDD, Clean Architecture, SOLID 기준으로 코드 구조를 개선할 때 적합합니다.

### 6. 웹사이트 품질을 종합 점검하고 싶다
- `audit-website`
SEO, 성능, 접근성, 보안, 콘텐츠 문제를 진단할 때 적합합니다.

### 7. Git 커밋을 바탕으로 릴리스 노트나 변경사항 문서를 만들고 싶다
- `changelog-generator`
커밋 이력을 사용자 친화적인 changelog로 정리할 때 적합합니다.

### 8. 내 컴퓨터 파일/폴더를 정리하고 싶다
- `file-organizer`
다운로드 폴더 정리, 중복 파일 탐색, 폴더 구조 개선에 적합합니다.

### 9. Linear 이슈를 관리하고 싶다
- `linear-cli-skill-main`
가볍고 단순한 CLI 중심 Linear 조작에 적합합니다.
- `linear-claude-skill-main`
프로젝트, 라벨, 설명 품질까지 포함한 본격적인 Linear 운영에 적합합니다.

### 10. PostgreSQL 데이터를 읽기 전용으로 조회하고 싶다
- `postgres`
테이블, 스키마, 샘플 데이터를 안전하게 조회할 때 적합합니다.

### 11. PostgreSQL/Supabase 성능 튜닝 기준이 필요하다
- `supabase-postgres-best-practices`
쿼리, 인덱스, RLS, 커넥션 관리 모범 사례를 참고할 때 적합합니다.

### 12. 외부 API를 LLM이 쓸 수 있는 MCP 서버로 만들고 싶다
- `mcp-builder`
MCP 서버 설계, 구현, 평가 기준 정리에 적합합니다.

### 13. 특수한 실험용 보조 기능이 필요하다
- `superpowers-lab-main`
중복 함수 탐지, MCP CLI, tmux 자동화, Windows VM 같은 실험적 도구 모음입니다.

## 상황별 추천

### 새 기능을 만들고 싶다
1. `brainstorming`
2. `using-git-worktrees`
3. `executing-plans` 또는 `subagent-driven-development`
4. 필요하면 `ddd`

### 이미 요구사항은 정해졌고 바로 개발하고 싶다
1. `using-git-worktrees`
2. `executing-plans`
3. 태스크가 잘 나뉘면 `subagent-driven-development`

### 코드가 돌아가긴 하지만 구조가 불안하다
1. `ddd`
2. 필요하면 `subagent-driven-development`

### 운영 중인 웹서비스를 점검하고 싶다
1. `audit-website`
2. DB 원인 분석이 필요하면 `postgres`
3. 성능 원칙 검토는 `supabase-postgres-best-practices`

### DB를 직접 확인하거나 튜닝하고 싶다
1. 데이터 조회는 `postgres`
2. 성능 기준 검토는 `supabase-postgres-best-practices`

### 업무 관리 도구로 Linear를 쓰고 있다
- 빠른 조회/생성/수정은 `linear-cli-skill-main`
- 운영 규칙 포함 관리까지 하려면 `linear-claude-skill-main`

### 배포 문서나 릴리스 노트를 만들어야 한다
- `changelog-generator`

### 개발 외에 로컬 파일 정리가 필요하다
- `file-organizer`

## 비슷해서 헷갈리는 폴더 차이

### `executing-plans` vs `subagent-driven-development`
- `executing-plans`: 정해진 계획을 순서대로 차분히 실행
- `subagent-driven-development`: 독립 작업을 나눠 병렬로 빠르게 실행

### `linear-cli-skill-main` vs `linear-claude-skill-main`
- `linear-cli-skill-main`: 가볍고 단순한 CLI 조작
- `linear-claude-skill-main`: 설명, 라벨, 프로젝트 배정까지 포함한 운영형 관리

### `postgres` vs `supabase-postgres-best-practices`
- `postgres`: 실제 데이터 조회 도구
- `supabase-postgres-best-practices`: 성능/설계 기준서

### `brainstorming` vs `ddd`
- `brainstorming`: 구현 전 아이디어와 요구사항 정리
- `ddd`: 구현 구조와 품질 원칙 정립

## 폴더별 한 줄 가이드
- `audit-website`: 웹사이트 품질 진단
- `brainstorming`: 구현 전 설계와 요구사항 정리
- `changelog-generator`: 커밋 기반 변경사항 문서 생성
- `ddd`: 도메인 중심 설계와 코드 품질 기준
- `executing-plans`: 계획서 기반 순차 실행
- `file-organizer`: 파일과 폴더 정리
- `linear-cli-skill-main`: 가벼운 Linear CLI 작업
- `linear-claude-skill-main`: 본격적인 Linear 운영 관리
- `mcp-builder`: MCP 서버 설계/구현 가이드
- `postgres`: 읽기 전용 Postgres 조회
- `subagent-driven-development`: 병렬 개발 실행
- `supabase-postgres-best-practices`: Postgres 최적화 기준
- `superpowers-lab-main`: 실험적 보조 스킬 모음
- `using-git-worktrees`: 분리된 Git 작업 공간 생성

## 추천 사용 순서 예시

### 기능 개발
`brainstorming` -> `using-git-worktrees` -> `executing-plans` 또는 `subagent-driven-development`

### 구조 개선
`ddd` -> `using-git-worktrees` -> `subagent-driven-development`

### 웹서비스 점검과 개선
`audit-website` -> 코드 수정 -> 재점검

### DB 확인과 성능 개선
`postgres` -> `supabase-postgres-best-practices`

## 참고
각 폴더 안에는 개별 한국어 설명 파일 `INDEX_KR.md`를 추가해두었습니다. 세부 용도는 해당 폴더의 `INDEX_KR.md`를 먼저 보면 됩니다.
