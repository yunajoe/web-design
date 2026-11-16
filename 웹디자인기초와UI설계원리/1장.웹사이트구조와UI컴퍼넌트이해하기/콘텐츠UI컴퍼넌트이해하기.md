# **카드부터 캐러셀까지, 콘텐츠 UI 컴포넌트 이해하기**

## **1. 콘텐츠에 맞는 컴포넌트 선택하기**

콘텐츠 UI는 **사용자가 정보를 어떤 방식으로 탐색하는지**에 따라 선택해야 해.

| 사용자의 탐색 방식          | 적합한 컴포넌트 |
| --------------------------- | --------------- |
| 콘텐츠를 하나씩 살펴보기    | 카드            |
| 여러 항목을 빠르게 훑어보기 | 리스트          |
| 여러 데이터 비교하기        | 테이블          |
| 긴 설명 접고 펼치기         | 아코디언        |
| 여러 콘텐츠를 좌우로 넘기기 | 캐러셀          |
| 이미지나 영상을 크게 보기   | 라이트박스      |

## **2. 주요 콘텐츠 UI 컴포넌트**

### **① 카드(Card)**

[Building a Modern E-commerce App with Next.js 15, Zustand, and TypeScript - DEV Community](https://images.openai.com/static-rsc-4/ulwl5pk4XCTij8a92L2OrmSXcwAHeJ8sMtrYXvm1JRc1XadqX89kDkiIxdv9i9IMhk5Dcr7PZgJ27IjT3GzLizPZzS7SWRcB7da2-EF0KLrUU022VvhlggjQXkK7rDVCOSuCEEXasWh2AY68SVh_0oiOopR-RXh7PP7ysMYpX-4?purpose=inline)

[dev.to](https://dev.to/blamsa0mine/building-a-modern-e-commerce-app-with-nextjs-15-zustand-and-typescript-18i5?utm_source=chatgpt.com)

이미지, 제목, 설명, 가격, 상태 등 관련 정보를 하나의 독립된 단위로 묶어 보여주는 컴포넌트.

**사용 상황**

- 상품 목록
- 블로그 글
- 포트폴리오
- 강의 목록

**설계 시 주의사항**

- 이미지와 제목 등 핵심 정보의 우선순위 설정
- 제목 최대 줄 수 지정
- 이미지 비율 통일
- 콘텐츠 길이가 달라져도 레이아웃 유지

### **② 리스트(List)**

[Dashboard Notification UI Design 🔔 :: Behance](https://images.openai.com/static-rsc-4/OmXkYT2oPFGW3Ylzf4d6CcOOP_7T9gXgY3hUaM_aTUkTKT77I5u0ptl-KqaX7STtTvMUWpMxwYgDfkJlljLPF6D0vaEhBN_2YB9QV-ipOWcCHk9TJQUTuNFSMnTnpIYcMISeX6E4X4EMjIsORZrZ40G-kUc_AhPF4VERV3_Maqo?purpose=inline)

[behance.net](https://www.behance.net/gallery/239530051/Dashboard-Notification-UI-Design-?utm_source=chatgpt.com)

여러 항목을 세로로 배치해 빠르게 훑어볼 수 있도록 만드는 방식.

**사용 상황**

- 알림
- 메시지
- 검색 결과
- 파일 목록
- 설정 메뉴

**설계 시 주의사항**

- 한 화면에 많은 정보를 보여줄 수 있도록 구성
- 텍스트와 상태 정보 중심으로 배치
- 편집·삭제·공유 등 자주 사용하는 행동만 노출
- 나머지 행동은 더보기 메뉴에 정리

### **③ 카드 vs 리스트**

| 구분      | 카드                     | 리스트                  |
| --------- | ------------------------ | ----------------------- |
| 목적      | 콘텐츠를 하나씩 살펴보기 | 여러 항목 빠르게 훑기   |
| 중심 정보 | 이미지와 핵심 콘텐츠     | 텍스트와 상태 정보      |
| 정보 밀도 | 낮음                     | 높음                    |
| 예시      | 상품, 블로그, 포트폴리오 | 알림, 메시지, 검색 결과 |

같은 콘텐츠라도 서비스의 목적에 따라 표현 방식이 달라질 수 있어.

### **④ 테이블(Table)**

데이터를 행(Row)과 열(Column)로 나눠 여러 항목의 값을 비교하는 컴포넌트.

**사용 상황**

- 회원 목록
- 주문 내역
- 통계
- 재고 관리
- 가격 비교

**설계 시 주의사항**

- 텍스트는 왼쪽 정렬
- 금액이나 수량처럼 자릿수를 비교하는 숫자는 오른쪽 정렬
- 모바일에서는 중요도가 낮은 열을 숨기거나 가로 스크롤 적용
- 필요에 따라 카드 형태로 전환

### **⑤ 아코디언(Accordion)**

[37 Best Bootstrap Accordion Examples 2025 - uiCookies](https://images.openai.com/static-rsc-4/f76S4dLorne4LGStlA_1I-YluApXtnLW6FRc_kAQlutqyG-Ryaz7JRgQwy2ddm4FVh_tmR0ESS7BOML8NSerII8hgzFsr16GpBwSl7ev7_lPMkmSgLtmjfolFrwAkVnCql_6UBSZ0uxgiWd6iPPjP1eqN__UrAWqSOZzlDCbsx4?purpose=inline)

[uicookies.com](https://uicookies.com/bootstrap-accordion/?utm_source=chatgpt.com)

내용을 접어두고 사용자가 원하는 항목만 펼쳐볼 수 있도록 만드는 컴포넌트.

**사용 상황**

- FAQ
- 추가 설명
- 상세 옵션
- 긴 부가 정보

**설계 시 주의사항**

- 핵심 정보는 바로 보여주기
- 가격이나 중요한 제한 사항을 아코디언 안에 숨기지 않기
- 추가 설명 위주로 접어두기

### **⑥ 캐러셀(Carousel)**

[12 Amazing Slider Website Designs \[Examples & When to use\] - Alvaro Trigo's Blog](https://images.openai.com/static-rsc-4/mhMFtxMlrhAp7-6AOX41ixaW53DOGdoc3Apn6ONYC2UY2qUGjcAdFV-BnlVkQH0JGPvJIiwOhKWCsD1vm-sJFDrLa3qShs34vxB3FD3axVdRfxmsSNCutZ0dj8CtaoUC-rOmoZmlGBitMWE6Yvayqr0W1Kcl3NF0HCnIBf3N8uk?purpose=inline)

[alvarotrigo.com](https://alvarotrigo.com/blog/slider-website-design-examples/?utm_source=chatgpt.com)

여러 콘텐츠를 좌우로 넘겨 보여주는 컴포넌트.

**사용 상황**

- 메인 배너
- 추천 상품
- 고객 후기
- 이미지 갤러리

**설계 시 주의사항**

- 중요한 콘텐츠를 첫 번째에 배치
- 현재 위치를 알려주는 인디케이터 제공
- 이전·다음 버튼 제공
- 자동 재생 시 충분한 표시 시간 제공
- 사용자가 직접 멈추거나 이동할 수 있도록 구성

주의

&#x20;사용자가 다음 슬라이드로 넘기지 않으면 뒤에 있는 콘텐츠를 보지 못할 수 있어.

### **⑦ 라이트박스(Lightbox)**

[Angular 2+ Lightbox & Gallery Component - ngbox | Angular Script](https://images.openai.com/static-rsc-4/STLbxsZopFzvghWf9a_jv2nm0aGDQ7E7PCUZT48myPz7cURmewHa8ABs2sMnjtUpEGMhaMdA5AHy1WovBvgB01husEEYKJRyjH3lYbTs_9g0pt81UUYYgEbtqJMHJFHB-c-15JKJVrca6uuwq-QI7m8t783dV0Q_6yYr35v0t_4?purpose=inline)

[angularscript.com](https://angularscript.com/angular-2-lightbox-gallery-component-ngbox/?utm_source=chatgpt.com)

이미지나 영상을 선택했을 때 현재 페이지 위에서 크게 보여주는 방식.

**사용 상황**

- 포트폴리오 이미지
- 상품 상세 이미지
- 사진 갤러리

**설계 시 주의사항**

- 배경을 어둡게 처리해 콘텐츠에 집중
- 여러 이미지가 있다면 이전·다음 버튼이나 스와이프 제공
- 닫기 버튼과 ESC 키 지원
- 원래 화면으로 쉽게 돌아갈 수 있도록 구성

## **3. 모달 vs 라이트박스**

둘 다 현재 페이지 위에 표시되는 형태지만 목적이 달라.

| 구분        | 모달(Modal)                | 라이트박스(Lightbox)       |
| ----------- | -------------------------- | -------------------------- |
| 목적        | 특정 작업에 집중           | 시각 콘텐츠 감상           |
| 주요 콘텐츠 | 폼, 안내, 확인             | 이미지, 영상               |
| 예시        | 삭제 확인, 회원가입        | 사진 확대, 상품 이미지     |
| 공통점      | 배경을 덮고 별도 영역 표시 | 배경을 덮고 별도 영역 표시 |

## **4. 콘텐츠 UI 선택 기준**

| 상황                          | 추천 컴포넌트 |
| ----------------------------- | ------------- |
| 상품 이미지와 가격을 보여주기 | 카드          |
| 알림 목록을 빠르게 확인하기   | 리스트        |
| 회원별 정보와 상태 비교하기   | 테이블        |
| FAQ 답변을 접어두기           | 아코디언      |
| 추천 상품을 좌우로 탐색하기   | 캐러셀        |
| 상품 이미지를 크게 보기       | 라이트박스    |

## **5. 빠르게 확인하기**

콘텐츠 UI를 설계할 때 아래 항목을 확인하면 좋아.

- 하나씩 살펴볼 콘텐츠라면 카드가 적합한가?
- 빠르게 훑어야 한다면 리스트가 더 적합하지 않은가?
- 여러 값을 비교해야 한다면 테이블을 사용했는가?
- 중요한 정보를 아코디언 안에 숨기지 않았는가?
- 캐러셀의 중요한 콘텐츠가 뒤쪽에만 배치되어 있지 않은가?
- 라이트박스를 쉽게 닫고 이전 화면으로 돌아갈 수 있는가?
- 모바일에서도 편리하게 사용할 수 있는가?

## **핵심 요약**

1. **카드**: 콘텐츠를 하나씩 살펴볼 때
2. **리스트**: 여러 항목을 빠르게 훑을 때
3. **테이블**: 여러 데이터의 값을 비교할 때
4. **아코디언**: 긴 부가 설명을 접어둘 때
5. **캐러셀**: 제한된 공간에서 여러 콘텐츠를 넘겨볼 때
6. **라이트박스**: 이미지와 영상을 크게 감상할 때

**가장 중요한 기준은 컴포넌트의 모양이 아니라 사용자가 콘텐츠를 어떻게 탐색해야 가장 편한가야.**

출처: [디자인베이스 – 카드부터 캐러셀까지, 콘텐츠 UI 컴포넌트 이해하기](https://designbase.co.kr/course/web-design-ui-foundations/lesson/content-ui-components-2/?utm_source=chatgpt.com)
