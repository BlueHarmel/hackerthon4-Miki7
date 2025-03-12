# 🏡 별책부록 🏡
### 부제

> 서비스 요약
### **별책부록 – 한 권의 책, 다양한 시선!**

🎬📚 **여러 명의 등장인물이 리뷰하는 독특한 리뷰 서비스** 

목표 : 다양한 시각을 담은 ‘별책부록’ 같은 리뷰를 제공

미키7이라는 팀명에서 시작된 아이디어로 한 가지 작품에 대해 별책부록은 기존의 단순한 리뷰 작성에서 벗어나, 여러 개성 있는 등장인물이 각자의 시선으로 리뷰를 남기는 독창적인 리뷰 플랫폼

💡**이런 순간, 별책부록을 사용하세요!**

✔**"이 영화 배우도 기억나고, 개봉년도도 아는데… 제목이 뭐였지?"**

✔**"친구들과 영화 이야기하다가 제목이 떠오르지 않을 때!"**

✔**"다른 사람들은 이 영화를 어떻게 봤을까?"**

<br><br>
## 팀원 소개 
![image]()
이영석  
김나경  
박성준  
<br><br>

## 개발 일정

![TimelineGanttOverviewSection]()

<br><br>

## 🌱 개발 언어 및 활용 기술

### FrontEnd
  <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/><img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"><img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=CSS3&logoColor=white"><img src="https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=Thymeleaf&logoColor=white">
### BackEnd
  <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"><img src="https://img.shields.io/badge/bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white">
### Infra & Cooporate
  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white"><img src="https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=Amazon%20EC2&logoColor=white"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=Amazon%20S3&logoColor=white"><img src="https://img.shields.io/badge/Discord-4169E1?style=for-the-badge&logo=Discord&logoColor=white"/><img src="https://img.shields.io/badge/aws-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white"/>
### DB
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white">
          
<br><br>

##  User Flow

① 플랫폼의 가장 첫 페이지인 메인페이지를 기준으로 Flow를 나누어 작성하였습니다.   <br>
② 노란색은 페이지를 보라색은 이동 버튼 및 트리거를 의미하며, 다이아몬드 모형은 논리 로직을 의미합니다. <br>
③ 빨간색 화살표는 비회원도 접근이 가능합니다. 파란색 화살표는 일반 유저의 로그인 상태일 경우 <br> 

![image]()

<br><br>

## 요구사항 및 기능 명세  

화면 단위로 기능을 분류하고, 해당 기능을 이용할 수 있는 권한을 기입하였습니다. 

| 화면        | 기능             | 내용                        | 권한               |
|------------|-----------------|---------------------------|-------------------|
| 메인       | 숙소 검색          | 공지사항 제목, 내용 조회     |            |
|            | 인기 숙소 Top6 조회 | 별점 기반 Top6 숙소 추천      |                   |
|            | 인기 지역 Top6 조회 | 최근 예약이 많았던 숙소 위치 기반의 6개 지역 제공 |                |
|            | 유튜브 영상 조회    | 핫한 여행지 기준 유튜브 영상 API 조회 |               |
| 마이 페이지 | 회원 정보 수정      | 회원가입시 제공한 데이터 수정    | 회원(이용자/관리자/사업자) |
|            | 회원 탈퇴           | 회원 탈퇴                     |                   |
|            | 예약 내역 조회      | 예약 내역 확인, 취소 및 수정, 스케줄링 통한 예약일 확인 및 변경 |  |
| 로그인/로그아웃 | 로그인           | 회원 이메일, 비밀번호 입력     |              |
|            | 로그아웃           | 로그아웃                       | 회원(이용자/관리자/사업자) |
| 회원가입     | 회원가입           | 이름, 이메일, 비밀번호, 회원 종류, 핸드폰 번호, 생년월일 입력 | 비회원 |
|            | 이메일 인증        | Gmail SMTP 사용한 메일 전송   |                   |
| 숙소 리스트  | 모든 숙소 조회      | 등록되어진 모든 숙소 조회      |             |
|            | 검색 기반 숙소 조회 | 검색 키워드 및 입/퇴실 날짜 기반 숙소 조회 |              |
| 숙소 상세    | 숙소 상세 내역 조회 | 숙소 사진, 숙소명, 위치, 가격 등의 숙박업소 상세 내역 조회 |  |
|            | 숙소 내역 수정      | 숙소 사진, 숙소명, 위치, 가격 등의 숙박업소 상세 내역 수정 | 사업자(본인이 등록한 숙소) |
|            | 숙소 삭제           | 본인이 등록한 숙소에 한해서, 숙소 정보가 이용자에게 노출되지 않도록 비활성화 | |
|            | 방 정보 조회       | 숙소에 있는 방에 대한 정보 조회 |  |
|            | 방 정보 수정       | 방의 정보 수정                | 사업자(본인이 등록한 숙소) |
|            | 방 비활성화       | 해당 방을 비활성화해 이용자에게 노출X |              |
|            | 예약               | 방 예약                       | 사업자(본인이 등록한 숙소) |
| 숙소 관리   | 숙박업소 조회       | 등록된 업소들 조회             | 회원(사업자)       |
|            | 숙박업소 등록       | 숙박업소 사진, 위치 등의 정보 등록 및 변경 |         |
|            | 숙박업소 수정       | 숙박업소 수정                 |         |
|            | 숙박업소 삭제       | 숙박업소 삭제                 |         |
| 예약 관리   | 예약 상세 조회 및 상태 변경 & Email 전송 | 사업자(본인이 등록한 숙소) |
| 관리자 페이지 | 회원 조회        | 모든 회원 조회                 | 관리자            |
|            | 회원 검색           | 회원 이름 검색을 통한 회원 정보 조회 |             |
|            | 회원 탈퇴           | 관리자 권한으로 회원 강제 탈퇴 |               |
|            | 회원 권한 변경      | 숙박업자, 사용자, 탈퇴자로 권한 변경 |              |


<br><br>


## 데이터베이스 모델링(ERD)  

![image]()

① 크게 회원테이블, 영화 테이블, 리뷰 테이블, 배우 테이블, 배역 테이블, 리뷰 좋아요 테이블 나누었습니다.    
② 배우와 영화 테이블 간에 배역 중간 테이블을 두어 매핑하였습니다.
③ 이미지가 필요한 테이블은 첨부파일 테이블을 별도로 두어 관리하였습니다.(예정)

![ERD](https://github.com/user-attachments/assets/f7c2905c-9cfd-4b1c-926c-d574c5b43f01)

<br><br>
##  API 명세서

![image]()

<br><br>

## :factory: Architecture
![image]()

<br><br>

##  프로젝트 구조
### FE + BE

📂 gradle  
📂 src  
┣ 📂 main  
┃ ┗ 📂 java  
┃ ┃ ┗ 📂 com   
┃ ┃ ┃ ┗ 📂 example
┃ ┃ ┃ ┃ ┃ 📂 miki7
┃ ┃ ┃ ┃ ┃ ┗ 📂 actor     
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 controller
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 db
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 model    
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 service   
┃ ┃ ┃ ┃ ┃ ┗ 📂 cast   
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 controller
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 db   
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 model   
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 service   
┃ ┃ ┃ ┃ ┃ ┗ 📂 common
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 controller       
┃ ┃ ┃ ┃ ┃ ┗ 📂 config   
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 SecurityConfig             
┃ ┃ ┃ ┃ ┃ ┗ 📂 movie
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 controller     
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 db   
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 model       
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 service   
┃ ┃ ┃ ┃ ┃ ┗ 📂 review  
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 controller   
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 db   
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 model       
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 service        
┃ ┃ ┃ ┃ ┃ ┗ 📂 user    
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 controller   
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 db    
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 model       
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂 service
┃ ┃ ┃ ┃ ┃ ┗ 📜 Miki7Application
┃ ┃ ┗ 📂 resources    
┃ ┃ ┃ ┗ 📂 static     
┃ ┃ ┃ ┃ ┗ 📂 css    
┃ ┃ ┃ ┃ ┃ ┗ 📜 app.css
┃ ┃ ┃ ┃ ┃ ┗ 📜 sb-admin.css
┃ ┃ ┃ ┃ ┃ ┗ 📜 theme.css
┃ ┃ ┃ ┗ 📂 img
┃ ┃ ┃ ┃ ┗ 📜 av.png
┃ ┃ ┃ ┃ ┗ 📜 card1.jpg
┃ ┃ ┃ ┃ ┗ 📜 logo.png
┃ ┃ ┃ ┃ ┗ 📜 screenshot.jpg
┃ ┃ ┃ ┃ ┗ 📜 undraw_posting_photo.svg
┃ ┃ ┃ ┃ ┗ 📜 undraw_profile.svg
┃ ┃ ┃ ┃ ┗ 📜 undraw_profile_1.svg
┃ ┃ ┃ ┃ ┗ 📜 undraw_profile_2.svg
┃ ┃ ┃ ┃ ┗ 📜 undraw_profile_3.svg
┃ ┃ ┃ ┃ ┗ 📜 undraw_rocket.svg
┃ ┃ ┃ ┗ 📂 js    
┃ ┃ ┃ ┃ ┗ 📂 demo
┃ ┃ ┃ ┃ ┃ ┗ 📜 chart-area-demo.js
┃ ┃ ┃ ┃ ┃ ┗ 📜 chart-bar-demo.js
┃ ┃ ┃ ┃ ┃ ┗ 📜 chart-pie-demo.js
┃ ┃ ┃ ┃ ┃ ┗ 📜 datatables-demo.js
┃ ┃ ┃ ┃ ┗ 📜 app.js      
┃ ┃ ┃ ┃ ┗ 📜 sb-admin-2.js     
┃ ┃ ┃ ┃ ┗ 📜 theme.js
┃ ┃ ┃ ┗ 📂 scss
┃ ┃ ┃ ┃ ┗ 📂 nav
┃ ┃ ┃ ┃ ┃ ┗ 📜 _global.scss
┃ ┃ ┃ ┃ ┃ ┗ 📜 _sidebar.scss
┃ ┃ ┃ ┃ ┃ ┗ 📜 _topbar.scss
┃ ┃ ┃ ┃ ┗ 📂 utilities
┃ ┃ ┃ ┃ ┃ ┗ 📜 _animation.scss
┃ ┃ ┃ ┃ ┃ ┗ 📜 _background.scss
┃ ┃ ┃ ┃ ┃ ┗ 📜 _border.scss
┃ ┃ ┃ ┃ ┃ ┗ 📜 _display.scss
┃ ┃ ┃ ┃ ┃ ┗ 📜 _progress.scss
┃ ┃ ┃ ┃ ┃ ┗ 📜 _rotate.scss
┃ ┃ ┃ ┃ ┃ ┗ 📜 _text.scss
┃ ┃ ┃ ┃ ┗ 📜 _buttons.scss
┃ ┃ ┃ ┃ ┗ 📜 _cards.scss
┃ ┃ ┃ ┃ ┗ 📜 _charts.scss
┃ ┃ ┃ ┃ ┗ 📜 _dropdown.scss
┃ ┃ ┃ ┃ ┗ 📜 _error.scss
┃ ┃ ┃ ┃ ┗ 📜 _footer.scss
┃ ┃ ┃ ┃ ┗ 📜 _global.scss
┃ ┃ ┃ ┃ ┗ 📜 _login.scss
┃ ┃ ┃ ┃ ┗ 📜 _mixins.scss
┃ ┃ ┃ ┃ ┗ 📜 _navs.scss
┃ ┃ ┃ ┃ ┗ 📜 _utilities.scss
┃ ┃ ┃ ┃ ┗ 📜 _variables.scss
┃ ┃ ┃ ┃ ┗ 📜 sb-admin-2.scss
┃ ┃ ┃ ┗ 📂 vendor
┃ ┃ ┃ ┃ ┗ 📂 bootstrap
┃ ┃ ┃ ┃ ┗ 📂 chart.js
┃ ┃ ┃ ┃ ┗ 📂 datatables
┃ ┃ ┃ ┃ ┗ 📂 fontawesome-free
┃ ┃ ┃ ┃ ┗ 📂 jquery
┃ ┃ ┃ ┃ ┗ 📂 jquery-easing
┃ ┃ ┃ ┃ ┗ 📜 favicon.ico
┃ ┃ ┗ 📂 templates       
┃ ┃ ┃ ┗ 📂 fragments
┃ ┃ ┃ ┃ ┗ 📜 detailsearch.html      
┃ ┃ ┃ ┃ ┗ 📜 footer.html         
┃ ┃ ┃ ┃ ┗ 📜 mainheader.html      
┃ ┃ ┃ ┃ ┗ 📜 topbar.html      
┃ ┃ ┃ ┗ 📜 author.html     
┃ ┃ ┃ ┗ 📜 index.html      
┃ ┃ ┃ ┗ 📜 login.html      
┃ ┃ ┃ ┗ 📜 post.html      
┃ ┃ ┃ ┗ 📜 register.html     
┃ ┃ ┃ ┗ 📜 result.html     
┃ ┃ ┃ ┗ 📜 review-form.html
┃ ┃ ┗ 📜 application.yaml
┃ ┃ ┗ 📜 data.sql
┣ 📂 test  
┃ ┣ 📂 java
┃ ┃ ┣ 📂 com.example.miki7
┃ ┃ ┃ ┣ 📜 Miki7ApplicationTests
┃ ┃ ┃ ┣ 📜 PasswordEncoderTest
┣ 📜 .env    
┣ 📜 .gitattributes    
┣ 📜 build.gradle    
┣ 📜 gradlew
┣ 📜 gradlew.bat
┣ 📜 settings.gradle

<br><br>

## UI
- 숙소 정보 수정
  ![숙소 정보 수정](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/fa69957a-9d57-49f8-9a8a-73e322d31ed2)  
- 내 숙소 관리
  ![내 숙소 과닐](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/34b4e460-8762-4371-bb2a-aca56d1caa2a)  
- 예약 페이지
  ![예약 페이지](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/ff1d239d-f12c-4a5e-a20b-dfa915009827)  
- 리스트 페이지
  ![리스트 페이지](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/40c733cc-4a19-4d8f-804b-1d09dca72d8f)  
- 마이페이지
  ![내정보 수정](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/61a75236-f712-4f63-903d-da2744b2b753)  
- 내 예약 내역
  ![내 예약내역](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/b3944edb-93f5-4b53-bde4-10932d435835)  
- 회원가입
  ![회원가입](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/25b49b0f-d765-45e9-b160-45457bbaa32b)  
- 로그인
  ![로그인](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/6e20618c-7edf-43b9-848e-7d6225ad1a02)  
- 관리자 페이지
  ![관리자 페이지](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/2b89a78f-96e7-4164-bb84-4d987b005816)  
- 숙소 상세  
  ![숙소상세페이지](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/877761e0-6afa-44a9-a734-8576387db7b4)  
- 메인 페이지  
  ![메인페이지](https://github.com/anonymousOrmi/simsasookbak/assets/42295097/68c29836-ff61-46da-81e1-6995fd9dc4b1)  

<br><br>
## 개발 이슈
- 앨런 데이터 가공 

🔗 [이슈 목록 상세 확인](https://github.com/anonymousOrmi/simsasookbak/issues?q=is%3Aissue+is%3Aclosed)

<br><br>
## 개발 회고
### 🧑‍💻 이영석  

### 🧑‍💻 김나경  

### 🧑‍💻 박성준
