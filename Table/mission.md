#### 1번

[move to site](https://www.post.japanpost.jp/int/UGX/charge_kr.html)

#### 2번 (스크린 리더 사용)

1. 해당 데이터 테이블의 페이지 내용을 확인하기 위해 링크를 클릭 후 tab을 통한 본문 접근 불가
2. thead, th, scope 등 연관성 활용하지 않고 단순한 tr,td 마크업
3. 데이터 테이블 양이 많아서 스크린 리더로는 활용하기 힘듬
4. caption은 사용 x

#### 3번 (WCAG 가이드라인)

1. 논리적 관계로 데이터를 구성해야하며, 이들을 정의하는 HTML 마크업 필요
2. 머리글 th, 데이터 셀 td, scope id, headers 속성
3. 본 사이트 테이블은 두 개의 머리글 사용함으로 scope 속성 col, row 사용
4. caption은 필수는 아니나 제공하여 데이터 탐색에 대한 힌트

#### 4번

1. 마크업 오류 방지
2. 표를 이해할 수 있도록 정보 제공, 쉽게 구성

#### 5번 구현

#### 6번 검사

![html-check](https://user-images.githubusercontent.com/69140464/136010643-0daa253b-6d96-4d6c-93ab-74f43e52bec3.PNG)
![css-check](https://user-images.githubusercontent.com/69140464/136010659-350a9ba8-df8f-4fa0-a2f0-7b6a11631c6f.PNG)

#### 7번 리포트

![lighthouse-check](https://user-images.githubusercontent.com/69140464/136012530-d2843c05-5ab4-4de0-8b1f-13cf64f690ec.PNG)

#### 8번 후기

- 시행착오

1. 스크린 리더를 통한 tab 이동 순서를 논리적으로 구현 하고 싶었지만 특정 태그는 자동으로 tab으로 이동하여 논리적으로 구현하기 힘들었음

2. 자료 조사를 위한 웹 페이지 선정 과정에서 생각보다 데이터 테이블을 접근성을 잘 지키려 하는 곳이 많았으며, 또한 많은 사이트 들이 시각적인 효과, 반응형 웹을 선호하여 웹 선정에 시간이 소요됬음

- 아쉬운 점

1. 우체국 웹 페이지 처럼 skip-nav를 통한 주소창에서 tab 시 본문 바로가기가 화면 제일 상단에 나타고 바로 데이터 테이블 제목으로 이동하게 구현 하고 싶었으나 시행착오를 겪는 단계라 우선 display:none; 선언
2. aria-label, aria-describedby, role="rowgroup",role="cell", role="row", header 만 사용하여 구현 해보고 싶었으나 시간이 부족했음

- 성장기

1. 요번 과제를 통해 table 각각의 속성들을 한번더 공부하며, 각각의 속성들이 화면에서 어떤식으로 나오는지 숙지하게됨

2. 선정했던 웹 사이트의 데이터 테이블 양이 많아서 스크린 리더기를 통한 확인 과정에서 테이블을 이해하기 곤혹스러웠으며, 스크린 리더기를 통한 웹 사이트 이용자에 대한 준비가 적은 점이 아쉽게 느껴졌음
