# Commitment

> Welcome to [Commit your moment](http://i4a308.p.ssafy.io/) :globe_with_meridians:
![image](https://user-images.githubusercontent.com/40655666/114405911-13152880-9be2-11eb-8614-a2976f74f83e.png)

<br>

## Member :family:

![](Document/Images/team.jpg)

### Contact :green_book:

박영철 [Github](https://github.com/dudcheol) 🐹

강해성 [Github](https://github.com/Haesungkang) 🐶

박소현 [Github](https://github.com/dbdtrapper) 🐱

김청화 [Github](https://github.com/cheonghwakim ) 🐯

박유정 [Github](https://github.com/ParkYooJeong/ParkYooJeong) 🐭

<br>

## Project Summary 🧭

- Purpose

  Github의 잔디 심기에서 아이디어를 얻어와 탄생한 여행 기록 웹서비스입니다.

  전국을 여행다니며 우리나라 지도를 채우고, 도전과제를 수행하며 여행의 재미를 두배로 느낄수 있도록 제작하였습니다 .

  또한 나만의 지도를 자랑할 수 있게 SNS형태를 만들고, 위치기반으로 서로 소통할 수 있는 공간을 마련했습니다. 

  > Commitment ❔
  >
  >  Commit your mement의 줄임말 으로써 지금의 소중한 순간을 기록하자는 의미입니다. 

- Duration

  Jan 11th 2021 ~ Feb 19th 2021

- Results

  - [PPT](Document/PPT/3반_8조_공통프로젝트_최종발표.pdf)
  - [시연영상](https://www.youtube.com/watch?v=t04WiXnqpVA)
  - [UCC](https://www.youtube.com/watch?v=eecCNU4JMsI)
  
<br>

## Project Info :pushpin:

### Tech Stack 🧩

![](Document/Images/techstack.jpg)

### Usage 🎈

#### Front-end

- Project Setup

  - ```bash
    $ npm install 
    ```
  
- Compiles and hot-reloads for development

  - ```bash
    $ npm run serve
    ```
  
- Compiles and minifies for production

  - ```bash
    $ npm run build
    ```
    
  
-  Run your tests

  - ```bash
    $ npm run test
    ```

-  Lints and fixes files

  - ```bash
    $ npm run lint
    ```

-  Customize configuration

  - [Configuration Reference](https://cli.vuejs.org/config/)

#### Back-end

**Install**

- Java (Open JDK 14)

- Maven

- STS 

- Docker

  - Start Maria DB Container

    ```bash
    docker run --name-db -p 3306:3306 -e MYSQL_ROOT_PASSWORD={your_password} -d mariddb
    ```

    ```bash
    docker exec -it maria-db mysql -u root -p
    ```

  - Create DB table

### Database Modeling :link:

   ![210125_DB 설계](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/ERD.PNG)

<br>

### Features :sparkles:

> 주요기능 소개 및 설명

- 커밋 지도

  - 현재위치를 기반으로 기록 저장가능
  - 기록만 하고 추후 게시글 및 이미지 게시가능

- 위치기반 SNS

  - 현재 위치를 기반으로 주변 게시글 확인 
  - 반경설정을 통해 원하는 위치까지 게시글 조회 

- 도전과제 & 랭킹

  - 각 지역별 & 기록수 기반으로 도전과제 수행가능 
  - 지역별 기록 전체 랭킹 조회
  - 내가 팔로우한 유저 기준으로 랭킹 확인 

- 타임라인

  - 자신의 기록을 타임라인으로 한눈에 확인 가능

    

<br>

### Pages in Detail :mag:

> 각 페이지별 소개

> PPT 참고
### 로그인 
![로그인](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EB%A1%9C%EA%B7%B8%EC%9D%B8.PNG)

### 메인페이지
![메인페이지1](https://user-images.githubusercontent.com/43662673/108456760-6212a180-72b4-11eb-9f10-bf0515bb302e.png)
![메인페이지2](https://user-images.githubusercontent.com/43662673/108456763-6343ce80-72b4-11eb-98a9-bd0582c9ce98.png)
![스크린샷 2021-02-22 오후 7 06 42](https://user-images.githubusercontent.com/40655666/114405812-fe389500-9be1-11eb-830e-e41984af143d.png)


### 실시간 알림
![실시간 알림](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EC%8B%A4%EC%8B%9C%EA%B0%84%EC%95%8C%EB%A6%BC.PNG)

### 커밋 클릭시
![커밋 클릭시](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EC%BB%A4%EB%B0%8B.PNG)
![image](https://user-images.githubusercontent.com/40655666/114405645-db0de580-9be1-11eb-8347-891d719a59c9.png)


### 커밋 후(연속커밋 방지를 위해 1분 시간제한)
![커밋 후](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EC%BB%A4%EB%B0%8B%ED%9B%84.PNG)

### 마이페이지 - 타임라인
![마이페이지](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%ED%83%80%EC%9E%84%EB%9D%BC%EC%9D%B8.PNG)

### 마이페이지 - 커밋지도
![마이페이지](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EB%A7%88%EC%9D%B4%ED%8E%98%EC%9D%B4%EC%A7%80.PNG)
![스크린샷 2021-02-22 오후 7 09 57](https://user-images.githubusercontent.com/40655666/114406291-625b5900-9be2-11eb-8c90-2b4b9d7ca609.png)


### 위치반경 SNS
![위치 반경1](https://user-images.githubusercontent.com/43662673/108456783-7060bd80-72b4-11eb-80e4-939e73e49fd1.png)
![위치 반경2](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EC%9C%84%EC%B9%98%EB%B0%98%EA%B2%BD+SNS.PNG)
![스크린샷 2021-02-22 오후 7 10 31](https://user-images.githubusercontent.com/40655666/114406475-89198f80-9be2-11eb-8cbf-d524b2d16c16.png)
![스크린샷 2021-02-22 오후 7 10 41](https://user-images.githubusercontent.com/40655666/114406489-8c148000-9be2-11eb-9f47-db67f0cd625f.png)


### 게시글 상세
![게시글 상세](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EA%B2%8C%EC%8B%9C%EA%B8%80+%EC%83%81%EC%84%B81.PNG)
![게시글 상세](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EA%B2%8C%EC%8B%9C%EA%B8%80+%EC%83%81%EC%84%B82.PNG)
![image](https://user-images.githubusercontent.com/40655666/114405312-88ccc480-9be1-11eb-80ed-c8829b21673b.png)
![image](https://user-images.githubusercontent.com/40655666/114405214-6cc92300-9be1-11eb-9513-052528e64e77.png)


### 랭킹페이지
![랭킹페이지](https://user-images.githubusercontent.com/43662673/108456769-65a62880-72b4-11eb-975e-7ec888624a5b.png)

### 찜목록
![찜목록](https://commitmentbucket.s3.ap-northeast-2.amazonaws.com/%ED%99%94%EB%A9%B4%EC%BA%A1%EC%B2%98/%EC%B0%9C%EB%AA%A9%EB%A1%9D.PNG)

### 지역별 커밋지도
![스크린샷 2021-03-09 오후 8 55 50](https://user-images.githubusercontent.com/40655666/114405445-a8fc8380-9be1-11eb-8335-8447f34e2e44.png)
![스크린샷 2021-03-09 오후 8 55 54](https://user-images.githubusercontent.com/40655666/114405448-aa2db080-9be1-11eb-9ec2-bbcc91ea16e9.png)
![스크린샷 2021-03-09 오후 8 55 57](https://user-images.githubusercontent.com/40655666/114405452-aac64700-9be1-11eb-8790-a3911432c7a8.png)
![스크린샷 2021-03-09 오후 8 56 06](https://user-images.githubusercontent.com/40655666/114405455-aac64700-9be1-11eb-8dda-52f7916ca13b.png)
![스크린샷 2021-03-09 오후 8 56 09](https://user-images.githubusercontent.com/40655666/114405456-ab5edd80-9be1-11eb-9419-67cc2ccd9176.png)
![스크린샷 2021-03-09 오후 8 56 17](https://user-images.githubusercontent.com/40655666/114405458-abf77400-9be1-11eb-9c89-ac74a5a2b675.png)
![스크린샷 2021-03-09 오후 8 56 24](https://user-images.githubusercontent.com/40655666/114405464-ac900a80-9be1-11eb-93cc-2153ff36429a.png)


<br>

### Tech log :bookmark:

<details>
<summary>Scrum</summary>
    <ul>
        <a href="Document/Tech_Log/Scrum/1월4주차_회의록.md"><li>1월 4주차</li></a>
        <a href="Document/Tech_Log/Scrum/1월5주차_회의록.md"><li>1월 5주차</li></a>
    <a href="Document/Tech_Log/Scrum/2월1주차_회의록.md"><li>2월 1주차</li></a>
        <a href="Document/Tech_Log/Scrum/2월2주차_회의록.md"><li>2월 2주차</li></a>
        <a href="Document/Tech_Log/Scrum/2월3주차_회의록.md"><li>2월 3주차</li></a>
    </ul>
</details>
<details>
<summary>Project Proposal and WireFrame</summary>
    <ul>
        <a href="Document/Tech_Log/Project_Proposal/Project_Proposal.md"><li>프로젝트 기획안</li></a>
    <a href="https://www.figma.com/file/D5d31VoT1Q3PfwKHgMWRkX/SSAFY-project-1"><li>와이어프레임</li></a>
    </ul>
</details>
<details>
<summary>Video Proposal</summary>
    <ul>
        <a href="Document/Tech_Log/Video/Video_Proposal.md"><li>영상기획안</li></a>
    </ul>
    <ul>
        <a href="Document/PPT/3반_8조_공통프로젝트_최종발표.pdf"><li>PPT</li></a>
    </ul>
</details>



