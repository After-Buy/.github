# After Buy

<img width="1491" height="1055" alt="프로젝트 소개 이미지" src="https://github.com/user-attachments/assets/90f5b766-3eb5-4d05-b6ee-7c1c0f16b22e" />

> 전자제품 등록부터 보증기간 관리까지, 한 번에

After Buy는 전자제품의 구매 정보, 보증기간, 영수증, 시리얼 넘버를 쉽고 깔끔하게 관리할 수 있도록 돕는 전자제품 보증 관리 서비스입니다.

사용자는 전자제품을 간편하게 등록하고, OCR을 통해 제품 정보와 구매 정보를 자동으로 추출하며, 보증기간 만료 전에 알림을 받을 수 있습니다.

---

## Problem & Solution

### Problem

전자제품을 구매한 뒤 시간이 지나면 구매일, 영수증, 보증기간, 모델명, 시리얼 넘버와 같은 정보를 다시 찾기 어려워집니다.

특히 보증기간이 지나기 전 수리나 교환이 필요해도 사용자가 직접 구매 정보를 기억하거나 영수증을 찾아야 하는 불편함이 있습니다.

### Solution

After Buy는 전자제품 구매 이후의 관리 과정을 하나의 서비스 안에서 해결합니다.

사용자는 전자제품을 등록하고, 제품 라벨과 영수증 이미지를 기반으로 주요 정보를 자동 입력할 수 있습니다.
또한 등록된 보증기간을 기준으로 만료 예정 알림을 받아 필요한 시점을 놓치지 않고 관리할 수 있습니다.

---

## Tech Stack

### Frontend

![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge\&logo=react\&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=for-the-badge\&logo=expo\&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge\&logo=react\&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge\&logo=vite\&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge\&logo=typescript\&logoColor=white)

### Backend

![Java 21](https://img.shields.io/badge/Java_21-007396?style=for-the-badge\&logo=openjdk\&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge\&logo=springboot\&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge\&logo=springsecurity\&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge\&logo=jsonwebtokens\&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=for-the-badge)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge\&logo=swagger\&logoColor=black)

### Database & Infra

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge\&logo=mysql\&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon_S3-569A31?style=for-the-badge\&logo=amazons3\&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/AWS_Lambda-FF9900?style=for-the-badge\&logo=awslambda\&logoColor=white)
![Amazon Textract](https://img.shields.io/badge/Amazon_Textract-FF9900?style=for-the-badge\&logo=amazonaws\&logoColor=white)
![Firebase FCM](https://img.shields.io/badge/Firebase_FCM-FFCA28?style=for-the-badge\&logo=firebase\&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge\&logo=docker\&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge\&logo=nginx\&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge\&logo=githubactions\&logoColor=white)

---

## Main Features

### 제품 등록 및 관리

전자제품의 모델명, 시리얼 넘버, 구매일, 구매처, 구매가격, 보증기간을 등록하고 관리할 수 있습니다.

### OCR 자동 입력

제품 라벨과 영수증 이미지를 분석하여 모델명, 시리얼 넘버, 구매일, 구매처, 구매가격 정보를 자동으로 추출합니다.

### 보증기간 알림

등록된 제품의 보증기간을 기준으로 만료 예정 알림을 제공하여 사용자가 필요한 시점을 놓치지 않도록 돕습니다.

### 관리자 운영

관리자 웹을 통해 공지사항, FAQ, 에러 로그, 사용자 및 서비스 통계를 관리할 수 있습니다.

---

## User Flow

```text
제품 등록
   ↓
제품 라벨 또는 영수증 이미지 업로드
   ↓
OCR을 통한 제품 정보 및 구매 정보 추출
   ↓
모델명, 시리얼 넘버, 구매일, 구매처, 보증기간 저장
   ↓
보증기간 만료 예정일 기준 알림 발송
   ↓
사용자는 만료 전에 수리, 교환, AS 여부 확인
```

---

## Architecture

<img width="1535" height="1024" alt="시스템 아키텍처" src="https://github.com/user-attachments/assets/f352f155-7a29-454d-84f3-7a8b7e64e190" />

---

## ERD

<img width="1700" height="1082" alt="ERD" src="https://github.com/user-attachments/assets/4bb7d62b-a61c-4df5-8a3d-e2ff4f593399" />

---

## Key Highlights

### 마이크로서비스 기반 구조

인증, 기기 관리, 알림, 관리자 기능을 각각 독립된 서비스로 분리하여 서비스별 책임을 명확하게 나누었습니다.

### OCR 기반 입력 자동화

사용자가 직접 입력해야 하는 모델명, 시리얼 넘버, 구매일, 구매처, 구매가격 등의 정보를 이미지 기반으로 추출하여 입력 과정을 줄였습니다.

### 보증기간 기반 알림 자동화

등록된 전자제품의 보증기간을 기준으로 만료 예정 알림을 생성하고, FCM을 통해 사용자에게 푸시 알림을 전송합니다.

### 사용자 앱과 관리자 웹 분리

일반 사용자를 위한 모바일 앱과 서비스 운영을 위한 관리자 웹을 분리하여 사용자 기능과 운영 기능을 독립적으로 관리할 수 있도록 구성했습니다.

### 클라우드 기반 OCR 처리

OCR 처리는 AWS Lambda와 Amazon Textract를 활용하여 서버리스 방식으로 분리했습니다.

---

## Services

### Auth Service

카카오 로그인, JWT 인증, 사용자 프로필, 회원 탈퇴 처리를 담당합니다.

### Device Service

전자제품 등록, 구매 정보 관리, 보증기간 관리, OCR 연동을 담당합니다.

### Notification Service

보증기간 알림, FCM 푸시, 알림 설정 관리를 담당합니다.

### Admin Service

관리자 인증, 공지사항, FAQ, 에러 로그, 통계 관리를 담당합니다.

### OCR Lambda

제품 라벨과 영수증 이미지를 분석하여 필요한 정보를 추출합니다.

---

## Repositories

| Repository                                                                                    | Description               |
| --------------------------------------------------------------------------------------------- | ------------------------- |
| [after-buy-app](https://github.com/After-Buy/after-buy-app)                                   | React Native 기반 사용자 모바일 앱 |
| [after-buy-admin](https://github.com/After-Buy/after-buy-admin)                               | React 기반 관리자 웹            |
| [after-buy-auth-service](https://github.com/After-Buy/after-buy-auth-service)                 | 사용자 인증 및 회원 관리 서비스        |
| [after-buy-device-service](https://github.com/After-Buy/after-buy-device-service)             | 전자제품 등록 및 관리 서비스          |
| [after-buy-notification-service](https://github.com/After-Buy/after-buy-notification-service) | 보증기간 알림 및 푸시 알림 서비스       |
| [after-buy-admin-service](https://github.com/After-Buy/after-buy-admin-service)               | 관리자 API 서비스               |
| [after-buy-ocr-lambda](https://github.com/After-Buy/after-buy-ocr-lambda)                     | AWS Lambda 기반 OCR 처리 함수   |
| [after-buy-infra](https://github.com/After-Buy/after-buy-infra)                               | 인프라 및 배포 설정               |

---

## Team

<table>
  <tr>
    <td align="center" width="20%">
      <a href="https://github.com/JJitHub21">
        <img src="https://avatars.githubusercontent.com/JJitHub21" width="72" height="72" alt="김진우" />
      </a>
      <br />
      <b>김진우</b>
      <br />
      <sub>Frontend</sub>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/chuchun4999">
        <img src="https://avatars.githubusercontent.com/chuchun4999" width="72" height="72" alt="한지성" />
      </a>
      <br />
      <b>한지성</b>
      <br />
      <sub>Frontend</sub>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/junhyeok020630">
        <img src="https://avatars.githubusercontent.com/junhyeok020630" width="72" height="72" alt="최준혁" />
      </a>
      <br />
      <b>최준혁</b>
      <br />
      <sub>Backend</sub>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/tastysoapwater">
        <img src="https://avatars.githubusercontent.com/tastysoapwater" width="72" height="72" alt="신태훈" />
      </a>
      <br />
      <b>신태훈</b>
      <br />
      <sub>Backend</sub>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/HYUNJOON-SUNG">
        <img src="https://avatars.githubusercontent.com/HYUNJOON-SUNG" width="72" height="72" alt="성현준" />
      </a>
      <br />
      <b>성현준</b>
      <br />
      <sub>Cloud & Infra</sub>
    </td>
  </tr>
</table>
