# 💊 메디패스 (MediPass)

> **약 봉투 한 장이면, 해외 의약품 반입 준비가 끝납니다.**
>
> _“약 때문에 여행을 망설이지 않도록.”_

약 봉투를 촬영하면 복용 중인 의약품을 인식하고, 여행 국가의 규정에 따라 **반입 가능 여부 · 준비 서류 · 현지 대응 정보**를 한곳에서 안내하는 해외여행 의약품 관리 서비스입니다.

MediPass는 식약처 의약품 정보와 국가별 정부 원천 데이터를 바탕으로 의약품 성분을 확인합니다. 여행 전에는 필요한 준비를 체크리스트로 관리하고, 여행 중에는 재외공관 연락처와 현지어 설명문을 통해 긴급 상황에 대응할 수 있습니다.

---

## 🗂️ 레포지토리

| 레포지토리 | 설명 | 기술 스택 |
| --- | --- | --- |
| [MediPass-FE](https://github.com/Likelion14-InfinityStone/FE) | 모바일 웹 프론트엔드 | React · TypeScript · Vite |
| [MediPass-BE](https://github.com/Likelion14-InfinityStone/BE) | 백엔드 서버 | Spring Boot · Java 21 |

---

## ✨ 서비스 소개

### 약 봉투에서 출국 준비까지

```text
📷 약 봉투 촬영
      ↓
🔎 OCR 인식 · 식약처 의약품 매칭
      ↓
💳 한글·영문 복약 카드 생성
      ↓
✈️ 여행 국가 · 복용 의약품 선택
      ↓
🚦 국가별 반입 가능 여부 판정
      ↓
✅ 준비 서류 체크 · 증빙 서류 보관
      ↓
🆘 재외공관 연락처 · 현지어 설명문 제공
```

### 국가별 반입 판정

의약품의 성분, 소지량, 목적지 국가의 규정을 종합해 다음 3단계로 안내합니다.

| 판정 | 의미 | 안내 내용 |
| --- | --- | --- |
| ✅ **반입 가능** `ALLOWED` | 별도 제한 없이 반입 가능한 의약품 | 기본 휴대 및 보관 안내 |
| 📄 **서류 준비 필요** `PREP_REQUIRED` | 처방전·의사 소견서·허가서 등이 필요한 의약품 | 준비 항목과 공식 신청 페이지 제공 |
| ⛔ **반입 제한** `NOT_ALLOWED` | 반입이 제한되거나 관계 기관 확인이 필요한 의약품 | 판정 근거와 확인 기관 안내 |

> MediPass의 판정은 여행 준비를 돕기 위한 정보이며, 실제 반입 가능 여부는 출국 전 해당 국가의 최신 공식 지침을 함께 확인해야 합니다.

---

## 📱 주요 화면

<table>
  <tr>
    <td colspan="3" align="center"><b>로그인 · 온보딩</b></td>
  </tr>
  <tr>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/3984e5ab-1abb-4bc8-9079-08c86619ccec" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/a320d716-5f9e-4b6b-b198-f7016f9385c9" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/ccd1904b-a0f5-470e-8512-f2e687a88cf9" />
</td>
  </tr>
  <tr>
    <td align="center">로그인</td>
    <td align="center">서비스 소개</td>
    <td align="center">약관 동의</td>
  </tr>
</table>

<table>
  <tr>
    <td colspan="3" align="center"><b>약 봉투 스캔 · 복약 카드</b></td>
  </tr>
  <tr>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/0bfb9620-eca5-4969-a439-06f9fa6fe629" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/0baf0b6a-5f96-418f-a1b8-6cf213c735e6" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/065bbc0a-6179-4fa4-9a90-cacaca2971cc" />
</td>
  </tr>
  <tr>
    <td align="center">약 봉투 촬영</td>
    <td align="center">OCR 결과 확인</td>
    <td align="center">복약 카드</td>
  </tr>
</table>

<table>
  <tr>
    <td colspan="3" align="center"><b>여행 등록 · 반입 체크로그</b></td>
  </tr>
  <tr>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/0fe160da-b99d-459e-9d0f-1d22d513e6e0" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/43f2e213-cd2b-4458-82e1-2e9b33972171" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/faca379f-1f1b-4a11-a83b-2b30edac413e" />
</td>
  </tr>
  <tr>
    <td align="center">여행 정보 입력</td>
    <td align="center">의약품 선택</td>
    <td align="center">여행별 체크로그</td>
  </tr>
</table>

<table>
  <tr>
    <td colspan="3" align="center"><b>반입 판정 · 준비 체크리스트</b></td>
  </tr>
  <tr>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/b1c3fc41-aebe-4967-9680-4c50fdd8da87" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/e048e66d-ff9b-47d1-90dc-138570fbd8df" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/9ce6b205-7963-4a1e-90c9-c0cfa68b6b3c" />
</td>
  </tr>
  <tr>
    <td align="center">신호등 판정</td>
    <td align="center">판정 근거</td>
    <td align="center">준비 서류 체크리스트</td>
  </tr>
</table>

<table>
  <tr>
    <td colspan="3" align="center"><b>서류함 · 긴급 도움</b></td>
  </tr>
  <tr>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/74a60a6e-f054-460a-8a0b-d77cad3724b7" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/df6f96f2-408e-440b-8439-c415653fb96d" />
</td>
    <td align="center"><img width="200" alt="image" src="https://github.com/user-attachments/assets/7e1b9316-61fe-44e1-8494-31e416e29626" />
</td>
  </tr>
  <tr>
    <td align="center">서류함</td>
    <td align="center">재외공관 연락처</td>
    <td align="center">현지어 긴급 설명문</td>
  </tr>
</table>

---

## 🔹 주요 기능

### 🔐 간편하고 안전한 인증

- 카카오 OAuth2 소셜 로그인
- JWT 기반 사용자 인증 및 로그인 상태 유지
- 서비스 이용 전 온보딩과 약관 동의

### 📷 약 봉투 인식과 복약 카드

- 카메라 촬영 또는 이미지 업로드를 통한 약 봉투 스캔
- CLOVA OCR로 약품명과 복용 정보를 추출
- 식약처 의약품 API를 활용한 제품·성분 매칭 및 검증
- 인식 결과 수정, 후보 의약품 선택, 직접 입력 지원
- 복용량·복용 횟수·처방 기관·조제일을 담은 한글·영문 복약 카드 제공

### ✈️ 여행 등록과 국가별 반입 판정

- 출발지·목적지와 여행 기간 등록
- 여행에 가져갈 의약품 선택
- 성분별 반입 가능·서류 준비 필요·반입 제한 판정
- 수량 제한이 있는 성분의 소지량 계산과 한도 비교
- 정부 원천 문서, 규정 기준일 등 판정 근거 제공

### ✅ 준비 체크리스트와 서류함

- 판정 결과에 따른 준비 서류·행동 항목 자동 생성
- 항목별 완료 상태 관리 및 정부 공식 신청 페이지 연결
- 처방전·의사 소견서·반입 허가서 등 PDF 증빙 서류 업로드
- 의약품별 서류 조회, 미리보기, 다운로드 및 삭제

### 🆘 여행 중 긴급 대응

- 외교부 데이터를 활용한 현지 재외공관 연락처 조회
- 의약품 분실·부족 등 상황별 대응 안내
- 병원·약국·세관에서 제시할 수 있는 현지어 의약품 설명문 생성

---

## 🏗️ 시스템 아키텍처

```text
📱 MediPass Mobile Web (React · TypeScript)
    │  카카오 OAuth · JWT
    │  복약 카드 · 여행 체크로그 · 서류함 · 긴급 도움
    ▼
💊 MediPass Backend (Spring Boot · Java 21)
    │
    ├─▶ 🗄️ MySQL          사용자 · 의약품 · 여행 · 규제 데이터
    ├─▶ 🪣 AWS S3         증빙 서류 · Presigned URL
    │
    ├─⇄ 📷 CLOVA OCR      약 봉투 인식
    ├─⇄ 🏥 식약처 API      의약품 품목 · 성분 검증
    ├─⇄ 🏛️ 외교부 API      재외공관 연락처
    └─⇄ 🤖 OpenAI         현지어 설명문 생성
```

백엔드는 외부 API를 전용 클라이언트로 분리해 도메인 로직과 외부 명세의 결합을 낮췄습니다. 규제 판정은 미리 정규화해 적재한 데이터베이스를 기준으로 수행하며, 서류는 S3 객체 키만 저장한 뒤 요청 시 만료형 URL을 발급합니다.

### 규제 데이터 파이프라인

```text
📄 국가별 정부 원천 문서
      │  오프라인 추출 · 정규화
      ▼
📋 TSV 규제 데이터
      │  애플리케이션 시작 시 UPSERT
      ▼
🗄️ 성분 규제 · 준비 서류 템플릿
      │
      ▼
⚖️ 반입 판정 엔진 ──▶ 🚦 판정 결과 + ✅ 준비 체크리스트
```

국가별 데이터 소스와 준비 서류 템플릿을 분리해 새로운 국가의 규정을 확장할 수 있도록 설계했습니다.

---

## 🚀 기술 스택

### 📱 Frontend

<img src="https://img.shields.io/badge/TypeScript%206-3178C6?style=flat-square&logo=typescript&logoColor=white" /> <img src="https://img.shields.io/badge/React%2019-61DAFB?style=flat-square&logo=react&logoColor=black" /> <img src="https://img.shields.io/badge/Vite%208-646CFF?style=flat-square&logo=vite&logoColor=white" /> <img src="https://img.shields.io/badge/Tailwind%20CSS%204-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" />

<img src="https://img.shields.io/badge/React%20Router%207-CA4245?style=flat-square&logo=reactrouter&logoColor=white" /> <img src="https://img.shields.io/badge/TanStack%20Query%205-FF4154?style=flat-square&logo=reactquery&logoColor=white" /> <img src="https://img.shields.io/badge/Zustand%205-443E38?style=flat-square" /> <img src="https://img.shields.io/badge/Axios%201.18-5A29E4?style=flat-square&logo=axios&logoColor=white" />

<img src="https://img.shields.io/badge/Kakao%20OAuth-FFCD00?style=flat-square&logo=kakao&logoColor=black" /> <img src="https://img.shields.io/badge/ESLint%2010-4B32C3?style=flat-square&logo=eslint&logoColor=white" /> <img src="https://img.shields.io/badge/Prettier%203-F7B93E?style=flat-square&logo=prettier&logoColor=black" />

### 🌐 Backend

<img src="https://img.shields.io/badge/Java%2021-007396?style=flat-square&logo=openjdk&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Boot%204.1-6DB33F?style=flat-square&logo=springboot&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" /> <img src="https://img.shields.io/badge/Spring%20Data%20JPA-59666C?style=flat-square&logo=hibernate&logoColor=white" />

<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" /> <img src="https://img.shields.io/badge/AWS%20S3-569A31?style=flat-square&logo=amazons3&logoColor=white" /> <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" /> <img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black" />

### 🔗 External API · Infra

<img src="https://img.shields.io/badge/CLOVA%20OCR-03C75A?style=flat-square&logo=naver&logoColor=white" /> <img src="https://img.shields.io/badge/식약처%20API-0B4DA2?style=flat-square" /> <img src="https://img.shields.io/badge/외교부%20API-003478?style=flat-square" /> <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />

<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" /> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" /> <img src="https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white" />


---

## 👥 팀 구성

<table>
  <tr>
    <td align="center" width="180"><a href="https://github.com/a-neey"><img src="https://github.com/a-neey.png" width="120" height="120" alt="김예나" /><br /><b>김예나</b></a></td>
    <td align="center" width="180"><a href="https://github.com/atelier-hs"><img src="https://github.com/atelier-hs.png" width="120" height="120" alt="장현서" /><br /><b>장현서</b></a></td>
    <td align="center" width="180"><a href="https://github.com/ThreeeJ"><img src="https://github.com/ThreeeJ.png" width="120" height="120" alt="정종진" /><br /><b>정종진</b></a></td>
    <td align="center" width="180"><a href="https://github.com/yj-044"><img src="https://github.com/yj-044.png" width="120" height="120" alt="조윤지" /><br /><b>조윤지</b></a></td>
  </tr>
  <tr>
    <td align="center">Frontend</td><td align="center">Frontend</td><td align="center">Backend</td><td align="center">Backend</td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/a-neey">@a-neey</a></td><td align="center"><a href="https://github.com/atelier-hs">@atelier-hs</a></td><td align="center"><a href="https://github.com/ThreeeJ">@ThreeeJ</a></td><td align="center"><a href="https://github.com/yj-044">@yj-044</a></td>
  </tr>
</table>
