<div align="center">
  <img width="120" height="120" alt="logo" src="https://github.com/user-attachments/assets/4ff9ff1f-58bf-4e93-8331-db269bfefec7" />
  <h1><strong>Welcome to the DoEatFit!</strong></h1>
  <p><strong>건강한 식단과 운동 습관을 위한 당신의 건강 파트너, DoEatFit에 오신 것을 환영합니다.</strong></p>
  <p>
    <a href="https://github.com/DoEatFit/doeatfit_front"><strong>🚀 Frontend</strong></a> |
    <a href="https://github.com/DoEatFit/doeatfit_back"><strong>⚙️ Backend</strong></a> |
    <a href="https://github.com/DoEatFit/doeatfit_infra"><strong>☸️ Infra</strong></a> |
    <a href="https://github.com/DoEatFit/project_management"><strong>📋 Project Management</strong></a>
  </p>
</div>

---

## 🌟 우리의 비전 (Our Vision)

DoEatFit은 복잡한 건강 정보를 누구나 쉽게 이해하고 실천할 수 있도록 돕는 것을 목표로 합니다. 우리는 개인 맞춤형 식단 추천, 체계적인 운동 계획, 그리고 직관적인 데이터 분석 기능을 통해 사용자가 자신의 건강을 주도적으로 관리하고, 지속 가능한 건강 습관을 형성할 수 있도록 지원하고자 합니다.

나아가 DoEatFit은 개인의 건강 기록에서 멈추지 않고, **피트니스 센터의 운영까지 아우르는 서비스**로 확장되고 있습니다. 회원은 수강권으로 수업을 예약하고, 트레이너는 자신의 수업 스케줄과 담당 회원을 관리하며, 센터 관리자는 회원·수강권·결제 내역과 예약 현황을 한곳에서 다룹니다. 개인의 기록과 센터의 운영이 하나의 서비스 안에서 이어지도록 만드는 것이 우리가 지향하는 방향입니다.

**개인 기능** · 식단/운동/컨디션 기록과 캘린더·추이 분석, 식단·심박수 계산기, 운동 가이드, 함께 운동하는 잼(Jam) 세션, 웹 푸시 알림, 오프라인에서도 동작하는 PWA

**센터 기능** · 센터 등록 신청과 승인, 센터 회원·역할 관리, 수업 스케줄과 수강권 발급, 수업 예약·대기열·출석·노쇼 처리, 결제 내역 집계, 예약 히트맵, 트레이너 스케줄과 코칭(트레이너↔회원) 관계 관리

<br>

## ✨ 스크린샷 (Screenshots)

| 메인 페이지 (Main)                                   | 운동 정보 (Workouts)                                 |
| :--------------------------------------------------- | :--------------------------------------------------- |
| <img width="427" alt="메인화면" src="https://github.com/user-attachments/assets/391a311d-89c7-420b-8c05-5c12c237f7ae" /> | <img width="427" alt="운동" src="https://github.com/user-attachments/assets/82b14976-9d3b-4391-9539-5a56944e4bf7" /> |
| **로그인 (Login)** | **마이페이지 (My Page)** |
| <img width="427" alt="로그인" src="https://github.com/user-attachments/assets/848ef325-796d-4feb-88c4-07d23595ef29" />     | <img width="427" alt="마이페이지" src="https://github.com/user-attachments/assets/0636be6a-12cc-4663-9ecd-9712b55504cb" />         |
| **칼로리 계산기 (Calculator)** | **관리자 페이지 (Admin CMS)** |
| <img width="427" alt="계산기" src="https://github.com/user-attachments/assets/cbe2d2c3-767c-4b2d-8632-bb037731f769" /> | <img width="427" alt="CMS" src="https://github.com/user-attachments/assets/649909b7-6e77-4199-9623-f6cfd07ab288" /> |

<br>

## 👥 작업자 프로필 (Contributors)

DoEatFit 프로젝트를 함께 만들어가는 팀원들을 소개합니다.

| Profile                                                          | Name / Role                                                                   |
| :--------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| <img src="https://github.com/EricNaKor.png" width="80">           | **[EricNakor](https://github.com/EricNaKor)**<br/>서비스 기획, 백엔드, 프론트엔드, 데브옵스 |
| <img src="https://github.com/jewon-oh.png" width="80">           | **[jewon-oh](https://github.com/jewon-oh)**<br/>기술 아키텍처 선정, 백엔드, 프론트엔드, 데브옵스 |

<br>

## 🏗️ 아키텍처 (Architecture)

DoEatFit은 역할과 책임에 따라 명확하게 분리된 4개의 핵심 레포지토리로 구성되어 있습니다.

| Repository                                                                  | Description                                                                                                                                |
| :-------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- |
| 🥑 **[doeatfit_front](https://github.com/DoEatFit/doeatfit_front)** | 사용자에게 풍부하고 인터랙티브한 경험을 제공하는 웹 애플리케이션의 프론트엔드입니다. 소비자용 사이트와 관리자 CMS를 하나의 Next.js 앱에서 서빙합니다. |
| ⚙️ **[doeatfit_back](https://github.com/DoEatFit/doeatfit_back)** | 데이터 처리, 비즈니스 로직, 외부 서비스 연동 등 모든 서버 사이드 로직을 담당하는 백엔드입니다. 애플리케이션이 매핑하는 REST API 엔드포인트는 모두 `/api` 접두사를 사용하며, 운영용 Actuator 엔드포인트(`/actuator/**`)는 별도 포트로 분리되어 있습니다. |
| ☸️ **[doeatfit_infra](https://github.com/DoEatFit/doeatfit_infra)** | 애플리케이션 코드 없이 k8s 매니페스트와 운영 문서만 두는 GitOps 레포입니다. `k8s/base` + `k8s/overlays/{prod,staging}` Kustomize 구조를 ArgoCD가 배포합니다. |
| 📋 **[project_management](https://github.com/DoEatFit/project_management)** | 조직 전체 이슈의 단일 창구이며, 기능 명세 위키(`docs/wiki/`)·기획 문서(`docs/`)·회의록(`meetings/`)을 관리합니다.                              |

이 외에 조직 프로필 README 와 조직 공통 PR 템플릿(`.github/pull_request_template.md`)을 담는 [.github](https://github.com/DoEatFit/.github) 레포가 있습니다. 위 4개 레포는 자체 PR 템플릿을 두지 않고 이 템플릿을 상속합니다.

<br>

## 🛠️ 기술 스택 (Tech Stack)

다음은 DoEatFit을 구성하는 핵심 기술들입니다.

| Category             | Frontend                                                                       | Backend                                                                        | Infra                                                                          |
| :------------------- | :----------------------------------------------------------------------------- | :----------------------------------------------------------------------------- | :----------------------------------------------------------------------------- |
| **Language/Runtime** | `TypeScript 5.8`, `Node.js 22` (컨테이너)                                      | `Java 17` (소스 레벨), `Amazon Corretto 25` (컨테이너)                          | `Kustomize` 매니페스트 (애플리케이션 코드 없음)                                |
| **Main Framework** | `Next.js 16 (App Router)`, `React 18`                                          | `Spring Boot 3.5`, `Spring Security`, `Spring Data JPA`                        | `Kubernetes (k3s)`                                                             |
| **Data Fetching** | `TanStack Query`, `Axios`                                                      | `JPA (Hibernate)`, `QueryDSL 5.1`                                              | -                                                                              |
| **State Management** | `TanStack Query` (서버 상태) + `React Context`                                 | -                                                                              | -                                                                              |
| **Database/Search** | -                                                                              | `MySQL 8.0`, `Redis 7`, `Meilisearch v1.10`                                    | `MySQL`, `Redis`, `Meilisearch` StatefulSet                                    |
| **Styling** | `Tailwind CSS 3.4`, `shadcn/ui`                                                | `Thymeleaf` (for email templates)                                              | -                                                                              |
| **Authentication** | `httpOnly 쿠키` + BFF 프록시 (`/api/proxy`)                                    | `JWT`, `Google OAuth 2.0`                                                      | `Sealed Secrets` (kubeseal)                                                    |
| **File Storage** | -                                                                              | S3 호환 스토리지 (`MinIO Java SDK`)                                            | `SeaweedFS` (S3 API 호환)                                                      |
| **Push/Realtime** | `Firebase Cloud Messaging`, `SSE`                                              | `Firebase Admin SDK`, `SSE (SseEmitter)`                                       | -                                                                              |
| **PWA/Offline** | `Serwist` (Service Worker), `IndexedDB` 캐시 + outbox 큐                       | -                                                                              | -                                                                              |
| **Test** | `Vitest`, `Playwright`                                                         | `JUnit 5`, `Testcontainers`                                                    | -                                                                              |
| **Monitoring** | -                                                                              | `Spring Boot Actuator`, `Micrometer`, `OpenTelemetry Java Agent`               | `Prometheus`, `Loki`, `Tempo`, `Grafana` (크로스사이트 수집 `Grafana Alloy` 은 구축 중) |
| **Deployment** | `GitHub Actions` → `GHCR`                                                      | `GitHub Actions` → `GHCR`                                                      | `ArgoCD` (GitOps), `Gateway API (HTTPRoute)`, `Argo CD Image Updater`          |

> 배포는 CI가 서버에 직접 밀어넣는 방식이 아니라, GitHub Actions가 GHCR에 이미지를 푸시하고 ArgoCD가 `doeatfit_infra`의 매니페스트를 폴링해 반영하는 pull 방식입니다.

<br>

<div align="center">
  <p><strong>DoEatFit과 함께 건강한 변화를 시작해보세요!</strong></p>
</div>
