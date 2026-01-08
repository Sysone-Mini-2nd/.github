# 📘 STM  - AI 기반 자동화 프로젝트 관리 플랫폼

> "반복적인 업무는 AI에게, 당신은 핵심 가치에 집중하세요."
> 프로젝트 생성부터 회의록 요약, 일정 관리까지 한 번에 해결하는 올인원 협업 툴입니다.

<img width="1146" height="707" alt="image" src="https://github.com/user-attachments/assets/e1e0f306-7990-445e-8751-d29109718214" />

## 📅 프로젝트 개요
기존 프로젝트 관리 방식의 비효율적인 의사소통과 수동 작업의 한계를 극복하기 위해 개발되었습니다. **STM**은 요구사항 정의서 기반의 **자동 작업 생성**, **AI 회의록 요약**, **실시간 대시보드** 기능을 통해 PM과 팀원 모두의 생산성을 극대화합니다.

* **개발 기간**: 2024.09.03 ~ 2024.09.16 (약 2주)
* **팀명**: Sysone F4

## 🚀 주요 기능 (Key Features)

### 1. 🤖 AI 기반 스마트 작업 생성
* 엑셀 형식의 요구사항 정의서를 업로드하면 AI(OpenAI)가 자동으로 세부 작업(Issue)을 생성하고 우선순위를 설정합니다.
* 반복적인 초기 세팅 시간을 획기적으로 단축합니다.

### 2. 📝 AI 회의록 및 음성 인식
* **CLOVA Speech**를 활용하여 회의 음성을 텍스트로 변환(STT)합니다.
* AI가 회의 내용을 분석하여 **핵심 안건, 결정 사항, 향후 계획**으로 자동 요약하고 이메일로 전송합니다.

### 3. 📊 생산성 대시보드
* 프로젝트 진행률, 팀원별 리소스 현황, 이슈 진행 상태를 시각화된 차트로 제공합니다.
* 데이터 기반의 의사결정을 지원합니다.

### 4. 💬 실시간 협업 & 메신저
* WebSocket 기반의 실시간 1:1 및 그룹 채팅을 지원합니다.
* 파일 공유 및 업무 알림 기능을 포함합니다.

### 5. 📅 일정 관리 (Gantt & Calendar)
* 간트 차트(Gantt Chart)를 통해 프로젝트 흐름을 한눈에 파악하고 일정을 조정합니다.
* 캘린더 뷰를 통해 개인 및 팀의 일정을 관리합니다.

---

## 🛠 기술 스택 (Tech Stack)

### Frontend
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=black"/> <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=Vite&logoColor=white"/> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/> <img src="https://img.shields.io/badge/Zustand-orange?style=flat-square&logo=R&logoColor=white"/> <img src="https://img.shields.io/badge/TanStack_Query-FF4154?style=flat-square&logo=ReactQuery&logoColor=white"/> <img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat-square&logo=TailwindCSS&logoColor=white"/> <img src="https://img.shields.io/badge/MUI-007FFF?style=flat-square&logo=MUI&logoColor=white"/>

* **Core**: React, SpringBoot, Vite
* **State Management**: Zustand, TanStack Query (React Query)
* **Styling**: TailwindCSS, Emotion, MUI
* **Visualization**: Recharts, svar-ui/react-gantt, React Big Calendar
* **Network**: Axios, StompJS/SockJS (WebSocket)

### Backend
<img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=Java&logoColor=white"/> <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=flat-square&logo=SpringBoot&logoColor=white"/> <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=SpringSecurity&logoColor=white"/> <img src="https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=Oracle&logoColor=white"/> <img src="https://img.shields.io/badge/JWT-black?style=flat-square&logo=JSON%20web%20tokens&logoColor=white"/>

* **Framework**: Spring Boot
* **Security**: Spring Security, JWT
* **Database**: Oracle
* **API**: OpenAI API, Naver CLOVA Speech

### Infra & DevOps
<img src="https://img.shields.io/badge/Amazon_EC2-FF9900?style=flat-square&logo=AmazonEC2&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=GitHubActions&logoColor=white"/>

* **Deploy**: EC2, Docker, GitHub Actions
* **Collab**: Jira, Figma, Slack, Notion

---

## 👨‍💻 팀원 소개 (Team Members)

| 이름 | 역할 | 담당 업무 |
|:---:|:---:|:---|
| **김대호** | **FE / BE** | • 전체적인 프론트엔드 UI/UX 개발 <br>• CI/CD 파이프라인 구축 (Docker, EC2, VM)<br>• 사용자 인증/인가 (JWT, Security)|
| **배지원** | **BE / FE** | • 회의록 기능 구현 (STT, AI 요약)<br>• 대시보드 데이터 시각화 및 통계 API<br>• 일정 관리 기능 |
| **백승준** | **BE / FE** | • 프로젝트 생성 및 관리 로직<br>• 요구사항 정의서 파싱 및 이슈 자동 생성<br>• 간트 차트 및 이슈 트래킹 |
| **조윤상** | **BE / FE** | • 실시간 메신저(WebSocket) 구현<br>• 채팅방 관리 및 알림 시스템<br>• 채팅 api 연동 |

---

## 🔧 트러블 슈팅 (Troubleshooting)

프로젝트 진행 중 발생한 주요 이슈와 해결 과정입니다.

### 1. WebSocket 인증 문제 (Access is denied)
* **문제**: JWT 로그인 후 발급받은 토큰으로 WebSocket 메시지(send) 전송 시 서버에서 권한 거부 오류 발생.
* **해결**: StompHandler 인터셉터를 구현하여 연결(Connect) 시점에 토큰을 검증하고, 해당 세션의 인증 정보를 SecurityContext에 저장하도록 개선.

### 2. 테스트 환경 Bean 주입 오류
* **문제**: 빌드 시 테스트 코드 실행 중 특정 서비스 Bean 주입 불가 오류 발생.
* **해결**: `application-test.yml`을 별도로 구성하고 `@ActiveProfiles("test")`를 적용하여 테스트 환경을 격리 및 정상화.

### 3. 공통 데이터 관리 (BaseEntity)
* **문제**: 생성일, 수정일 등 반복되는 컬럼 관리의 비효율성.
* **해결**: Interceptor(또는 JPA Auditing) 기능을 통해 Insert/Update 시 자동으로 현재 시간을 주입하고, Soft Delete 로직을 공통화하여 코드 중복 제거.

### 4. 일관된 예외 처리
* **문제**: 팀원별로 상이한 예외 처리 방식으로 인한 관리 어려움.
* **해결**: `GlobalExceptionHandler`와 `@ExceptionHandler`를 도입하여 전역적으로 예외를 포착하고 일관된 응답 포맷을 반환하도록 구조화.

---
