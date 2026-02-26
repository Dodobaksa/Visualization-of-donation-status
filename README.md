# Visualization-of-donation-status

🧩 **기빙코리아 2026 개인기부자 설문 데이터 분석 프로젝트**  
작업기간: *2026.02.07 ~ 2026.02.25*  
작업자: **dodobaksa**

데이터 출처:  
🔗 https://research.beautifulfund.org/22799/

---

## 🔗 전체 시각화 페이지 바로가기

<p align="left">
  <a href="https://www.notion.so/2026-312a4a076c608032a3bac127701c972a" target="_blank">
    <img src="https://img.shields.io/badge/📊_Notion_Visualization_Page-000000?style=for-the-badge&logo=notion&logoColor=white" />
  </a>
</p>

---

## 📘 프로젝트 소개
기빙코리아 2026 개인기부자 설문 데이터를 기반으로 기부 행동·동기·패턴을 시각화한 프로젝트입니다.  
데이터 전처리, 통계 분석, 인사이트 도출, EDA 및 시각화를 포함합니다.


---

## 0. 프로젝트 소개(Introduction)

이 프로젝트는 *기빙코리아 2024 개인기부자 조사* 데이터를 기반으로  
한국 성인(만 19세 이상)의 **기부 행태, 기부 의향, 사회적 인식, 지역·연령·소득별 기부 패턴**을 분석하는 것을 목표로 합니다.

특히 다음을 중점적으로 다룹니다.

- 국내 기부자 현황과 구조 파악  
- 기부 의향에 영향을 미치는 주요 요인 도출  
- 지역·연령·소득별 기부 특성 비교  
- 페르소나 기반 타겟팅 전략 제안  
- 비기부자 → 기부자 전환 요인 분석  

분석은 **Python 기반 Jupyter Notebook(.ipynb)** 형태로 수행되었습니다.

---
## 1. 요약 (Summary)

### 1) 전체 기부 구조
- 일시기부자(1,143명)가 가장 많아 **정기기부 전환 잠재력 큼**
- 정기기부자는 351명으로 소수
- 기부중단자 > 비기부자 순

### 2) 연령대·세대 특성
- 고연령층은 정기·일시 기부 비중 높음
- 20~30대: SNS·유튜브 선호  
- 60대+: TV·라디오 선호

### 3) 소득수준과 기부
- 정기기부자 소득 가장 높음  
- 소득 감소 시 기부 중단 가능성↑  
- 고소득층: 의료·문화예술 기부 선호

### 4) 지역별 특징
- 정기기부율 최고: 강원 / 최저: 전남  
- 일시기부율 최고: 서울 / 최저: 울산  
- 기부 취약 지역: 세종, 제주, 전남, 광주

### 5) 기부의향 결정 요인
- 가장 강한 요인: 나이, 소득, 가구원 수  
- 긍정 요인: 작년 기부액, 정기기부 횟수, 비영리에 대한 긍정 인식  
- 부정 요인: 소득감소, 미래전망 비관, 종교기부 경험

### 6) 페르소나(4개)
- 사회구호형  
- 문화고액형  
- 기부소극층  
- 무관심층  

### 7) 우선 타겟팅 집단
1. **세종 30대 무관심층**  
2. **제주 60대 이상 무관심층**  
3. **광주 60대 이상 무관심층**

### 8) 채널 접근 전략
- 대부분 지역: TV·라디오  
- 세종/대구/충북: 포털 기부 플랫폼  
- 20~30대: SNS·유튜브

### 9) 기부 전환 요인
- 촉진: 나이↑, 소득↑, 비영리 긍정 인식  
- 저해: 소득 감소, 미래 비관, 종교적 기부경험

---
## 2. 데이터 설명(Data Description)

기빙코리아 2024 – 개인기부자 조사(일반국민 대상) 원자료 기반이며 주요 항목은 다음과 같습니다.

### ◎ 조사 개요
- **대상:** 만 19세 이상 전국 성인 2,500명  
- **방법:** 웹조사(컴퓨터)  
- **년도:** 2024

### ◎ 주요 수집 변수
- 기부 경험 및 형태(정기/일시)
- 기부 분야 및 기부 금액
- 기부 정보 접근 방식(SNS, TV, 유튜브 등)
- 기부 의향 및 결정 요인
- 비기부 사유, 기부 중단 사유
- 자원봉사 경험
- 비영리조직 인식(신뢰도, 투명성 등)
- 고향사랑기부제·종교 기부
- 인구통계(성별, 나이, 소득, 지역 등)

## @ 설문지 구조

아래 표는 *기빙코리아 2024 개인기부자 조사*의 전체 설문 문항을 구조화해 정리한 것입니다.

---

### 1. 조사 개요(Survey Overview)

| 항목 | 내용 |
|------|------|
| **조사 대상 (Target)** | 일반국민(만 19세 이상 전국 성인 남녀) / General Public (Adults aged 19+) |
| **표본 수 (Sample Size)** | 2,500 |
| **조사 방법 (Survey Method)** | 웹조사(컴퓨터) / Online (Computer) |

---

### 2. 기부 실태(Status Quo of Donation)

| 주요 항목 | 세부 내용 |
|-----------|-----------|
| **기부 경험** | Experience of Donation |
| **기부 정보 접근 방식** | Ways of Accessing Donation-related Information |
| **기부 분야 및 금액** | Area & Amount of Donation |
| **기부한 단체 수** | Number of Organizations Donated to |
| **참여한 이슈** | Issues Participated in Donation |
| **기부 이유** | Reasons for Donation |
| **기부처 결정 고려사항** | Considerations When Choosing Recipients |
| **정기 기부 여부·횟수** | Regular Donation Status & Frequency |
| **일시 기부 여부·횟수** | One-time Donation Status & Frequency |
| **2023년 기부 활동** | Donation Activities Participated in 2023 |
| **현재 기부 중 최고 금액 단체** | Current Organization with Highest Donation Amount |
| **이전 기부 중 최고 금액 단체** | Previous Organization with Highest Donation Amount |
| **2024년 기부 의향** | Intention to Donate in 2024 |
| **비기부 사유(비기부자)** | Reasons for Not Donating (Non-Donors) |
| **2023년 이전 기부 경험(비기부자)** | Pre-2023 Donation Experience (Non-Donors) |
| **기부 중단 이유** | Reasons for Discontinuing Donations |

---

### 3. 자원봉사(Volunteer)

| 주요 항목 | 세부 내용 |
|-----------|-----------|
| **자원봉사 여부** | Volunteer Experience |
| **자원봉사 시간** | Volunteer Hours |

---

### 4. 비영리조직 인식(Perception of Non-Profit Organizations)

| 주요 항목 | 세부 내용 |
|-----------|-----------|
| **알고 있는 기부 단체** | Known Donation Organizations |
| **비영리조직 역할·신뢰·투명성 인식** | Perception of Role, Trustworthiness & Transparency |
| **기부환경 인식** | Perception of Donation Environment |
| **비영리 운영 인식** | Perception of Non-Profit Operations |

---

### 5. 기부로 인한 변화(Impact of Donation)

| 주요 항목 | 세부 내용 |
|-----------|-----------|
| **기부 만족도** | Donation Satisfaction |
| **기부단체와의 관계성** | Relationship with Donation Organizations |
| **기부단체 충성도** | Loyalty to Donation Organizations |
| **기부로 인한 사회변화 인식** | Perception of Social Change Through Donation |
| **기부자 노력** | Donor Efforts |

---

### 6. 고향사랑기부제 & 종교 기부(Hometown Love Donation & Religious Giving)

| 주요 항목 | 세부 내용 |
|-----------|-----------|
| **고향사랑 기부제 인지** | Awareness of Hometown Love Donation |
| **고향사랑 기부 경험** | Experience with Hometown Love Donation |
| **기존 기부에 미친 영향** | Impact on Existing Donations |
| **종교단체 헌금·보시 경험** | Experience with Religious Donations |
| **종교단체 헌금·보시 금액** | Amount of Religious Donations |

---

### 7. 인구학적 특성(Demographics)

| 주요 항목 | 세부 내용 |
|-----------|-----------|
| **성별** | Gender |
| **연령** | Age |
| **지역** | Region |
| **학력** | Education Level |
| **가구원 수** | Household Size |
| **혼인 상태** | Marital Status |
| **자녀 유무** | Presence of Child(ren) |
| **종교** | Religion |
| **고용 상태** | Employment Status |
| **월평균 가구소득** | Average Monthly Household Income |
| **연평균 소득 변화** | Yearly Average Income Change (Last Year) |

## 📦 Requirements

아래 명령어로 필요한 패키지를 설치할 수 있습니다:

```bash
pip install -r requirements.txt

---
---
