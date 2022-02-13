# Apocalypse-frontend

## 프로젝트 소개

종말된 시대에 알맞은 상품들을 판매하는 커머스 사이트

향수 판매 커머스 사이트인 JoMalone의 클론코딩 프로젝트 입니다.

## 개발 인원 및 기간

- 2022/01/25 ~ 2022/02/10
- 프로젝트 관리 : <a href="https://trello.com/b/CtBcsddi/first-project-apocalypse">Trello</a>
- Frontend : 김기만, 박재형, 이화종, 홍지은(4명)
- Backend : 김준영, 이강일(2명)
- <a href="https://github.com/wecode-bootcamp-korea/29-1st-Apocalypse-backend">Backend Git Reopository</a>

## 적용 기술

- Frontend : javascript, React.JS, Sass, React-router-dom
- Backend : Python, Django, Mysql, AWS(EC2, RDS, S3)
- 협업 및 일정관리 : Git, GitHub, Slack, Trello, Notion

## 구현 영상

[![프로젝트 구현 영상 링크](https://img.youtube.com/vi/rbnuJMyuUyM/sddefault.jpg)](https://www.youtube.com/watch?v=rbnuJMyuUyM)

## 구현 기능

#### 1. Nav Bar(김기만)

- MouseOver, MouseOut 이벤트를 이용한 SubNav
- SubNav 활성화시 BackGround 불투명화
- 제품 카테고리 API를 통한 제품 목록 구현
- 로그인 페이지 및 Token 저장
- Token 유무에 따른 Login, MyPage 변환
- 검색 API를 통한 제품 검색 -로그인 Token 보유 시 유저 장바구니 목록 및 제품 삭제 구현

#### 2. 제품 목록 리스트(김기만)

- RestFul API를 이용한 제품 필터링 기능
- sort Method를 이용한 가격기준 오름, 내림차순

#### 3. 고객 성향에 따른 제품추천(김기만)

- button click에 따른 질문지 전환
- reset button을 통한 상태 초기화
- button value를 통한 Filtering
