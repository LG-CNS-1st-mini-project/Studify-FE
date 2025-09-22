# STUDYFY

스터디파이(STUDYFY)는 IT 분야 팀원 모집, 스터디/프로젝트 관리, 커뮤니티 기능을 제공하는 웹 서비스입니다.  
개발자, 디자이너 등 다양한 포지션의 팀원을 쉽게 찾고, 모집글 작성·관리·신청·댓글 등 협업에 필요한 기능을 제공합니다.

---

## 주요 기능

- **회원가입/로그인**  
  JWT 기반 인증, 회원정보 관리

- **모집글 작성/수정/삭제**  
  프로젝트/스터디 모집글 등록, 수정, 삭제  
  모집 분야, 기술스택, 마감일 등 다양한 정보 입력

- **모집글 목록/검색/필터**  
  전체 모집글 조회, 키워드/포지션별 검색, 필터링

- **모집글 상세**  
  모집글 상세 정보, 댓글, 신청하기, 모집 마감, 수정/삭제

- **댓글**  
  모집글별 댓글 작성/삭제

- **알림**  
  팀원 신청 등 주요 이벤트 알림

- **마이페이지**  
  내 정보, 내가 쓴 글, 내 신청 내역 관리

---

## 기술 스택

- **Frontend**: React, React Router, Axios, CSS Modules
- **Backend**: Spring Boot, Spring Security, JPA, MySQL
- **API 문서**: Swagger (OpenAPI)
- **인증**: JWT

---

## 프로젝트 구조
STUDYFY/
├── src/
│   ├── api/           # API 호출 함수 (axios)
│   ├── components/    # 공통 컴포넌트 (Navbar, Button 등)
│   ├── pages/         # 주요 페이지 (Home, SignIn, SignUp, WritePage, PostDetail, MyPage 등)
│   ├── styles/        # CSS 파일
│   └── App.js
├── public/
│   └── ...            # 정적 파일, 이미지 등
├── package.json
└── ...


---

## 실행 방법

### 1. 백엔드(Spring Boot) 실행

1. `git clone` 또는 소스 다운로드
2. `application.yml` DB 설정
3. Gradle/Maven으로 빌드 및 실행

4. Swagger: [http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)

### 2. 프론트엔드(React) 실행

1. `npm install`
2. `package.json`에 `"proxy": "http://localhost:8080"` 추가
3. `npm start`
4. [http://localhost:3000](http://localhost:3000) 접속

---

## API 예시

- 모집글 전체 조회: `GET /studify/api/v1/post/posts`
- 모집글 생성: `POST /studify/api/v1/post/posts`
- 모집글 상세: `GET /studify/api/v1/post/detail/{postId}`
- 모집글 수정: `PUT /studify/api/v1/post/{postId}`
- 모집글 삭제: `DELETE /studify/api/v1/post/{postId}`
- 모집글 마감: `PATCH /studify/api/v1/post/{postId}`
- 키워드 검색: `GET /studify/api/v1/post/search?keyword=...`
- 포지션 검색: `GET /studify/api/v1/post/search/position?position=...`

---

## 개발/기여

- 이 저장소는 IT 협업을 위한 오픈소스 프로젝트입니다.
- 이슈/PR/기여 환영합니다!

---

## 기타

- 문의: 팀장 또는 저장소 이슈 탭 이용
- 본 프로젝트는 교육 및 포트폴리오 용도로 제작되었습니다.

---

**스터디파이와 함께 IT 협업을 더 쉽고, 더 즐겁게!** 🚀
