<p align="center">
  <img width="852" height="148" alt="monew" src="https://github.com/user-attachments/assets/98ab2834-7986-45a4-8b8e-e59660d1dcf1" />
</p>

# Monew
**Monew**는 여러 뉴스 API를 통합하여 사용자 맞춤 뉴스를 제공하고, 사용자 활동 내역 및 의견을 기록/관리할 수 있는 플랫폼입니다.

PostgreSQL과 MongoDB 기반으로 데이터를 안전하게 저장하고, Spring Batch로 뉴스 백업/수집을 자동화하며, Spring Actuator와 Prometheus를 통한 모니터링을 지원합니다.

---

## 📆 개발 기간 <a id="dev-period"></a>
- **기간:** 2025.10.17 ~ 2025.11.10
- **목적:** 뉴스 API 통합 및 맞춤형 뉴스 제공, 활동/의견 관리
- **특징:**
  - PostgreSQL + MongoDB 기반 데이터 안정성
  - Spring Batch로 뉴스 수집/백업 자동화
  - Spring Actuator + Prometheus 모니터링
  - 대용량 데이터 처리와 안정성 고려한 설계
 
---

## 📚 Table of Contents <a id="table-of-contents"></a>
- [프로젝트 소개](#Monew)
- [개발 기간](#dev-period) 
- [개발 환경](#dev-env)
- [기술 스택](#tech-stack)
- [레포지토리 구성](#repo-structure)
- [커밋 컨벤션](#commit-convention)
- [팀원 구성](#team-members)
- [API 문서](#api-문서)
- [협업 문서](#collab-docs)

## 🖥️개발 환경 <a id="dev-env"></a>
- Version : Java 17
- IDE: IntelliJ
- Framwork: SpringBoot 3.5.6 springBoot admin 3.5.0
- ORM : Spring Data JPA + Hibernate

---

## ⚙️기술 스택 <a id="tech-stack"></a>
- Server/Deployment: AWS EC2 github Actions
- DataBase : PostgreSQL (RDS), MongoDB Atlas
- WS/WAS : Tomcat, Spring Boot Admin
- Storage : AWS S3
- Monitoring
- 아이디어 회의 : Notion, git/github, Discord, zep

---

## 🗂️ 레포지토리 구성 <a id="repo-structure"></a>
| Repo | 설명 |
|------|------|
|  [monew-mvc](https://github.com/sb05-monew-team3/monew-mvc.git)  | 메인 API 서버 (Spring Boot MVC) | |
|[monew-batch](https://github.com/sb05-monew-team3/monew-batch.git)  | 뉴스 수집 및 백업 Batch 서비스 ||
| [monew-actuator](https://github.com/sb05-monew-team3/monew-actuator.git) | 모니터링 및 상태 관리 서비스 ||

---

## 🧾 커밋 컨벤션 <a id="commit-convention"></a>
### 기본 구조
```terminal
<type>(<scope>): <subject>

<body>

<footer>
``` 
> **예시:**
> `feat(UserService) : add login method

### Type 분류류
| 타입 | 설명 |
| ---- | -----|
| feat | 새로운 기능 추가 |
| fix  | 버그 수정 |
| docs | 문서 수정 |
| style | 코드 스타일 변경(포매팅, 세미콜론 등) |
| design | UI / CSS 디자인 변경 |
| test | 테스트 코드 관련 변경 |
| refactor | 리펙토링(동작 변화 없음) |
| build | 빌드 파일 수정 |
| ci | CI 설정 수정 |
| perf | 성능 개선
| chore | 자잘한 수정, 설정 변경 |
| rename  | 파일/폴더명 변경 |
| remove | 파일 삭제 |

### Scope
- 변경된 기능 또는 모듈명을 명시합니다.

### Subject 작성 규칙
- 첫 글자는 소문자로 지정합니다.
- 문장 마침표(`.`) 사용 금지.
- 50자 이하로 간결하게 작성합니다.
- "무엇을" 했는지 중심으로, **명령형 동사 원형** 사용
  - ✅ `add`, `update`, `fix`, `remove`, `refactor`
  - ❌ `added`, `fixed`

### Body 작성 규칙
- 각 줄은 **72자 이하**로 작성합니다.
- "무엇을" 변경했는지보다는 **왜 변경했는지(이유)** 중심으로 작성합니다.

### Footer 작성규칙
- 관련 이슈 번호 또는 참고 링크를 명시합니다.

---

## 👥 팀원 구성 <a id="team-members"></a>
| 이름 | 역할 | GitHub |
|------|------|--------|
| 정기주 | 팀장 / 배치 및 데이터 관리 담당| [GitHub](https://github.com/jeonggiju) |
| 김용희 | 사용자 관리 및 활동 담당 | [GitHub](https://github.com/backKim1024) |
| 민재영 | 뉴스 콘텐츠 관리 담당 | [GitHub](https://github.com/jymin0) |
| 박지석 | 관심사 콘텐츠 관리 담당 | [GitHub](https://github.com/commicat2) |
| 이성훈 | 알림 및 시스템 구조 담당 | [GitHub](https://github.com/polodumbo) |
| 주세훈 | 댓글 및 QA 담당 | [GitHub](https://github.com/Jusehun) |

---

## API 문서 <a id="api-docs"></a>
- [Swagger UI ↗](http://sprint-project-1196140422.ap-northeast-2.elb.amazonaws.com/sb/monew/api/swagger-ui/index.html)

---

## 협업 문서 <a id="collab-docs"></a>
- [Notion ↗](https://polydactyl-pufferfish-876.notion.site/MoNew-28e08cfefb45803ebd28ffcd05a97b2e?source=copy_link)
