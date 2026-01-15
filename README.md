# 🍳 YoriZori — 요리 정보 제공 & 레시피 커뮤니티 플랫폼

<p align="center">
  <img src="https://github.com/user-attachments/assets/3f5231f5-e368-4875-9b5e-bcb8ff08f52e" alt="YoriZori Project Banner" />
</p>

---

## 📌 프로젝트 소개

**YoriZori**는 사용자가 레시피를 공유하고 검색하며,  
커뮤니티 기능(실시간 채팅·쪽지)을 통해 소통할 수 있는  
**요리 정보 제공 & 레시피 커뮤니티 플랫폼**입니다.

기존 STS3 기반 프로젝트를 **STS4 환경으로 리빌드**하며  
구조 개선 및 기능 안정화를 진행했고,  
Spring MVC · Spring Security · MyBatis · Oracle DB를 기반으로  
인증/인가, CRUD, 커뮤니티 핵심 기능을 구현했습니다.

- 기존 프로젝트(STS3):  
  👉 https://github.com/kh2yorizori/kh2_yorizori

---

## 👨‍💻 담당 역할 (정찬호)

본 프로젝트에서 **백엔드 핵심 기능 설계 및 구현**을 담당했습니다.

- **DB 설계**
  - 레시피, 레시피 상세, 이미지, 쪽지 관련 테이블 설계
  - 기능 흐름에 맞춘 관계 정의 및 정규화

- **레시피 기능 구현**
  - 레시피 등록 / 수정 / 상세 조회
  - 레시피 상세 페이지 데이터 가공 및 출력
  - 레시피 상세 조건 기반 검색 기능 구현

- **이미지 처리 전반**
  - 레시피 대표 이미지 및 상세 이미지 업로드
  - 서버 저장 및 조회 로직 구현
  - 레시피 상세 화면 이미지 렌더링 처리

- **실시간 쪽지 기능 설계 및 구현**
  - 사용자 간 1:1 쪽지 송수신 기능
  - 실시간 메시지 전송 및 즉시 답장 가능 구조 설계
  - 쪽지 읽음 / 안읽음 상태 실시간 반영
  - 읽지 않은 쪽지 개수 관리 및 UI 표시 연동

---

## ✨ 주요 기능

- **회원 관리**
  - 회원가입, 로그인/로그아웃
  - Spring Security 기반 인증/권한 관리
  - 마이페이지 정보 조회 및 수정

- **레시피 관리**
  - 레시피 등록 / 수정 / 삭제
  - 전체·카테고리·상세 조건 검색
  - 북마크(즐겨찾기) 기능

- **커뮤니티 기능**
  - WebSocket 기반 실시간 채팅
  - *메신저형 1:1 실시간 쪽지 기능*
    - 실시간 메시지 송수신
    - 읽음 / 안읽음 상태 즉시 반영
    - 대화 흐름 유지 가능한 구조 설계
  - AI 요리 챗봇(Gemini) 연동

- **게시판**
  - 공지사항 게시판
  - 게시글 CRUD 및 관리 기능

---

## 📸 서비스 화면

### 🔐 로그인 / 🧾 메인 페이지
<p align="center">
  <img src="https://github.com/user-attachments/assets/f7193ac1-6d4f-4f84-9dc9-e1f67d233842" width="47%" />
  <img src="https://github.com/user-attachments/assets/e28d85b0-2158-4f78-8869-3a88241671b7" width="47%" />
</p>

### 🥘 레시피 목록 / 🍳 레시피 상세 페이지
<p align="center">
  <img src="https://github.com/user-attachments/assets/1f24b8c3-0a7b-4b04-8e7c-00190cdcb368" width="47%" />
  <img src="https://github.com/user-attachments/assets/a608aaad-3331-47f4-9e9e-d42bd2b11d65" width="47%" />
</p>

### 💬 실시간 채팅 / 🤖 AI 요리 챗봇
<p align="center">
  <img src="https://github.com/user-attachments/assets/92ba12a9-38b6-465a-b5aa-c13f70f18123" width="47%" />
  <img src="https://github.com/user-attachments/assets/1d43cb23-df41-4dda-a2f3-f7adbf9a04bc" width="47%" />
</p>

### ✉️ 실시간 쪽지 기능
<p align="center">
  <img src="https://github.com/user-attachments/assets/0535efa8-5177-4df5-b391-fcde6d0c22a4" width="47%" />
  <img src="https://github.com/user-attachments/assets/3ab112f6-6d08-4837-b0ca-eb1bca8f1fb2" width="47%" />
</p>

---

## 🛠 기술 스택

### Backend
- Java 17
- Spring MVC / Spring Security
- MyBatis
- Tomcat
- Oracle Database

### Frontend
- JSP
- HTML5 / CSS3 / JavaScript
- jQuery

### Tools & Environment
- Git / GitHub
- STS3 → STS4
- Gradle
- Postman

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,html,css,js,git,github" />
</p>

---

## 💡 한 줄 요약

> **YoriZori는 레시피 CRUD·검색·이미지 처리와  
실시간 읽음 처리가 가능한 쪽지 기능을 Spring 기반으로 구현한  
요리 커뮤니티 플랫폼입니다.**
