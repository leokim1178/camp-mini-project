<p align="center">
<img src="https://capsule-render.vercel.app/api?&type=waving&color=2c1aa3&height=180&section=header&text=Mini Project%20Starbucks&fontSize=50&animation=fadeIn&fontAlignY=45&fontColor=FFFFFF">
  </p>

# ☕️ 스타벅스 모의어플 백엔드

-   mongoDB,nodejs를 이용해 구성했습니다

---

## 📑 목차

- [☕️ 스타벅스 모의어플 백엔드](#️-스타벅스-모의어플-백엔드)
  - [📑 목차](#-목차)
  - [🚀 프로젝트 실행 및 테스트](#-프로젝트-실행-및-테스트)
  - [🕹 서버,DB 설계](#-서버db-설계)
  - [💻 기술 스택](#-기술-스택)
  - [🛠 파이프 라인](#-파이프-라인)
  - [🗂 폴더 구조](#-폴더-구조)
  - [🔒 ENV](#-env)

---

## 🚀 프로젝트 실행 및 테스트

-   local에서 테스트 💡

```
git clone https://github.com/leokim1178/camp-mini-project
cd backend
# .env 추가
docker 설치
docker compose build
docker compose up
```

-   swagger에서 테스트하기
    -   http://localhost:3001/swagger
-   frontend static html에서 테스트하기
    -   login, menou, user 내의 index.html을 실행하여 api 테스트

---

## 🕹 서버,DB 설계

-   Server FrameWork : Node.js
-   API Docs : Swagger Docs
-   DB : MongoDB (NoSQL)
-   ODM : Mongoose
-   crawler : puppeteer

---

## 💻 기술 스택

<div align="center">
📑&nbsp&nbsp&nbsp구성 언어
<br>
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> 
  </div>

 <div align="center">
  🚂  &nbsp&nbsp 서버
  <br>
  <img src="https://img.shields.io/badge/node.js-339933?style=for-the-badge&logo=Node.js&logoColor=white">
  <img src="https://img.shields.io/badge/express-000000?style=for-the-badge&logo=express&logoColor=white">
  <br>
  <img src="https://img.shields.io/badge/docker-3c90e5?style=for-the-badge&logo=docker&logoColor=white"> 
  <img src="https://img.shields.io/badge/swagger-6b8d1f?style=for-the-badge&logo=swagger&logoColor=white">
  <img src="https://img.shields.io/badge/puppeteer-ffffff?style=for-the-badge&logo=puppeteer&logoColor=black">
  </div>
 <p align="center">
💾&nbsp&nbsp&nbsp 데이터
  </p>
 <p align="center">
  <img src="https://img.shields.io/badge/mongoDB-47A248?style=for-the-badge&logo=MongoDB&logoColor=white">

---

## 🛠 파이프 라인

-   [스타벅스 메뉴조회 API](imgs/스타벅스%20메뉴조회%20API%20PG.png)

-   [토큰 인증 API](imgs/토큰%20인증%20API%20PG.png)

-   [휴대폰 인증 완료 API](imgs/휴대폰%20인증완료%20API%20PG.png)

-   [회원 가입 API](imgs/회원가입%20API%20PG.png)

-   [회원 목록 조회 API](imgs/회원%20목록%20조회%20API%20PG.png)

---

## 🗂 폴더 구조

```
mini-project
├─ 🚀 backend
│  ├─ 🐳 .dockerignore
│  ├─ 🐳 Dockerfile
│  ├─ 🐳 docker-compose.yaml
│  ├─ 📮 email.js
│  ├─ index.js
│  ├─ models
│  │  ├─ ☕️ starbucks.model.js
│  │  ├─ 🪙 token.model.js
│  │  └─ 👩🏻‍💻 user.model.js
│  ├─ 🎒 package.json
│  ├─ 📞 phone.js
│  ├─ 🎨 scrapper.js
│  ├─ swagger
│  │  ├─ config.js
│  │  ├─ phone-swagger.js
│  │  ├─ starbucks-swagger.js
│  │  ├─ user-swagger.js
│  │  └─ users-swagger.js
│  └─ utils.js
├─ ➬ frontend
├─ imgs
├─ .gitignore
├─ .prettierrc
├─ README.md
└─ webcrawler
   ├─ index.js
   ├─ models
   │  └─ starbucks.model.js
   └─ package.json
```

---

## 🔒 ENV

```
SMS_APP_KEY=
SMS_X_SECRET_KEY=
SMS_SENDER=
EMAIL_APP_KEY=
EMAIL_X_SECRET_KEY=
EMAIL_SENDER=
```
