---
name: readme-skill
description: Generate or update a README.md for the current project
user-invocable: true
---

# readme-skill

현재 프로젝트의 README.md를 생성하거나 업데이트할 때 사용하는 스킬입니다.

TRIGGER when: 사용자가 "README 만들어줘", "README 작성해줘", "README 업데이트해줘" 또는 `/readme`를 사용할 때.

## 지침

이 스킬이 실행되면:

1. 프로젝트 구조를 탐색하여 다음을 파악합니다:
   - 프로젝트의 목적과 주요 기능
   - 기술 스택 및 의존성 (`package.json`, `pyproject.toml`, `go.mod` 등 확인)
   - 기존 문서나 코드 주석

2. 다음 섹션으로 구성된 README.md를 생성합니다:
   - **제목** — 프로젝트 이름과 한 줄 설명
   - **개요** — 문제 인식, 해결방법, 프로젝트 소개
   - **멤버** - 개인 프로젝트의 경우 dellyu03만 표시 팀 프로젝트의 경우 팀 구성원 및 정보, 역할
   - **기술스택** - github 배치 형태로 구획을 나눠서 작성
   - **시작하기** — 사전 요구사항 및 설치 방법
   - **사용법** — 실행 방법과 예시
   - **프로젝트 구조** — 주요 디렉토리/파일 설명 (복잡한 경우)
   - **기여하기** — 기여 방법 (해당하는 경우)
   - **라이선스** — 라이선스 정보 (해당하는 경우)

3. 프로젝트에 맞게 섹션을 조정합니다. 해당하지 않는 섹션은 생략합니다.

4. 명확하고 간결하게 작성합니다. 불필요한 문구는 사용하지 않습니다.

## 사용 예시

- `이 프로젝트 README 만들어줘`
- `README 작성해줘`
- `/readme`
- `새로운 기능을 반영해서 README 업데이트해줘`


5. 상세 템플릿은 아래 경로를 참조
- reference/ex-README.md