# **3강. 웹 디자이너가 알아야 할 필수 개념: 반응형 vs 적응형, 모바일 퍼스트 이해하기**

디자인베이스 · 웹 디자인 기초와 UI 설계 원리

## **1. 핵심 개념**

웹디자인은 데스크톱 화면만 고려하는 것이 아니라 **스마트폰, 태블릿 등 다양한 화면 크기에서도 콘텐츠와 기능을 편리하게 사용할 수 있도록 설계하는 것**이 중요하다.

대표적인 개념은 다음 4가지다.

- 반응형 웹 (Responsive Web)
- 적응형 웹 (Adaptive Web)
- 데스크톱 퍼스트 (Desktop First)
- 모바일 퍼스트 (Mobile First)

## **2. 반응형 웹 (Responsive Web)**

**하나의 웹사이트 구조를 기반으로 화면 너비에 따라 레이아웃이 유연하게 변경되는 방식이다.**

[User Experience (UI/UX) + Responsive Web Design (RWD)](https://images.openai.com/static-rsc-4/k_w7xgGErYZKvRcDDI7Shgt5zeUqbE0MCuNbWD_DLk3gRDhJV08h5MnTC-anozSjD2YLHIHqH72V6FEROyke-5zZ5fPqXblWKo92O_UPqxw7KK-KFpt2IAYXQKVAuk-QMDWFgTXZp5tC5SqxSfmHv-bUFsYawkqYftFs_p7Pw9o?purpose=inline)

[frontlinedev.com](https://www.frontlinedev.com/user-experience-ui-ux-responsive-web-design-rwd?utm_source=chatgpt.com)

화면 크기에 따른 변화 예시

| 기기     | 카드 배치 |
| -------- | --------- |
| 데스크톱 | 4열       |
| 태블릿   | 2열       |
| 모바일   | 1열       |

**주요 특징**

- 하나의 웹사이트 구조로 여러 화면에 대응한다.
- 화면 너비에 따라 콘텐츠 크기와 배치가 변경된다.
- 일반적으로 동일한 URL을 사용한다.
- 별도의 모바일 사이트를 관리할 필요가 적다.

**화면이 좁아질 때 변경되는 요소**

- 여러 열의 콘텐츠가 한두 열로 변경
- 좌우 배치가 위아래 배치로 변경
- 검색창이 검색 아이콘으로 변경
- 내비게이션이 메뉴 버튼 안으로 이동
- 콘텐츠 여백과 글자 크기 조정

### **브레이크포인트 (Breakpoint)**

**화면 너비에 따라 레이아웃이 변경되는 기준점이다.**

[How to Optimize UI for Mobile, Tablet, and Desktop | Adalo](https://images.openai.com/static-rsc-4/Pc0BVo8qdv7hFZywbDsoGNu9LMJimeRTHxm4nzjw1w3nCc4DtMIHTr0XtIBjtK7YAb7ULN7-2XHvYm7HKkNQ993SYgsnw5kKIL8XF3RTVp0CJbbxDl0CkrpUZ3I_uUEqrntkz7_jQ8Aadj3AwMF9xXpNQkn4f_pJBXV8UVVd6Wk?purpose=inline)

[adalo.com](https://www.adalo.com/posts/optimize-ui-mobile-tablet-desktop/?utm_source=chatgpt.com)

예시:

- 넓은 화면: 카드 4열
- 특정 너비 이하: 카드 3열
- 태블릿 구간: 카드 2열
- 모바일 구간: 카드 1열

**중요한 점**

- 단순히 PC, 태블릿, 모바일이라는 기기 이름으로 결정하지 않는다.
- 콘텐츠와 레이아웃이 자연스럽게 유지되기 어려운 지점을 기준으로 설정한다.
- 열 개수뿐 아니라 여백, 글자 크기, 내비게이션 등도 변경할 수 있다.

## **3. 적응형 웹 (Adaptive Web)**

**기기나 화면 크기별로 미리 준비된 서로 다른 화면을 제공하는 방식이다.**

[Web Design Mistakes to Avoid in Malaysia | XBTECH Studio | XBTECH Studio](https://images.openai.com/static-rsc-4/pmNk1YcLiYD1rLg_HqSjFbk_j-jHEc4F_oPeojvjbJz6FTFjYqkYb40y_jlDvlbTkfareVTBfPitRjSmh_JN4NyMxIHh1FCvH0sgXXd4yvBAXk5WbUViX4zd0f3lLgixT0lsHFlJd-sMt-4IJseXrZNk_mc0M-O2zPyWUeaZXe4?purpose=inline)

[xbtechstudio.com](https://xbtechstudio.com/blog/web-design-mistakes-malaysia?utm_source=chatgpt.com)

예시:

- 데스크톱: 다양한 뉴스, 콘텐츠, 광고, 바로가기 기능 제공
- 모바일: 자주 사용하는 기능 중심으로 화면 구성

**주요 특징**

- 화면별 레이아웃을 별도로 준비한다.
- 기기 환경에 맞는 화면 버전을 제공한다.
- 화면별 디자인 차이가 클 수 있다.
- 모바일 전용 주소를 사용할 수도 있다.

모바일 전용 주소 예시:

```
www.example.com
m.example.com
www.example.com/m
```

단, 모든 적응형 웹이 별도의 모바일 주소를 사용하는 것은 아니다.

## **4. 반응형 웹 vs 적응형 웹**

| 구분      | 반응형 웹                   | 적응형 웹                |
| --------- | --------------------------- | ------------------------ |
| 기본 방식 | 하나의 구조가 유연하게 변경 | 미리 준비된 화면 제공    |
| 레이아웃  | 화면 크기에 따라 조정       | 화면별 레이아웃 선택     |
| 웹 주소   | 일반적으로 동일             | 별도 주소 사용 가능      |
| 디자인    | 여러 화면에서 일관성 유지   | 화면별 차이가 클 수 있음 |
| 유지보수  | 하나의 구조 중심            | 여러 버전 관리 가능      |
| 특징      | 다양한 화면에 유연하게 대응 | 특정 환경에 맞춰 최적화  |

**어떤 방식이 더 좋을까?**

- 일반적인 웹사이트: 반응형 방식이 효율적일 수 있다.
- 기기별 사용 목적과 기능이 크게 다른 서비스: 적응형 방식이 적합할 수 있다.
- 두 방식을 하나의 서비스에서 함께 사용할 수도 있다.

## **5. 데스크톱 퍼스트 (Desktop First)**

**넓은 데스크톱 화면을 먼저 설계한 다음, 작은 화면에 맞춰 축소하고 재배치하는 방식이다.**

[Mobile First vs Desktop First: Which Is Better for Web Development](https://images.openai.com/static-rsc-4/YFlX1LmydxX4aR-MK29_fQk6YniiKFsDv6eOZbL6doTm-y7tFep3swy935uslmzqhzqLUHA4sQa0s4OPuyrgHuvsw45d0sEiYNe0T8WQgNd4K2gIfXq7iT-FMuYEORSEHhvKqO2ifKKBgKb9IkaWoHjGp4K4BDeuuJMLT0dIlks?purpose=inline)

[softermii.com](https://www.softermii.com/blog/web-development-mobile-first-or-desktop-first?utm_source=chatgpt.com)

설계 순서:

## **데스크톱 → 노트북 → 태블릿 → 모바일**

**장점**

- 많은 정보와 기능을 한 화면에 구성하기 쉽다.
- 복잡한 레이아웃과 여러 열의 콘텐츠 설계에 유리하다.
- 데스크톱 사용 비중이 높은 서비스에 적합할 수 있다.

**주의점**

- 모바일 화면이 지나치게 복잡해질 수 있다.
- 어떤 요소를 유지하고 숨길지 결정해야 한다.
- 단순히 화면을 축소하면 사용성이 떨어질 수 있다.

## **6. 모바일 퍼스트 (Mobile First)**

**모바일 화면을 먼저 설계한 다음, 태블릿과 데스크톱처럼 큰 화면으로 확장하는 방식이다.**

[Responsive Web Design Malaysia: A Complete Guide | XBTECH Studio | XBTECH Studio](https://images.openai.com/static-rsc-4/Cw7_Sv5vYkE_uKkzyFBXUF0OxV8hNei3YruZHJJEfbMe6NQlVHyLVJc7Ts5yTi3Vjc-Jg0dyz6fewVxL4XVN5zioqkstp_LlX2SeK4w2I0oxcyg9wA4bO8kk3as92MJusSHJrMy5fzntuUD_JCy3nzDtQnVlfAwhNO979jyTWSg?purpose=inline)

[xbtechstudio.com](https://xbtechstudio.com/blog/responsive-web-design-malaysia?utm_source=chatgpt.com)

설계 순서:

## **모바일 → 태블릿 → 노트북 → 데스크톱**

모바일은 화면 공간이 제한적이기 때문에 핵심 콘텐츠와 기능을 먼저 선택해야 한다.

**장점**

- 콘텐츠의 우선순위를 명확하게 정할 수 있다.
- 핵심 기능에 집중하기 좋다.
- 작은 화면에서 발생하는 문제를 초기에 발견할 수 있다.
- 모바일 사용자가 많은 서비스에 적합할 수 있다.

**주의점**

- 큰 화면에서 공간이 지나치게 비어 보일 수 있다.
- 큰 화면에서는 관련 콘텐츠, 필터, 보조 내비게이션 등을 추가로 고려해야 한다.
- 모바일 화면을 단순히 확대하는 것은 좋은 설계가 아니다.

## **7. 데스크톱 퍼스트 vs 모바일 퍼스트**

| 구분        | 데스크톱 퍼스트           | 모바일 퍼스트                |
| ----------- | ------------------------- | ---------------------------- |
| 시작 화면   | 데스크톱                  | 모바일                       |
| 설계 방향   | 큰 화면 → 작은 화면       | 작은 화면 → 큰 화면          |
| 초기 정보량 | 많은 정보 배치            | 핵심 정보부터 선택           |
| 주요 고민   | 무엇을 줄일 것인가?       | 무엇을 추가할 것인가?        |
| 장점        | 복잡한 화면 설계에 유리   | 콘텐츠 우선순위 정리에 유리  |
| 주의점      | 모바일이 복잡해질 수 있음 | 데스크톱이 비어 보일 수 있음 |

## **8. 모바일 퍼스트와 반응형 웹은 같은 개념일까?**

중요한 차이

두 개념은 서로 관련 있지만 의미가 다르다.

| 구분      | 반응형 웹                          | 모바일 퍼스트             |
| --------- | ---------------------------------- | ------------------------- |
| 의미      | 화면 크기에 대응하는 레이아웃 방식 | 화면 설계를 시작하는 전략 |
| 핵심 질문 | 화면이 바뀌면 어떻게 변경할까?     | 어떤 화면부터 설계할까?   |
| 목적      | 다양한 화면에서 사용성 유지        | 콘텐츠 우선순위 설정      |

따라서 다음 조합이 가능하다.

- 모바일 퍼스트 + 반응형 웹
- 데스크톱 퍼스트 + 반응형 웹
- 모바일과 데스크톱을 별도로 제작하는 적응형 웹

**모바일 퍼스트라고 반드시 반응형 웹인 것은 아니며, 반응형 웹이라고 반드시 모바일부터 설계하는 것도 아니다.**

## **9. 모바일 화면에서 콘텐츠 우선순위 정하기**

화면이 좁아질수록 모든 정보를 동일한 중요도로 보여줄 수 없다.

따라서 다음 질문을 기준으로 콘텐츠를 배치한다.

1. 사용자가 이 페이지에 들어온 가장 큰 목적은 무엇인가?
2. 반드시 확인해야 하는 정보는 무엇인가?
3. 가장 중요한 행동은 무엇인가?
4. 지금 보여주지 않아도 되는 보조 정보는 무엇인가?
5. 다른 화면이나 펼침 영역으로 이동할 수 있는 정보는 무엇인가?

중요도가 낮은 정보는 무조건 삭제하지 않고 다음과 같이 구성할 수 있다.

- 아코디언
- 탭
- 더보기 버튼
- 상세 페이지

## **10. 반응형 디자인에서 확인해야 할 요소**

| 요소        | 고려 사항                              |
| ----------- | -------------------------------------- |
| 그리드      | 화면 크기에 따라 열 개수 변경          |
| 콘텐츠 순서 | 모바일에서 자연스러운 읽기 순서        |
| 내비게이션  | 모바일 메뉴 및 하단 내비게이션         |
| 검색과 필터 | 검색 아이콘, 필터 버튼 등으로 단순화   |
| 글자 크기   | 작은 화면에서도 가독성 유지            |
| 이미지      | 화면에 맞는 크기와 이미지 크롭         |
| 버튼        | 손가락으로 터치하기 충분한 크기와 간격 |

### **반응형 디자인에서 자주 발생하는 실수**

- 데스크톱 화면을 비율대로 축소한다.
- 데스크톱과 모바일 시안만 만들고 중간 화면을 고려하지 않는다.
- 모바일에서 요소를 무조건 숨긴다.
- 브레이크포인트를 특정 기기 이름에만 맞춘다.
- 화면 크기에 따라 콘텐츠의 읽는 순서가 어색해진다.

## **핵심 요약**

**이번 강의에서 기억할 4가지**

1. **반응형 웹**: 하나의 구조가 화면 크기에 따라 유연하게 변경된다.
2. **적응형 웹**: 화면 환경별로 미리 준비된 레이아웃을 제공한다.
3. **데스크톱 퍼스트**: 큰 화면부터 설계하고 작은 화면으로 확장한다.
4. **모바일 퍼스트**: 작은 화면부터 핵심 기능을 설계하고 큰 화면으로 확장한다.

**가장 중요한 내용**

좋은 반응형 웹디자인은 화면을 단순히 축소하는 것이 아니다. 화면 크기가 달라져도 사용자가 동일한 목적을 자연스럽게 달성할 수 있도록 콘텐츠의 우선순위와 레이아웃을 설계하는 것이다.

## **프론트엔드 개발 관점에서 기억할 점**

| 디자인 개념      | 프론트엔드 구현                 |
| ---------------- | ------------------------------- |
| 브레이크포인트   | CSS Media Queries               |
| 그리드 변경      | CSS Grid                        |
| 요소 재배치      | Flexbox, Grid                   |
| 모바일 메뉴      | 반응형 Navigation               |
| 이미지 크기 조정 | `max-width: 100%`, `object-fit` |
| 화면별 스타일    | Mobile First Media Queries      |

예를 들어 모바일 퍼스트 방식의 CSS는 다음과 같아.

```
/* 모바일: 기본 1열 */
.card-list {
  display: grid;
  grid-template-columns: 1fr;
  gap: 16px;
}

/* 태블릿 */
@media (min-width: 768px) {
  .card-list {
    grid-template-columns: repeat(2, 1fr);
  }
}

/* 데스크톱 */
@media (min-width: 1024px) {
  .card-list {
    grid-template-columns: repeat(4, 1fr);
  }
}
```

출처: [디자인베이스 – 웹 디자이너가 알아야 할 필수 개념](https://designbase.co.kr/course/web-design-ui-foundations/lesson/web-design-1-3-2/?utm_source=chatgpt.com) · 강의 내용 기반 요약
