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

#### 1. Nav Bar

- MouseOver, MouseOut 이벤트를 이용한 SubNav </br>
  Nav Menu에 MouseOver 시 Sub Menu Display: Block으로 변경</br>
  다른 Nav Menu에 MouseOver 시 기존에 열려있던 Sub Menu의 Display를 None으로 변경하고 해당 Sub Menu Display를 Block으로 변경함.</br>
  Sub Menu에서 MouseLeave 시 Sub Menu Display: None으로 변경</br>
  SubNav 활성화시 BackGround 불투명화</br>

- 제품 카테고리 API를 통한 제품 목록 구현</br>
  제품 카테고리 API의 상태를 저장하고 Map 함수를 사용하여 Component를 재사용함.</br>

- 로그인 페이지 및 Token 저장</br>
  Login Complete Message를 서버로부터 수신 시 해당 토큰을 sessionStorage에 저장함.</br>

- Token 유무에 따른 Login, MyPage 변환</br>
  SessionStorage에 Login Token 존재 유무에 따라 조건부 렌더링을 함.</br>
  Login Token이 없을 시 로그인 화면, Login Token이 존재하면 마이페이지 이동화면 구현</br>

- 검색 API를 통한 제품 검색</br>
  Input Value의 상태를 저장하고 Enter Key Event가 발생하면 서버에 해당 Value의 정보를 검색 요청하고 화면에 구현함.</br>

- 로그인 Token 보유 시 유저 장바구니 목록 및 제품 삭제 구현</br>
  SessionStorage에 Login Token이 없을 시 장바구니가 비어있음, Login Token이 존재하면 해당 유저의 장바구니 정보를 화면에 구현함.</br>
  Delete Method를 사용하여 삭제 버튼 클릭 시 해당 제품에 대한 정보를 서버에 삭제 요청하고 서버에 해당 유저의 장바구니 정보를 다시 요청하고 화면에 구현함.</br>

#### 2. 제품 목록 리스트

- RestFul API를 이용한 제품 필터링 기능</br>
  CheckBox 선택 시 set Method를 통해 상태를 관리하고 서버에 대한 CheckBox Value에 대해 Filtering을 요청함.</br>

- sort Method를 이용한 가격기준 오름, 내림차순</br>
  Sort함수를 통하여 가격 기준 제품에 대하여 오름, 내림차순 정렬을 구현함.</br>

#### 3. 고객 성향에 따른 제품추천

- button click에 따른 질문지 전환</br>
  상수 데이터를 활용하여 질문지 정보를 저장하고 상시로 업데이트를 할수있도록 구현함.</br>
  질문지 버튼 클릭 시 버튼 Value의 상태를 저장하고 다음 질문지로 화면을 전환시킴.(Node Method를 활용하여 추적함)</br>
  결과보기 버튼 클릭 시 저장된 Value 상태를 서버에 Filtering 요청함.(서버에 구현되지 않아 Mock Data를 활용함)</br>
  Filtering 된 제품을 화면에 구현함.</br>

- reset button을 통한 상태 초기화</br>
  reset 버튼 클릭 시 초기화면으로 돌아가며 저장된 Value 상태를 초기화 시킴.</br>