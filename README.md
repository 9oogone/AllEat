# 식단·식비 통합 자동 관리 서비스 : AllEat!
- 진행 기간 : 2024.08.26 ~ 2024.10.11
- 서비스명 : AllEat!
- 서비스 소개 : AI를 활용한 식단·식비 통합 자동 관리 핀테크 서비스

## ◽ 프로젝트 소개
![AllEat](readmeimg/main.png)

### 페르소나

- 균형 잡힌 식단을 원하면서도 합리적인 지출 관리에 서툰 사람
- 지출 비용은 낮췄으나 필수 영양소 섭취가 부족한 사람
- 식단 및 식비 수기 작성 때문에 어플 사용이 불편한 사람

### 기능 소개
<details>
<summary><b>1. 거래 내역 기반 자동 기록 시스템</b></summary>
<br>
사용자가 '페이머니'를 통해 지출한 식비 내역을 실시간으로 분석하여 자동으로 기록합니다. 충전식 결제 데이터를 기반으로 소비 패턴을 추적하며, 별도의 수기 입력 없이도 정확한 식비 관리가 가능합니다.
</details>

<details>
<summary><b>2. YOLOv10 & ResNet 기반 AI 식단 인식</b></summary>
<br>
YOLOv10 객체 탐지 모델을 활용하여 식단 사진 촬영 시 메뉴를 자동 식별합니다. ResNet 모델을 사용하여 양을 추정합니다.식별된 메뉴를 바탕으로 칼로리 및 영양 정보를 자동 추출하며, 불확실한 메뉴 정보에 대한 데이터 객관성을 확보합니다.
</details>

<details>
<summary><b>3. 통합 분석 레포트 및 맞춤형 피드백</b></summary>
<br>
기록된 데이터를 시각화하여 일간·주간·월간 레포트를 제공합니다. 
특히 <b>'식비 효율성'</b>과 <b>'영양소 섭취 균형'</b>을 교차 분석하여, 예산 초과나 영양 불균형 발생 시 개선 방향을 제시하는 맞춤형 피드백 시스템을 가동합니다.
</details>


### 기대효과

**자동 결제 내역 연동을 통한 사용자 편의성 극대화**  
수기 입력 과정을 최소화하여 사용자의 번거로움을 해결하고 가계부 작성의 진입장벽을 낮춥니다.

**AI 기반의 객관적인 식단 분석 및 등록**  
정확한 정보 확인이 어려운 메뉴도 AI 사진 분석을 통해 데이터화하며, 기록의 객관성과 신뢰도를 확보합니다.

**식단·지출 통합 관리를 통한 데이터 인사이트 제공**  
식습관과 소비 패턴을 결합한 통합 레포트를 제공하여, 효율적인 영양 섭취와 합리적인 지출 관리를 동시에 실현합니다.



## ◽ 프로젝트 산출물
<details>
<summary><b>시퀀스 다이어그램 / 플로우 차트</b></summary>
<br>

> 🔗 **[Figma 바로가기](https://www.figma.com/board/LNHvyWWpNPSdRtDbChgeH0/Flow-Chart?node-id=0-1&t=6hRLYmyGvSfEzZ6r-1)**  

**◽시퀀스 다이어그램**  

| 회원가입 | 배달앱 결제 |
| :---: | :---: |
| ![회원가입 시퀀스](./readmeimg/signupdi.png) | ![배달앱 결제 시퀀스](./readmeimg/deliverydi.png) |

| 마트 결제 | 식당 결제 |
| :---: | :---: |
| ![마트 결제 시퀀스](./readmeimg/martdi.png) | ![식당 결제 시퀀스](./readmeimg/restaurantdi.png) |  

**◽플로우 차트**
![플로우차트](./readmeimg/flowchart.png)

</details>

<details>
<summary><b>API 명세서</b></summary>
<br>  

> 🔗 **[Notion 바로가기](https://ring-barracuda-ca0.notion.site/API-fb4d9e04b25e4ef3a6ddb387e7ef43be)**  

![API명세서0](./readmeimg/image(5).png)
![API명세서1](./readmeimg/image(6).png)
![API명세서2](./readmeimg/image(7).png)
![API명세서3](./readmeimg/image(8).png)
![API명세서4](./readmeimg/image(9).png)
</details>

<details>
<summary><b>ERD</b></summary>
<br>

![ERD](./readmeimg/erd.png) 

</details>

<details>
<summary><b>화면 정의서</b></summary>
<br>  

> 🔗 **[Figma 바로가기](https://www.figma.com/design/0IExZ6iqKqPp9Pdy8HhAZ4/%ED%99%94%EB%A9%B4%EC%A0%95%EC%9D%98%EC%84%9C?node-id=0-1&t=KwG8Nf9NkKd1zOr0-1)**  

초기 페이지|로그인 페이지|회원 가입|메인 페이지
-----|-----|-----|-----
![초기페이지](readmeimg/startpage.png)|![로그인페이지](readmeimg/signin.png)|![회원가입](readmeimg/signup.png)|![메인페이지](readmeimg/myhome.jpg)

식단 등록|메뉴 등록|사진 등록|수기 등록
-----|-----|-----|-----
![식단등록](readmeimg/create-oreo.png)|![메뉴등록](readmeimg/add-menu.png)|![카메라](readmeimg/camera.png)|![수기등록](readmeimg/create-menu.png)

일간 레포트|주간 레포트|월간 레포트|식비 내역
-----|-----|-----|-----
![일간](readmeimg/dayreport.png)|![주간](readmeimg/weekreport.png)|![월간](readmeimg/monthreport.png)|![식비내역](readmeimg/logpage.png)

페이 머니|마이 페이지|내 정보 수정|---
-----|-----|-----|-----
![페이머니](readmeimg/paymoney.png)|![마이페이지](readmeimg/mypage.png)|![업데이트](readmeimg/mypageupdate.png)|---

</details>


## ◽ 기술 스택 및 개발 환경

### 📱 Frontend
<img src="https://img.shields.io/badge/React%20Native-61DAFB?style=flat-square&logo=react&logoColor=black"/><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/><img src="https://img.shields.io/badge/Redux%20Toolkit-593D88?style=flat-square&logo=redux&logoColor=white"/><img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/><img src="https://img.shields.io/badge/Axios-5A29E4?style=flat-square&logo=axios&logoColor=white"/><img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black"/>

### ⚙️ Backend
<img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/><img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white"/><img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/><img src="https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white"/>

### 🧠 AI & Database
<img src="https://img.shields.io/badge/YOLOv10-FF4B4B?style=flat-square&logo=python&logoColor=white"/><img src="https://img.shields.io/badge/ResNet-FF4B4B?style=flat-square&logo=pytorch&logoColor=white"/><img src="https://img.shields.io/badge/OpenAI%20API-412991?style=flat-square&logo=openai&logoColor=white"/><img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>

### 🏗 Infra & DevOps
<img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white"/><img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/><img src="https://img.shields.io/badge/NGINX-009639?style=flat-square&logo=nginx&logoColor=white"/><img src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white"/><img src="https://img.shields.io/badge/Certbot-003A70?style=flat-square&logo=letsencrypt&logoColor=white"/>

### 🛠 Collaboration & Tools
<img src="https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=gitlab&logoColor=white"/><img src="https://img.shields.io/badge/Jira-0052CC?style=flat-square&logo=jira&logoColor=white"/><img src="https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white"/><img src="https://img.shields.io/badge/Mattermost-0058CC?style=flat-square&logo=mattermost&logoColor=white"/>

![architecture](./readmeimg/arch.png)

### 🎯 기술 도입 배경 (Tech Stack Rationale)

| 분류 | 기술 스택 | 도입 목적 및 의사결정 근거 |
| :--- | :--- | :--- |
| **Client** | **React Native** | iOS 및 Android 크로스 플랫폼 앱의 동시 릴리즈를 통한 개발 비용 단축 및 단일 코드베이스 유지보수. |
| **Main API** | **Spring Boot** | '결제 내역'과 '식비'라는 정합성이 필수적인 데이터를 다루므로, 강력한 트랜잭션 관리(JPA)와 안정성이 검증된 프레임워크 채택. |
| **AI Serving**| **FastAPI** | YOLOv10, ResNet 등 Python 기반 AI 모델 서빙에 최적화. 비동기 처리(Asynchronous)를 통해 이미지 추론 시 발생하는 병목 현상 최소화. |
| **AI Model** | **YOLOv10 / ResNet** | 식단 이미지 내 음식 객체의 실시간 탐지(YOLO) 및 양 추정(ResNet) 연계를 통해 사용자의 수기 입력 프로세스 완전 자동화. |
| **DevOps** | **Docker / Jenkins** | Spring Boot(Java)와 FastAPI(Python)의 이기종 런타임 환경을 컨테이너로 격리하여 종속성 충돌을 방지하고, 자동화된 CI/CD 파이프라인 구축. |



## ◽ 팀원 및 역할
<div align="center">
<table>
  <tr>
    <td align="center">
      <img src="./readmeimg/최봉준.jpg" width="120"><br>
      <strong>최봉준</strong><br>
      팀장 / BE
    </td>
    <td align="center">
      <img src="./readmeimg/라송연.jpg" width="120"><br>
      <strong>라송연</strong><br>
      BE Leader
    </td>
    <td align="center">
      <img src="./readmeimg/김수민.jpg" width="120"><br>
      <strong>김수민</strong><br>
      Full Stack
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="./readmeimg/윤채영.jpg" width="120"><br>
      <strong>윤채영</strong><br>
      FE
    </td>
    <td align="center">
      <img src="./readmeimg/구고운.png" width="120"><br>
      <strong>구고운</strong><br>
      FE Leader
    </td>
    <td align="center">
      <img src="./readmeimg/김예운.jpg" width="120"><br>
      <strong>김예운</strong><br>
      FE
    </td>
  </tr>
</table>
</div>