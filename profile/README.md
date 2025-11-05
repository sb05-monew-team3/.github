<p align="center">
  <img width="852" height="148" alt="monew" src="https://github.com/user-attachments/assets/98ab2834-7986-45a4-8b8e-e59660d1dcf1" />
</p>

## About

Monew는 여러 뉴스 API를 통합하여 사용자 맞춤 뉴스를 제공하고, 사용자 활동 내역 및 의견을 기록/관리할 수 있는 플랫폼입니다.  
PostgreSQL과 MongoDB 기반으로 데이터를 안전하게 저장하고, Spring Batch로 뉴스 백업/수집을 자동화하며, Spring Actuator와 Prometheus를 통한 모니터링을 지원합니다.

## Table of Contents

- [프로젝트 소개](#프로젝트-소개)
- [팀원 구성](#팀원-구성)
- [기술 스택](#기술-스택)
- [레포지토리 구성](#레포지토리-구성)
- [브랜치 전략](#브랜치-전략)
- [커밋 컨벤션](#커밋-컨벤션)
- [프로젝트 구조](#프로젝트-구조)
- [팀원별 구현 예정 기능](#팀원별-구현-예정-기능)
- [API 문서](#api-문서)
- [협업 문서](#협업-문서)

## 프로젝트 소개

- **기간:** 2025.10.17 ~ 2025.11.10  
- **목적:** 뉴스 API 통합 및 맞춤형 뉴스 제공, 활동/의견 관리  
- **특징:**
  - PostgreSQL + MongoDB 기반 데이터 안정성
  - Spring Batch로 뉴스 수집/백업 자동화
  - Spring Actuator + Prometheus 모니터링
  - 대용량 데이터 처리와 안정성 고려한 설계

## 팀원 구성

| 이름 | 역할 | GitHub |
|------|------|--------|
| 정기주 | 팀장 / 백엔드 개발 | [GitHub](https://github.com/jeonggiju) |
| 김용희 | 백엔드 개발 | [GitHub](https://github.com/backKim1024) |
| 민재영 | 백엔드 개발 | [GitHub](https://github.com/jymin0) |
| 박지석 | 백엔드 개발 | [GitHub](https://github.com/commicat2) |
| 이성훈 | 백엔드 개발 | [GitHub](https://github.com/polodumbo) |
| 주세훈 | 백엔드 개발 | [GitHub](https://github.com/Jusehun) |

## 기술 스택

### Backend

- Spring Boot
- MapStruct
- JPA

### Database

- PostgreSQL
- MongoDB

### Sever

- AWS ECR
- AWS ECS
- AWS S3
- AWS RDS

### Batch / Monitoring

- Spring Batch
- Spring Actuator
- Prometheus

### 협업 Tool

- Git / GitHub
- Notion
- Discord

## 레포지토리 구성

| Repo | 설명 |
|------|------|
| `monew-mvc` | 메인 API 서버 (Spring Boot MVC) | https://github.com/sb05-monew-team3/monew-mvc.git |
| `monew-batch` | 뉴스 수집 및 백업 Batch 서비스 |--------------------------------------------------|
| `monew-actuator` | 모니터링 및 상태 관리 서비스 |--------------------------------------------------|

## 브랜치 전략

- `main`: 배포용  
- `develop`: 통합 개발  
- `feature/*`: 기능 단위 개발  
  - 예시: `feature/news-api`, `feature/user-preference`, `feature/batch-backup`, `feature/actuator-monitor`  

## 커밋 컨벤션

- `feat`: 새로운 기능 추가  
- `fix`: 버그 수정  
- `refactor`: 코드 리팩토링  
- `test`: 테스트 코드 추가  
- `docs`: 문서 변경  
- `chore`: 빌드/설정 관련 작업  

## 프로젝트 구조 (예시)

```text
monew-mvc/
├─ src/
│  ├─ main/
│  │  ├─ java/
│  │  │  └─ com/monu/
│  │  │       ├─ config/
│  │  │       ├─ controller/
│  │  │       ├─ dto/
│  │  │       ├─ entity/
│  │  │       ├─ repository/
│  │  │       ├─ service/
│  │  │       └─ util/
│  │  └─ resources/
│  │       └─ application.yml
└─ test/
```

## 팀원별 구현 예정 기능

| 팀원 | 기능 |
|------|------|
| 정기주 | 기능 a 구현 |
| 김용희 | 기능 b 구현 |
| 민재영 | 기능 c 구현 |
| 박지석 | 기능 d 구현 |
| 이성훈 | 기능 e 구현 |
| 주세훈 | 기능 f 구현 |

## API 문서

- [Swagger UI ↗](http://sprint-project-1196140422.ap-northeast-2.elb.amazonaws.com/sb/monew/api/swagger-ui/index.html)

## 협업 문서

- [Notion ↗](https://polydactyl-pufferfish-876.notion.site/MoNew-28e08cfefb45803ebd28ffcd05a97b2e?source=copy_link)
