### 🧑‍💻 개발 명령어
```bash
  # docker-compose.yml 실행
  docker-compose up -d
  
  ```

# 🚀 "OHFLIX" - 영상 스트리밍 플랫폼

<br>

<p align="center">
  <img src="https://github.com/chugue/project-ohflix/assets/30003848/3ba28c1a-6ab4-444a-8832-e07f103bfe85)"  style="width: 50%; height: auto;"/>
</p>

<br>

# 👉 영상 스트리밍 플랫폼
> ### 개발기간: 2024.06.12 ~ 2024.07.03

<br>

# 👉 깃허브 주소
  
> #### 애플리케이션 서버          : [https://github.com/chugue/project-ohflix](https://github.com/chugue/project-ohflix)<br>
> #### 인코딩 / 라이센스 서버     : [https://github.com/chugue/video-server](https://github.com/chugue/video-server)<br>
<br>

# 👉 개발팀 소개


<table style="width:100%; text-align:center;">
  <tr>
    <th style="text-align:center;">김성훈(팀장)</th>
    <th style="text-align:center;">박동기</th>
    <th style="text-align:center;">양승호</th>
    <th style="text-align:center;">공지영</th>
    <th style="text-align:center;">최윤정</th>
  </tr>
  <tr>
    <td style="text-align:center; vertical-align:middle;"><img width="160px" src="https://avatars.githubusercontent.com/u/30003848?v=4" /></td>
    <td style="text-align:center; vertical-align:middle;"><img width="160px" src="https://avatars.githubusercontent.com/u/153582240?v=4" /></td>
    <td style="text-align:center; vertical-align:middle;"><img width="160px" src="https://avatars.githubusercontent.com/u/97007464?v=4"/></td>
    <td style="text-align:center; vertical-align:middle;"><img width="160px" src="https://avatars.githubusercontent.com/u/52162820?v=4" /></td>
    <td style="text-align:center; vertical-align:middle;"><img width="160px" src="https://avatars.githubusercontent.com/u/129649095?v=4" /></td>
  </tr>
  <tr>
    <td style="text-align:center; vertical-align:middle;"><a href="https://github.com/chugue">@chugue</a></td>
    <td style="text-align:center; vertical-align:middle;"><a href="https://github.com/dongkipark1">@dongkipark1</a></td>
    <td style="text-align:center; vertical-align:middle;"><a href="https://github.com/LifeIsOne">@LifeIsOne</a></td>
    <td style="text-align:center; vertical-align:middle;"><a href="https://github.com/Kongjiyoung">@Kongjiyoung</a></td>
    <td style="text-align:center; vertical-align:middle;"><a href="https://github.com/yunchocopie">@yunchocopie</a></td>
  </tr>
</table>


<br>

# 👉프로젝트 소개 (핵심로직 설명)
> #### 오플릭스는 영상 스트리밍 서비스를 제공하는 플랫폼입니다.
> #### 사용자는 서비스를 구독하고, 오플릭스는 사용자에게 암호화된
> #### 영상을 DASH 프로토콜로 네트워크 상황에 따라 품질을 다르게 전송하여
> #### 끊김이 없는 영상 서비스를 제공합니다.

<br>


| 시연영상 링크 ( 사진 클릭 👇👇) |
|:---------------------------:|
| [![시연02](https://img.youtube.com/vi/3YMpCAriG0Y/0.jpg)](https://www.youtube.com/watch?v=3YMpCAriG0Y) |


<br>
<br>

# 👉 프로젝트 구조

![프로젝트구조 1](https://github.com/chugue/project-ohflix/assets/30003848/15e36619-ed3a-4d78-9639-122ff89c0d9f)
![프로젝트구조 2](https://github.com/chugue/project-ohflix/assets/30003848/e9a1d443-f4ab-4176-b2a9-fdb4b29dc27f)


<br>
<br>

# 👉 오플릭스 PPT 발표자료
[오플릭스 PPT - pdf](https://github.com/user-attachments/files/16082996/OHFLIX-PPT.pdf)

<br>
<br>

# 👉 Stacks

![기술스택](https://github.com/chugue/project-ohflix/assets/30003848/b169db7a-e2a7-46d2-9d6c-7eda6fe892d7)



### Communication

![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white)

<br>

# 👉 Dependencies
```java
dependencies {
    implementation 'com.github.iamport:iamport-rest-client-java:0.1.6' // iamport
    implementation 'org.springframework.boot:spring-boot-starter-data-jpa'
    implementation 'org.springframework.boot:spring-boot-starter-mustache'
    implementation 'org.springframework.boot:spring-boot-starter-web'
    compileOnly 'org.projectlombok:lombok'
    developmentOnly 'org.springframework.boot:spring-boot-devtools'
    runtimeOnly 'com.h2database:h2'
    annotationProcessor 'org.projectlombok:lombok'
    testImplementation 'org.springframework.boot:spring-boot-starter-test'
    testImplementation 'org.springframework.restdocs:spring-restdocs-mockmvc'
    testRuntimeOnly 'org.junit.platform:junit-platform-launcher'
    /////////// 추가 의존성 //////////
    implementation 'org.springframework.boot:spring-boot-starter-validation'
    implementation 'org.springframework.boot:spring-boot-starter-aop'
    implementation group: 'org.apache.commons', name: 'commons-lang3', version: '3.0'
    implementation group: 'com.auth0', name: 'java-jwt', version: '4.3.0'
    implementation group: 'org.mindrot', name: 'jbcrypt', version: '0.4'
    implementation 'com.google.code.gson:gson:2.10.1'
    implementation group: 'org.qlrm', name: 'qlrm', version: '4.0.1'
    runtimeOnly 'com.mysql:mysql-connector-j'
    implementation 'commons-codec:commons-codec:1.15'
    implementation 'org.springframework.boot:spring-boot-starter-data-redis'
    implementation 'org.springframework.session:spring-session-data-redis'
    implementation 'io.github.cdimascio:java-dotenv:5.2.2'
}
```

<br>

# 👉 테이블 설계
![ERD구조](https://github.com/chugue/project-ohflix/assets/30003848/2aebd0c4-c789-4a7a-8572-8e7b7adeb784)


<br>


# 👉 팀 블로깅  
[팀 블로그 링크](https://www.notion.so/stephenkiim/a382fcac61694a7297ffad6c39bd86cb)

<br>
<br>

# 👉 프로젝트 주요 기능 정리
* #### Redis 세션 인증
* #### 카카오 OAuth 인증
* #### 로그인 인터셉터 - 세션 기반
* #### 영상 CRUD 구현
* #### DASH 프로토콜 영상 재생
* #### 영상 암호화 패키징 - Shaka Packager
* #### 인코딩 / 라이센스 서버 구축 (DRM)
* #### 카카오 페이 결제
* #### 아임포트 카드 결제
* #### 비밀번호 암호화 - Bcrypt
* #### AI 추천 컨텐츠 - OpenAI
* #### 영상 시청 중단점 프로그레스 바
* #### 영상 찜하기
* #### 영상 좋아요
* #### 매출 페이지 chart.js 표현
* #### 키보드 입력 동시 검색기능
* #### AWS S3 스토리지 서버 구축
* #### 매출페이지 Chart.js 사용
* #### 메인페이지 Swiper 사용
<br>
<br>


# 👉 핵심 시나리오 시연
### 🔹영상 등록 => 인코딩 서버로 비동기로 전송

![영상등록](https://github.com/chugue/project-ohflix/assets/30003848/d5448404-c8e2-4aba-a5ff-a90a42c91c7e)

<br>

### 🔹 사용자 회원가입 => 구독결제하지 않아도 메인페이지 접속 가능

![사용자 회원가입](https://github.com/chugue/project-ohflix/assets/30003848/117ce445-d963-4497-ba00-0b7fb0dcd359)

<br>

### 🔹 카카오 OAuth => 회원정보가 없으면 자동가입, 있으면 자동로그인

![카카오 OAuth](https://github.com/chugue/project-ohflix/assets/30003848/55441b35-945f-4f25-b738-08ec40e9ed7a)


<br>

### 🔹 아엠포트 카드 결제

![아엠포트 카드결제](https://github.com/chugue/project-ohflix/assets/30003848/17f5c302-c4fe-4c55-a69c-6ec644f34a8e)


<br>

### 🔹 카카오 페이 결제

![카카오 페이 결제](https://github.com/chugue/project-ohflix/assets/30003848/33218062-1e59-4194-9686-efda654e8160)



### 🔹 관리자 매출확인
![매출확인](https://github.com/chugue/project-ohflix/assets/30003848/4d1d5eba-40a3-4ced-839e-490b407433a0)

<br>

### 🔹 영상 보기 => 세그먼트 호출
![영상보기](https://github.com/chugue/project-ohflix/assets/30003848/77ccd66e-4c52-431f-9e71-c6c8a3e11ba6)

<br>

### 🔹 영상 보기 => 재생 시점부터 세그먼트 호출
![재생 시점부터 세그먼트 호출](https://github.com/chugue/project-ohflix/assets/30003848/8798943c-269a-460e-b2bb-f81257c9f3ec)

<br>

### 🔹 영상 보기 => 캐시데이터 호출
![캐시 데이터 호출](https://github.com/chugue/project-ohflix/assets/30003848/f27e2407-4983-4524-a9a7-f4ffe632ed87)

<br>

### 🔹 영상 보기 => 최근 종료된 재생시점에서 이어보기
![영상 이어보기](https://github.com/chugue/project-ohflix/assets/30003848/2c97922b-490a-4389-8821-bb92a3a1b644)

<br>
 
### 🔹 영상 찜하기
![영상 찜하기](https://github.com/chugue/project-ohflix/assets/30003848/19553edd-8058-47a6-821d-f8790ce6a884)

<br>
 
### 🔹 AI추천 컨텐츠
![AI추천 컨텐츠](https://github.com/chugue/project-ohflix/assets/30003848/3b2342e3-53ab-47a3-a4bb-b97227a1456f)

<br>

### 🔹 KeyUp 검색
![KeyUp 검색](https://github.com/chugue/project-ohflix/assets/30003848/0e97ba24-32fc-44d0-892a-1b0c6cc763b1)


<br>
<br>


