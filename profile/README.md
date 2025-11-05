<p align="center">
  <img width="852" height="148" alt="monew" src="https://github.com/user-attachments/assets/98ab2834-7986-45a4-8b8e-e59660d1dcf1" />
</p>

# Monew
Monew는 여러 뉴스 API를 통합하여 사용자 맞춤 뉴스를 제공하고, 사용자 활동 내역 및 의견을 기록/관리할 수 있는 플랫폼입니다.  
PostgreSQL과 MongoDB 기반으로 데이터를 안전하게 저장하고, Spring Batch로 뉴스 백업/수집을 자동화하며, Spring Actuator와 Prometheus를 통한 모니터링을 지원합니다.

## 개발 기간
- **기간:** 2025.10.17 ~ 2025.11.10
- **목적:** 뉴스 API 통합 및 맞춤형 뉴스 제공, 활동/의견 관리
- - **특징:**
  - PostgreSQL + MongoDB 기반 데이터 안정성
  - Spring Batch로 뉴스 수집/백업 자동화
  - Spring Actuator + Prometheus 모니터링
  - 대용량 데이터 처리와 안정성 고려한 설계

## 팀원 구성

| 이름 | 역할 | GitHub |
|------|------|--------|
| 정기주 | 팀장 / 배치 및 데이터 관리 담당| [GitHub](https://github.com/jeonggiju) |
| 김용희 | 사용자 관리 및 활동 담당 | [GitHub](https://github.com/backKim1024) |
| 민재영 | 뉴스 콘텐츠 관리 담당 | [GitHub](https://github.com/jymin0) |
| 박지석 | 관심사 콘텐츠 관리 담당 | [GitHub](https://github.com/commicat2) |
| 이성훈 | 알림 및 시스템 구조 담당 | [GitHub](https://github.com/polodumbo) |
| 주세훈 | 댓글 및 QA 담당 | [GitHub](https://github.com/Jusehun) |

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

## 🖥️개발 환경
- Version : Java 17
- IDE: IntelliJ
- Framwork: SpringBoot 3.5.6 springBoot admin 3.5.0
- ORM : Spring Data JPA + Hibernate
## ⚙️기술 스택
- Server/Deployment: AWS EC2 github Actions
- DataBase : PostgreSQL (RDS), MongoDB Atlas
- WS/WAS : Tomcat, Spring Boot Admin
- Storage : AWS S3
- Monitoring
- 아이디어 회의 : Notion, git/github, Discord, zep

## 레포지토리 구성

| Repo | 설명 |
|------|------|
|  [monew-mvc](https://github.com/sb05-monew-team3/monew-mvc.git)  | 메인 API 서버 (Spring Boot MVC) | |
|[monew-batch](https://github.com/sb05-monew-team3/monew-batch.git)  | 뉴스 수집 및 백업 Batch 서비스 ||
| [monew-actuator](https://github.com/sb05-monew-team3/monew-actuator.git) | 모니터링 및 상태 관리 서비스 ||

## API 문서
- [Swagger UI ↗](http://sprint-project-1196140422.ap-northeast-2.elb.amazonaws.com/sb/monew/api/swagger-ui/index.html)

## 협업 문서
- [Notion ↗](https://polydactyl-pufferfish-876.notion.site/MoNew-28e08cfefb45803ebd28ffcd05a97b2e?source=copy_link)
