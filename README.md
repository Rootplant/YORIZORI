# 🍳 YoriZori — 요리 정보 제공 & 레시피 커뮤니티 플랫폼

<p align="center">
  <img src="https://via.placeholder.com/900x260?text=YoriZori+Project+Banner" alt="banner" />
</p>

## 📌 프로젝트 소개
**YoriZori**는 사용자가 레시피를 공유하고 북마크하며  
실시간 채팅과 쪽지 기능을 통해 소통할 수 있는 **요리 정보 제공 플랫폼**입니다.
ST​S3 → ST​S4로 리빌드하며 전체 기술 스택을 안정적으로 재구성했고, 
Spring 기반 서버와 JSP 기반 화면, Oracle DB, MyBatis, Spring Security 등을 사용하여  
CRUD, 인증/인가, 커뮤니티 기능 등 다양한 기능을 제공합니다.

---

## ✨ 주요 기능

### 👤 회원 기능
- 회원가입
- 로그인 / 로그아웃
- Spring Security 기반 인증/권한 관리
- 마이페이지
- 회원 정보 수정

### 📚 레시피 기능
- 레시피 등록
- 레시피 수정
- 레시피 삭제
- 전체 레시피 조회
- 카테고리별 레시피 조회
- 북마크(즐겨찾기) 기능
- 내 레시피 관리

### 📰 게시판 기능
- 공지사항 게시판
- 글 작성 / 수정 / 삭제

### 💬 커뮤니티 기능
- 실시간 전체 채팅(WebSocket)
- AI 요리 챗봇 기능
- 1:1 쪽지 기능

---

## 🛠 기술 스택

### Backend
- **Java 17**
- **Spring Framework / Spring MVC**
- **Spring Security**
- **MyBatis**
- **Tomcat**
- **Oracle Database**

### Frontend
- **JSP**
- **HTML5, CSS3, JavaScript**
- **jQuery**

### DevOps & Tools
- **Git / GitHub**
- **ST**S3 → **STS4**
- **gradle**
- **Postman**

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,mysql,html,css,js,git,github" />
</p>

---

## 📁 프로젝트 구조

```bash
YoRiZoRi/
├─ src/main/java/com.boot/
│  ├─ Board/               # 게시판 기능
│  ├─ Chat/                # Gemini 챗봇
│  ├─ ChatBot.controller/  # 챗봇 컨트롤러
│  ├─ common.dto/          # 공통 DTO 모음
│  ├─ Detailed_Page/       # 레시피 상세 페이지
│  ├─ login/               # 로그인/회원 관리
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
│  ├─ mybatis.mappers/     # MyBatis XML 매퍼 파일들
│  ├─ templates/           # (필요시) Thymeleaf 템플릿
│  ├─ static/              # CSS/JS/IMG 정적파일
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

👥 팀원 & 역할
이름	역할
손봉균(팀장)	풀스택 - 로그인/회원가입/실시간 챗봇/ 구글 소셜로그인/ 페이징 처리
이현진	백엔드 개발 - 마이페이지/시큐리티/네이버,카카오 소셜로그인/ 댓글,대댓글 
박동영	백엔드 개발 - 레시피 페이지 /카테고리 구분/제미나이 챗봇
정찬호  백엔드 개발 - 레시피 상세 페이지 / 사용자 쪽지 

기타
JWT + Spring Security 인증 적용
WebSocket 실시간 채팅
REST API 기반 통신
컴포넌트 기반 UI 구성
