# 🍳 YoriZori — 요리 정보 제공 & 레시피 커뮤니티 플랫폼

<p align="center">
  <img src="https://via.placeholder.com/900x260?text=YoriZori+Project+Banner" alt="YoriZori Project Banner" />
</p>

## 📌 프로젝트 소개
**YoriZori**는 사용자가 다양한 레시피를 공유하고, 북마크하며,  
실시간 채팅과 1:1 쪽지를 통해 소통할 수 있는 **요리 정보 플랫폼**입니다.  
STS3 → STS4 기반으로 전체 기술 스택을 안정적으로 리빌드했으며,  
Spring 기반의 서버, JSP 화면, Oracle DB, MyBatis, Spring Security 등  
최신 기술을 활용해 CRUD, 인증/인가, 커뮤니티 기능을 제공합니다.

---

## ✨ 주요 기능

- **회원 관리**: 회원가입, 로그인/로그아웃, 마이페이지, 회원 정보 수정, Spring Security 기반 인증/권한 관리
- **레시피 관리**: 레시피 등록/수정/삭제, 전체/카테고리별/내 레시피 조회, 북마크(즐겨찾기)
- **게시판**: 공지사항 게시판, 게시글 작성/수정/삭제
- **커뮤니티**: 실시간 채팅(WebSocket), AI 요리 챗봇(Gemini), 1:1 쪽지 기능

---

## 📸 서비스 화면

### 🔐 로그인 페이지
<p align="center">
  <img src="이미지URL" width="750" alt="로그인 페이지" />
</p>

### 🧾 메인 페이지
<p align="center">
  <img src="이미지URL" width="750" alt="메인 페이지" />
</p>

### 🥘 레시피 목록
<p align="center">
  <img src="이미지URL" width="750" alt="레시피 목록 페이지" />
</p>

### 🍳 레시피 상세 페이지
<p align="center">
  <img src="이미지URL" width="750" alt="레시피 상세 페이지" />
</p>

### 💬 실시간 채팅(WebSocket)
<p align="center">
  <img src="이미지URL" width="750" alt="실시간 채팅" />
</p>

### 🤖 AI 요리 챗봇(Gemini)
<p align="center">
  <img src="이미지URL" width="750" alt="AI 요리 챗봇" />
</p>

---

## 🛠 기술 스택

### Backend
- Java 17
- Spring Framework / MVC / Security
- MyBatis
- Tomcat
- Oracle Database

### Frontend
- JSP
- HTML5, CSS3, JavaScript
- jQuery

### DevOps & Tools
- Git / GitHub
- STS3 → STS4
- Gradle
- Postman

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,mysql,html,css,js,git,github" />
</p>

---

## 📁 프로젝트 구조

```bash
YoRiZoRi/
├─ src/main/java/com.boot/
│  ├─ Board/               # 게시판 기능
│  ├─ Chat/                # 실시간 채팅/챗봇
│  ├─ ChatBot.controller/  # 챗봇 컨트롤러
│  ├─ common.dto/          # 공통 DTO
│  ├─ Detailed_Page/       # 레시피 상세페이지
│  ├─ login/               # 로그인/회원 기능
│  ├─ Main_Page/           # 메인 페이지
│  ├─ MY_Page/             # 마이페이지
│  ├─ Notice/              # 공지사항
│  ├─ Recipe/              # 레시피 CRUD
│  ├─ config/
│  │  ├─ WebMvcConfig.java
│  │  └─ UnreadMessageInterceptor.java
│  └─ YoRiZoRiApplication.java
│
├─ src/main/resources/
│  ├─ mybatis.mappers/     # MyBatis 매퍼 XML
│  ├─ templates/           # (필요시) Thymeleaf 템플릿
│  ├─ static/              # 정적 파일(CSS/JS)
│  ├─ application.properties
│  └─ mybatis-config.xml
│
├─ src/main/webapp/
│  ├─ WEB-INF/
│  │  ├─ lib/
│  │  └─ views/
│  │     ├─ board/
│  │     ├─ common/
│  │     ├─ notice/
│  │     ├─ recipe/
│  │     ├─ login.jsp
│  │     ├─ home.jsp
│  │     ├─ mypage_edit.jsp
│  │     ├─ myrecipe.jsp
│  │     ├─ recipe_list.jsp
│  │     ├─ recipeDetail.jsp
│  │     └─ write_recipe.jsp
│  └─ web.xml
│
├─ build.gradle
├─ gradlew
├─ gradlew.bat
└─ README.md
```

---

## 👥 팀원 및 역할

| 이름           | 역할 및 담당 |
|----------------|-------------|
| **손봉균(팀장)** | 풀스택 - 로그인, 회원가입, 실시간 챗봇, 구글 소셜로그인, 페이징 |
| **이현진**      | 백엔드 - 마이페이지, 시큐리티, 네이버·카카오 소셜로그인, 댓글/대댓글 |
| **박동영**      | 백엔드 - 레시피 페이지, 카테고리 구현, Gemini 챗봇 |
| **정찬호**      | 백엔드 - 레시피 상세페이지, 쪽지 기능 |

---

## 🧩 기타 특장점

- **JWT + Spring Security 기반 인증/인가**
- **WebSocket 기반 실시간 채팅**
- **REST API 기반 통신 구성**
- **컴포넌트 기반 UI 구조 채택**

---
