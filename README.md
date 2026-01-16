# 🍳 YoriZori — 요리 정보 제공 & 레시피 커뮤니티 플랫폼

<p align="center">
  <img src="https://github.com/user-attachments/assets/3f5231f5-e368-4875-9b5e-bcb8ff08f52e" alt="YoriZori Project Banner" />
</p>

---

## 📌 프로젝트 소개

**YoriZori**는 사용자가 레시피를 공유하고 검색하며,  
실시간 채팅·쪽지 기능을 통해 소통할 수 있는  
**요리 정보 제공 & 레시피 커뮤니티 플랫폼**입니다.

기존 **STS3 기반 프로젝트를 STS4 환경으로 리빌드**하며  
구조 개선, 보안 강화, 기능 안정화를 진행했고  
Spring MVC · Spring Security · MyBatis · Oracle DB 기반으로  
인증/인가, CRUD, 커뮤니티 핵심 기능을 구현했습니다.

- 기존 프로젝트(STS3)  
  👉 https://github.com/kh2yorizori/kh2_yorizori

---

## 👨‍💻 담당 역할 (정찬호)

> **백엔드 핵심 기능 설계 및 구현 담당**

| 구분 | 담당 내용 |
|---|---|
| 🧱 DB 설계 | 레시피·상세·이미지·쪽지 테이블 설계 및 정규화 |
| 🍳 레시피 | 등록 / 수정 / 상세 조회 / 조건 검색 |
| 🖼 이미지 처리 | 대표·상세 이미지 업로드 및 렌더링 |
| 💬 실시간 쪽지 | 1:1 실시간 송수신, 읽음 상태 관리 |
| 🛠 구조 개선 | STS3 → STS4 마이그레이션 |

---

## ✨ 주요 기능

- 🔐 **회원 관리**
  - 회원가입, 로그인/로그아웃
  - Spring Security 기반 인증·권한 관리
  - 마이페이지 정보 조회 및 수정

- 🍳 **레시피 관리**
  - 레시피 등록 / 수정 / 삭제
  - 전체·카테고리·조건 검색
  - 북마크(즐겨찾기)

- 💬 **커뮤니티 기능**
  - WebSocket 기반 실시간 채팅
  - 메신저형 1:1 실시간 쪽지
    - 실시간 송수신
    - 읽음 / 안읽음 상태 즉시 반영
    - 대화 흐름 유지 구조 설계
  - AI 요리 챗봇(Gemini) 연동

- 📢 **게시판**
  - 공지사항 게시판
  - 게시글 CRUD 및 관리 기능

---

## 🔍 내가 구현한 핵심 기능

---

### 🍳 레시피 조회 · 검색

<p align="center">
  <img src="https://github.com/user-attachments/assets/1f24b8c3-0a7b-4b04-8e7c-00190cdcb368" width="45%" />
  <img src="https://github.com/user-attachments/assets/a608aaad-3331-47f4-9e9e-d42bd2b11d65" width="45%" />
</p>

📌 **설명**

- 카테고리·재료·조건 기반 레시피 검색 기능 구현
- 레시피 목록 및 상세 페이지 데이터 가공 후 출력
- 대표 이미지 포함 레시피 정보 조회 처리
- 검색 결과와 상세 화면 간 자연스러운 사용자 탐색 흐름 구성

👉 단순 조회가 아닌  
**사용자가 원하는 레시피를 빠르게 찾을 수 있도록 설계된 검색 기능**

---

### 🖼 레시피 등록 · 수정

<p align="center">
  <img width="491" height="850" src="https://github.com/user-attachments/assets/620c3840-a0bd-4f6a-b0d9-9c26b12394e2" />
  <img width="373" height="658" src="https://github.com/user-attachments/assets/ad16fdc4-2b9e-4ad9-922f-352e6fa2193b" />
</p>

📌 **설명**

- 레시피 등록 / 수정 / 삭제 기능 구현
- 대표 이미지 및 상세 이미지 포함 레시피 데이터 등록 처리
- 서버 저장 경로 관리 및 이미지-레시피 매핑 구조 설계
- 수정 시 기존 이미지 유지·변경을 고려한 로직 구현

👉 **이미지를 포함한 레시피 콘텐츠를 안정적으로 관리할 수 있는 구조 설계**

---

### ✉️ 1:1 실시간 쪽지 기능 (핵심)

<p align="center">
  <img src="https://github.com/user-attachments/assets/6773976e-a6d9-4184-9db8-5492f7a684f7" width="90%" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/0535efa8-5177-4df5-b391-fcde6d0c22a4" width="45%" />
  <img src="https://github.com/user-attachments/assets/b6ffe36c-472e-4056-bb98-9b205e6e32d8" width="45%" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/3ab112f6-6d08-4837-b0ca-eb1bca8f1fb2" width="45%" />
</p>

📌 **설명**

- 사용자 간 1:1 실시간 쪽지 송수신
- 메시지 전송 즉시 상대방 화면 반영
- 읽음 / 안읽음 상태 실시간 처리
- 읽지 않은 쪽지 개수 UI 연동

👉 단순 메시지 저장이 아닌  
**실제 메신저와 유사한 실시간 커뮤니케이션 구조 구현**

---

### 🧱 DB 설계 & 구조 안정화

📌 **설명**

- 레시피 / 상세 / 이미지 / 쪽지 테이블 분리 설계
- 기능 흐름에 맞춘 관계 정의 및 정규화
- 확장 가능한 구조로 커뮤니티 기능 고려

👉 기능 추가를 고려한  
**유지보수 중심의 DB 설계**

---

## 📸 서비스 화면 예시

<details>
<summary><strong>🏠 메인 화면</strong></summary>

<p align="center">
  <!-- 메인 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>🍳 레시피 조회</strong></summary>

<p align="center">
  <!-- 레시피 목록 / 검색 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>🖼 레시피 등록 · 수정</strong></summary>

<p align="center">
  <!-- 레시피 등록 / 수정 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>👤 마이페이지</strong></summary>

<p align="center">
  <!-- 마이페이지 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>⭐ 즐겨찾기</strong></summary>

<p align="center">
  <!-- 즐겨찾기(북마크) 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>🤖 AI 요리 챗봇</strong></summary>

<p align="center">
  <!-- AI 요리 챗봇 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>💬 실시간 채팅</strong></summary>

<p align="center">
  <!-- 실시간 채팅 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>✉️ 1:1 실시간 쪽지 기능</strong></summary>

<p align="center">
  <!-- 1:1 쪽지 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>📢 공지사항</strong></summary>

<p align="center">
  <!-- 공지사항 화면 이미지 삽입 예정 -->
</p>

</details>

---

<details>
<summary><strong>📝 자유게시판</strong></summary>

<p align="center">
  <!-- 자유게시판 화면 이미지 삽입 예정 -->
</p>

</details>


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
실시간 읽음 처리가 가능한 1:1 쪽지 기능을  
Spring 기반으로 구현한 요리 커뮤니티 플랫폼입니다.**
