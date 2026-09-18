# AXP / AXPORT Design Specification

## 1. 브랜드

- 서비스명: AXP
- 대시보드명: AXPORT
- AI 어드바이저: 한결

### 브랜드 구조
AXP는 반도체 수출 의사결정을 지원하는 전체 서비스 브랜드다.

AXPORT는 AXP 내부에서 실제 분석 기능을 수행하는 대시보드다.

한결은 AXPORT 안에서 분석 결과를 설명하고 실무 액션을 제안하는 AI 어드바이저다.

---

## 2. 핵심 콘셉트

반도체 × 글로벌 무역 × Control Tower × Mac OS

반도체 제조사의 수출 의사결정을 지원하는 미래지향적 분석 플랫폼을 지향한다.

단순히 데이터를 보여주는 무역 대시보드가 아니라,

- 어느 국가에 수출하는 것이 적합한지
- 현재 수출구조에 어떤 리스크가 있는지
- 환율·규제·물류가 수출에 어떤 영향을 주는지
- 현재 데이터를 기반으로 어떤 대응을 해야 하는지

를 한 공간에서 확인할 수 있는 Trade Control Tower를 표현한다.

### 디자인 키워드

- Semiconductor
- Global Trade
- Export Intelligence
- Control Tower
- Data Analysis
- Mac OS
- Professional
- Future-oriented

### 디자인 방향

미래지향적이지만 게임 UI나 과도한 사이버펑크 스타일은 피한다.

실제 기업의 해외영업·수출관리·SCM·경영기획 담당자가 사용할 수 있을 정도로 전문적이고 차분한 분위기를 유지한다.

정보량은 많지만 화면은 복잡해 보이지 않도록 카드, 창, 차트 단위로 명확하게 구분한다.

---

## 3. 전체 서비스 구조

전체 서비스는 크게 두 영역으로 나눈다.

### 3-1. AXP Landing Page

서비스 소개와 첫인상을 담당하는 기업형 메인 홈페이지.

주요 역할:

- AXP 브랜드 소개
- 반도체 수출 플랫폼이라는 정체성 전달
- 핵심 기능 소개
- AXPORT 대시보드 진입 유도

### 3-2. AXPORT Dashboard

실제 분석 기능이 실행되는 업무 공간.

Mac OS를 모티프로 한 데스크톱 환경으로 구성한다.

주요 역할:

- 업체 데이터 선택 또는 업로드
- HS Code 및 국가 선택
- 수출 적합성 분석
- 수출입 분석
- 규제 분석
- 환율 분석
- 물류 분석
- 영업전략 확인
- AI 어드바이저 한결 사용
- 보고서 생성

---

## 4. 메인 사용자 흐름

AXP Landing Page

↓

AXPORT 시작하기

↓

AXPORT Mac OS Desktop

↓

회사 또는 샘플 데이터 선택

↓

HS Code / 국가 / 기간 선택

↓

수출 적합성 확인

↓

수출·규제·환율·물류 상세 분석

↓

한결에게 질문

↓

보고서 확인 또는 다운로드

---

# 5. AXP Landing Page

## 5-1. 목적

AXP가 반도체 수출 의사결정을 지원하는 글로벌 무역 플랫폼이라는 점을 기업형 메인 홈페이지 스타일로 전달한다.

첫 화면에서 사용자가 다음 세 가지를 바로 이해할 수 있어야 한다.

1. 반도체 산업을 위한 서비스
2. 글로벌 수출을 분석하는 서비스
3. 데이터를 기반으로 의사결정을 지원하는 서비스

---

## 5-2. 전체 플로우

Landing Page는 위에서 아래로 다음 순서로 구성한다.

1. Full-screen Hero
2. AXP 소개
3. 핵심 Pain Point
4. 핵심 기능
5. 작동 방식
6. AXPORT 미리보기
7. 프로젝트 소개
8. Footer

전체적인 페이지 흐름은 대기업 글로벌 비즈니스 홈페이지처럼 큰 비주얼과 넓은 여백을 사용한다.

---

# 6. Hero Section

## 6-1. 핵심 콘셉트

메인 홈페이지의 첫 화면은 컨테이너선이 바다를 항해하는 장면을 위에서 촬영한 영상이 전체 배경으로 재생된다.

이를 통해 글로벌 수출과 물류의 이미지를 직관적으로 전달한다.

영상 위에는 반도체 관련 그래픽과 데이터 시각화 요소를 결합하여 단순한 물류 사이트처럼 보이지 않도록 한다.

핵심 메시지는 다음 세 가지가 동시에 보여야 한다.

- Semiconductor
- Export
- Data Intelligence

---

## 6-2. Hero 배경

- 화면 전체를 채우는 배경 영상
- 컨테이너선이 바다 위를 항해하는 항공 촬영 영상
- 영상은 자동재생
- 음소거
- 반복재생
- 페이지 진입 즉시 재생
- 영상 위에 Navy / Black 계열의 반투명 오버레이 적용
- 텍스트 가독성을 위해 영상 자체는 약간 어둡게 처리

영상은 너무 빠르거나 역동적인 장면보다 천천히 항해하는 장면을 사용한다.

---

## 6-3. Hero 반도체 비주얼

컨테이너선 영상 위 또는 우측 영역에 반도체 관련 그래픽을 추가한다.

사용 가능한 요소:

- 반도체 Chip
- Semiconductor Board
- Wafer
- Circuit Pattern
- Data Graph
- Digital Signal
- Network Line

반도체 그래픽은 실제 제품 사진을 그대로 크게 보여주기보다는 배경 영상과 자연스럽게 섞이도록 반투명 또는 HUD 형태로 사용한다.

---

## 6-4. 글로벌 수출 효과

한국에서 세계 주요 국가로 데이터가 이동하는 느낌을 표현한다.

예:

- Korea → United States
- Korea → China
- Korea → Vietnam
- Korea → Japan
- Korea → Germany
- Korea → India

표현 방식:

- 얇은 Arc Line
- 작은 빛 입자가 이동하는 효과
- 목적지 Pulse
- 데이터 흐름처럼 보이는 Animation

Arc는 화면을 과도하게 덮지 않도록 제한적으로 사용한다.

---

## 6-5. Hero 레이아웃

전체 화면 높이는 첫 진입 화면을 거의 꽉 채운다.

### 좌측 영역

텍스트와 CTA를 배치한다.

위에서 아래 순서:

1. Category Label
2. AXP 브랜드명
3. Main Copy
4. Description
5. CTA Buttons
6. Demo Status

### 우측 영역

반도체 및 데이터 관련 시각 요소를 배치한다.

예:

- Chip
- Circuit
- Globe
- Export Arc
- HUD Data

배경 영상 자체가 강한 경우에는 우측 시각 요소를 과도하게 추가하지 않는다.

---

## 6-6. Hero 문구

### Category Label

Semiconductor Export Intelligence

### Service Name

AXP

### Main Copy

반도체 수출의 모든 신호를,  
하나의 Control Tower에서.

### Description

시장·규제·환율·물류 데이터를 연결해  
반도체 제조사의 글로벌 수출 의사결정을 지원합니다.

### English Supporting Copy

AI-driven Export Intelligence Platform

---

## 6-7. Hero CTA

Primary Button

AXPORT 시작하기

Secondary Button

기능 둘러보기

Primary Button이 가장 먼저 시선을 끌어야 한다.

---

## 6-8. Hero HUD

화면 일부에 작은 데이터 카드 형태로 배치한다.

예:

Monitored Markets  
8

HS Codes  
4

Export Signal  
+12.4%

System  
ONLINE

현재 디자인 프로토타입에서는 실제 데이터가 아닌 경우 반드시 SAMPLE 또는 DEMO임을 표시한다.

---

# 7. Navigation

상단에는 투명 또는 반투명 Navigation Bar를 사용한다.

스크롤 전:

- 투명에 가까운 형태
- 배경 영상이 자연스럽게 보이도록 구성

스크롤 후:

- Dark Navy 또는 Glass Blur Background 적용

### 왼쪽

AXP Logo

### 중앙

- 서비스 소개
- 주요 기능
- 작동 방식
- AXPORT
- 프로젝트 소개

### 오른쪽

- Language Selector
- Theme Toggle
- AXPORT 열기

---

# 8. 다국어

지원 언어:

- 한국어
- English
- 中文
- 日本語

기본 언어:

한국어

Navigation 또는 Menu Bar에서 언어를 변경한다.

표시 예:

KO

클릭 시:

- 한국어
- English
- 中文
- 日本語

사용자가 선택한 언어는 가능한 경우 세션 동안 유지한다.

---

# 9. Light / Dark Mode

## 9-1. Dark Mode

기본적으로 AXP와 가장 잘 어울리는 모드.

주요 색상:

- Deep Navy
- Charcoal
- Black
- Cyan
- Electric Blue
- Amber

특징:

- 반도체와 데이터 시각화가 잘 보임
- 글로벌 Control Tower 이미지 강화
- Glass UI 사용 가능

---

## 9-2. Light Mode

분석 가독성을 강화한 모드.

주요 색상:

- Off White
- Light Blue Gray
- Navy
- Cyan Accent

특징:

- 차트와 테이블의 가독성 우선
- 분석 대시보드에서 장시간 사용하기 편한 환경

---

# 10. Landing Page 하단 섹션

## 10-1. AXP 소개

서비스가 해결하려는 문제를 설명한다.

핵심 메시지:

반도체 제조사의 수출 의사결정에는 시장 데이터뿐 아니라 규제, 환율, 물류, 공급망 정보가 함께 필요하다.

AXP는 흩어진 데이터를 하나의 Control Tower에서 연결한다.

---

## 10-2. Pain Point

주요 Pain Point를 카드 형태로 표현한다.

예:

### 시장 데이터 분산

수출통계와 해외시장 데이터를 각각 다른 사이트에서 확인해야 한다.

### 규제 확인의 복잡성

전략물자, 수출통제, 최종사용자 검토가 수작업으로 이루어진다.

### 환율 영향 판단 어려움

환율 변화가 매출과 이익에 미치는 영향을 즉시 파악하기 어렵다.

### 물류 리스크

운송 지연 및 리드타임 변화가 여러 데이터에 흩어져 있다.

### 국가 의존도

특정 국가 또는 거래처에 대한 집중 리스크를 빠르게 확인하기 어렵다.

### 보고서 작성

분석한 내용을 다시 보고서로 정리하는 시간이 오래 걸린다.

---

# 11. 핵심 기능

기능은 카드 또는 큰 이미지 블록 형태로 구성한다.

### Export Suitability

특정 국가와 HS Code에 대한 수출 적합성을 점수로 제공한다.

### Trade Analysis

국가별 수출액, 성장률, 비중, HHI 등을 분석한다.

### Compliance

전략물자 및 수출통제 관련 검토 필요 항목을 확인한다.

### FX Simulator

환율 변화에 따른 매출과 이익 변화를 시뮬레이션한다.

### Logistics

운송기간, 지연, 항로별 물류 리스크를 분석한다.

### AI Advisor

AI 어드바이저 한결이 현재 데이터를 기반으로 실무 인사이트와 액션을 제안한다.

---

# 12. AXPORT Preview Section

Landing Page 중간 또는 후반부에서 실제 AXPORT 화면을 미리 보여준다.

Mac OS 형태의 대시보드 화면을 큰 목업 이미지처럼 배치한다.

보여줄 주요 요소:

- Top Menu Bar
- Desktop
- Finder
- Dock
- Overview Window
- Suitability Window

사용자가 AXPORT를 클릭하기 전에 실제 분석 환경이 어떻게 생겼는지 이해할 수 있어야 한다.

---

# 13. AXPORT Dashboard Concept

## 13-1. 핵심 콘셉트

AXPORT는 일반적인 웹 대시보드가 아니라 Mac OS 형태의 업무용 분석 환경을 표방한다.

사용자는 웹사이트 안에서 하나의 운영체제를 사용하는 듯한 경험을 한다.

---

## 13-2. 전체 화면 구조

AXPORT Desktop은 크게 네 영역으로 구성한다.

1. Top Menu Bar
2. Left File Area
3. Desktop Workspace
4. Bottom Dock

---

# 14. Top Menu Bar

Mac OS 상단 메뉴바를 참고한다.

### 왼쪽

- AXP Symbol
- AXPORT
- 파일
- 보기
- 분석
- 보고서
- 도움말

### 오른쪽

- Language
- Light / Dark Mode
- Data Status
- Exchange Rate
- Time

전체적으로 얇고 반투명한 Glass UI를 적용한다.

---

# 15. Desktop

중앙 영역은 실제 Mac Desktop처럼 보이도록 한다.

배경은 AXP Landing Page와 연결되는 톤을 유지한다.

가능한 배경 요소:

- Dark Navy Gradient
- Semiconductor Circuit
- Faint Globe
- Minimal Grid

화면이 너무 화려하지 않도록 한다.

---

# 16. Left File Area

화면 왼쪽에는 Finder Sidebar와 Desktop File의 중간 형태로 데이터 접근 영역을 둔다.

예:

### Favorites

- Companies
- Sample Data
- Uploads
- Reports

### Sample Files

- C001
- C002
- C003
- C004
- C005

각 데이터는 Excel 또는 File Icon 형태로 표현한다.

더블클릭 시 미리보기 또는 데이터 선택 창이 열린다.

---

# 17. Dock

화면 하단에는 Mac OS 스타일 Dock을 배치한다.

추천 기능:

1. Finder
2. Overview
3. Trade
4. Suitability
5. Compliance
6. FX
7. Logistics
8. Strategy
9. 한결
10. Reports

Dock 기능:

- Hover 시 아이콘 확대
- 클릭 시 해당 Window Open
- 실행 중인 앱에는 작은 Indicator 표시
- 최소화된 Window는 Dock에서 복구 가능

---

# 18. Window System

각 기능은 독립적인 Window 형태로 실행한다.

Window 상단 왼쪽에는 세 개의 Control Button을 둔다.

- Close
- Minimize
- Maximize

기본 동작:

- Window Drag
- Resize
- Focus
- Minimize
- Maximize
- Close
- Multiple Window

포커스된 Window가 가장 앞으로 올라온다.

---

# 19. Overview Window

## 목적

현재 선택된 업체, 국가, HS Code의 핵심 상태를 한눈에 확인한다.

### 상단 Filter

- Company
- HS Code
- Country
- Period

### KPI Card

- Export Amount
- YoY
- Country Dependency
- Export Suitability
- Regulation Status
- Logistics Status

### Main Chart

- Export Trend
- Country Composition
- Market Comparison

### Risk Summary

- Regulation
- FX
- Logistics
- Concentration

전체적인 카드 구조는 금융 또는 BI Dashboard처럼 깔끔하게 구성한다.

---

# 20. Export Suitability Window

AXPORT에서 가장 중요한 핵심 화면.

## 목적

선택한 회사, HS Code, 국가에 대한 수출 적합성을 직관적으로 보여준다.

### 상단

Company  
HS Code  
Country  
Period

### Main Score

가장 크게 표시한다.

예:

Export Suitability

82 / 100

Grade A

### Component Score

- Market
- Dependency
- Regulation
- FX
- Logistics

### Evidence

점수 아래에는 계산 근거를 보여준다.

예:

Market YoY  
+14.2%

Country Dependency  
24.1%

Average Transit Time  
9.3 days

Compliance  
Low Risk

### Input Coverage

현재 점수가 어떤 데이터를 기반으로 계산되었는지 표시한다.

예:

Input Coverage  
85%

### Button

근거 자세히 보기

---

# 21. Trade Window

## 목적

회사의 글로벌 수출 구조를 확인한다.

표시 요소:

- 국가별 수출액
- 국가별 비중
- YoY
- MoM
- HHI
- 무역수지
- 24개월 추이

차트:

- Bar Chart
- Line Chart
- Donut Chart
- Treemap
- Data Table

---

# 22. Compliance Window

## 목적

전략물자 및 규제 관련 검토 필요성을 보여준다.

### Status

- 판정 필요
- 주의
- 해당 가능성 낮음
- 미평가

### Content

- HS Code
- Product
- End User
- Destination
- Keyword Match
- Restricted Party Candidate

### Checklist

- EUC 확인
- 전문판정 확인
- 재수출 경로 확인

법적 최종 판단이 아니라 참고용 1차 검토임을 항상 표시한다.

---

# 23. FX Window

## 목적

환율 변화가 매출과 이익에 미치는 영향을 시뮬레이션한다.

### 상단

- Base FX
- Current FX

### Simulator

Slider

-20% ~ +20%

### Results

- Revenue
- Profit
- Margin
- Break-even FX

### Chart

환율 변화와 손익 변화의 관계를 Line Chart로 보여준다.

---

# 24. Logistics Window

## 목적

물류 리스크와 운송 지연을 확인한다.

표시 항목:

- Average Transit Time
- Median Transit Time
- Air / Sea
- Route Delay
- Delayed Shipment
- B/L Search

가능한 경우 Route Map 또는 Transport Flow를 시각적으로 표현한다.

---

# 25. Strategy Window

## 목적

분석 결과를 실제 업무 액션으로 연결한다.

국가별 전략 분류:

- 확대
- 방어
- 신규 개척
- 추천 보류

각 전략 카드에는 반드시 근거 수치를 함께 표시한다.

예:

USA

확대

Suitability  
82

Market YoY  
+14.2%

Country Share  
12%

### Department Action

- Sales
- Export Management
- SCM

---

# 26. AI Advisor 한결 Window

## 목적

현재 분석 데이터를 기반으로 사용자에게 실무 인사이트와 대응 액션을 제공한다.

### Header

한결

Trade Control Tower AI Advisor

### Chat Layout

- Assistant Message
- User Message
- Input Area

### 현재 분석 Context

- Company
- HS Code
- Country
- Period

### 한결의 기본 응답 구조

1. 현황 요약
2. 리스크 / 기회
3. 권장 액션
4. 다음 확인 질문

한결은 별도의 AI Application처럼 Dock에서 실행한다.

---

# 27. Reports Window

## 목적

현재 분석 결과를 보고서 형태로 출력한다.

### Report Types

- Summary PDF
- Full PDF
- Company Comparison PDF
- Excel

### 화면 구성

- Report Preview
- 최근 생성 보고서
- Download Button

---

# 28. Design System

## Typography

기본 서체:

Pretendard

보조:

Inter 또는 system-ui

숫자:

font-variant-numeric: tabular-nums

데이터 테이블 숫자는 우측 정렬한다.

---

## Color Direction

색상은 CSS Variable로 관리한다.

### Dark

Background  
Deep Navy / Charcoal

Surface  
Dark Blue Gray

Primary Accent  
Cyan

Secondary Accent  
Electric Blue

Warning  
Amber

Danger  
Muted Red

Text  
White / Cool Gray

### Light

Background  
Off White

Surface  
White

Secondary Surface  
Light Blue Gray

Primary Text  
Navy

Secondary Text  
Gray

Accent  
Cyan / Blue

---

# 29. UI Style

공통 UI 스타일:

- Rounded Card
- Glass Panel
- Thin Border
- Soft Shadow
- Large Spacing
- Clear Hierarchy

Window Radius:

약 12~16px

Card Radius:

약 12~20px

버튼은 지나치게 둥근 Pill 형태보다는 전문적인 Rounded Rectangle 형태를 기본으로 한다.

---

# 30. Animation

Animation은 보조 역할로만 사용한다.

허용:

- Container Ship Background Video
- Export Arc Movement
- Globe Rotation
- Dock Hover Magnification
- Window Open / Close
- Soft Fade
- Chart Transition
- Pulse Indicator

피해야 할 것:

- 과도한 Neon Flash
- 빠른 Background Movement
- 게임 UI처럼 보이는 효과
- 불필요한 Particle 남용

---

# 31. Responsive

Desktop을 우선 설계한다.

AXPORT는 데스크톱 업무 환경이 핵심이므로 1440px 기준을 우선 고려한다.

1024px 이하:

- Window를 전체화면 Card 형태로 변경
- Dock을 Bottom Navigation 형태로 변경
- Left File Area 축소 가능

Mobile에서는 핵심 기능 확인 위주로 단순화한다.

---

# 32. 디자인 프로토타입 범위

현재 디자인 단계에서는 모든 기능을 완성하지 않는다.

우선 다음 화면을 실제 코드로 구현한다.

1. AXP Landing Page
2. AXPORT Desktop
3. Overview Window
4. Export Suitability Window
5. 한결 Window
6. Language UI
7. Light / Dark Toggle
8. Dock
9. Basic Window Interaction

나머지 기능:

- Compliance
- FX
- Logistics
- Strategy
- Reports

초기 시안에서는 Dock Icon과 기본 Window Frame까지만 구현해도 된다.

---

# 33. 디자인 우선순위

1. Export Suitability
2. Overview
3. Trade Analysis
4. Risk
5. Strategy
6. AI Advisor

가장 중요한 정보가 항상 먼저 보이도록 구성한다.

---

# 34. 디자인 원칙

1. 정보보다 장식이 앞서지 않는다.
2. 모든 숫자는 단위와 의미가 명확해야 한다.
3. 카드 수를 과도하게 늘리지 않는다.
4. 주요 지표는 한눈에 비교할 수 있어야 한다.
5. 경고 색상은 실제 Risk 또는 Warning에만 사용한다.
6. 실제 데이터가 아닌 값은 SAMPLE 또는 DEMO로 표시한다.
7. 반도체·수출·데이터 분석이라는 서비스 정체성이 첫 화면부터 유지되어야 한다.
8. Landing Page와 AXPORT는 스타일이 다르더라도 하나의 브랜드처럼 연결되어야 한다.
9. AXPORT의 Mac OS 메타포가 실제 분석 기능보다 앞서지 않도록 한다.
10. 사용자가 3초 안에 현재 화면의 핵심 메시지를 이해할 수 있어야 한다.