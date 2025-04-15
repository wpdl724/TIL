# TIL
##  VS 코드 주요 단축키
* `Ctrl + K` -> `Ctrl + \` 위/아래 화면 분활
* `Ctrl + \` -> 좌/우 수평 화면 분활
* `Ctrl + J` -> 터미널 실행 / 닫기 
* `Q`or `Ctrl + C` -> 터미널 입력안되는 에러 해결 단축키 
## 작업 폴더 설명
* `html_basic/` : html 기초 연습파일 모음
* `task/` : 과제 제출 폴더, 파일 모음(폴더명은 날짜별로 구성됨)
* `README.md/` : 배운 내용 기록, 어려운 점 및 막힌 점 자유롭게 정리
### 2025/04/04 | HTML 3일차 문서
* `h1~h6`, `p`, `br`, `strong`, `em`, `del`, `s`, `sup`, `sub`
### 202/04/07 - HTML 4일차
* `div`, `span`
* 웹/앱 레이아웃 방향과 의미에 따라 2개 이상의 요소를 묶어주는 레이아읏 요소
* `div`는 생성 시 반드시 그룹을 구분 할 수 있는 이름을 설정해야 한다. 
`span`은 선택! 
* 이름 작성시 주의사항 : 반드시 용도에 맞는 의미있는 영단어 사용!!
## HTML 구조 공부 순서
1. 클론 코딩 & 클론 디자인 할 사이트 정하기
2. 피그마에서 와이어프레임 만들기(레이어, 폴더 이름 주의)
3. 피그잼에 일부 화면 넘겨서 태그 계획하기
4. 계획한 태그를 가족관계에 맞게 트리구조 만들기
5. VS code에서 실제 HTML 작성하기 (트리구조 순서에 맞게 바깥쪽 -> 안쪽 순서로!)
### 다른 환경에서 git 이어서 작업하기
1. 새폴더 연결하기
2. `git clone 저장소 주소 붙여넣기`
3. `cd 저장소 폴더명`
4. `파일 받고 파일 수정 및 내용 추가 한 다음, 저장하기`
5. `git status` 상태 확인
6. `git add . `
7. `git commit -m '메세지'`
8. `git push origin main` 저장소 업로드
### (위 이어서) 다른 환경에서 git 이어서 작업하기 (학원)
* `git pull origin main` 집에서 올린 파일 내려받기
-----
### 바로가기 메뉴 만들기
0. (조건) 화면이 수직으로 충분히 이동 할 수 있을 만큼 세로 스크롤 준비
1. 바로가기 메뉴 a 태그 준비하기
2. 바로가기 위치 div id 명 준비하기
3. 위 1번 `a` 속성 `href`값으로 `#` 먼저 작성 후 위 2번 이름 작성하기
4. 위 3번 결과 예시) id가 abcd일 경우 `<a href="#abcd"></a>
### 링크 복습
* 임시링크 `<a href="#"></a>` -> 의미 : 연결페이지 제작 전 일 경우
* 바로가기 링크 `<a href="#header"></a>` -> 의미 : 같은 파일 내 다른 위치 이동
* 상대경로 이동 `<a href="./basic/index.html"></a>` 
* 특정 아이디 위치로 이동 (상대경로+바로가기 링크) `<a href="./basic/index.html#main"></a>`
### 자주 쓰는 글꼴 주소
1. Pretendard -> `<link rel="stylesheet" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.9/dist/web/static/pretendard-dynamic-subset.min.css" />`
2. Noto Sans KR -> `<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@100..900&display=swap" rel="stylesheet">`
### CSS style sheet
* 외부스타일시트 파일 저장 **styles** 폴더에 저장한다. `파일명.css` 저장한다
* 위 파일 생성 후 CSS연결을 원하는 HTML파일 head위치에 `<link>` 태그로 연결한다.
* HTML 작성 후 HTML의 모든 디자인형태를 초기화 하는 `reset.css` 반드시 연결!
* 웹 글꼴(Noto Sans KR, Pretendard 등) 연결시 HTML파일에 `<link>` 태그 연결!
### head 태그 내에 들어가는 link 태그 작성 순서
1. 웹글꼴 포함 기타 플러그인 연결 주소
2. reset.css
3. 해당 HTML별 디자인 .CSS
### 디자인 CSS 작성시 작성 순서 및 주의사항 
* **부모->자식** 순서로 가장 바깥쪽 부모부터 먼저 선택자를 만들고 디자인 한다.
* 레이아웃 관련 요소에 `width, height` 속성 작성 시 영역 확인을 위한 `background-color`를 꼭 함께 작성해서 정확히 구분한다. 이때 색상은 쉬운 영역 구분을 위한 `aqua, lime, yellow, pink` 등의 밝은 색상 위주로 사용한다. 영역 확인과 디자인 작업을 모두 마친 후 위 색상은 제거로 마무리 해야한다.
* 실제 디자인에 들어가는 색상은 **rgba 또는 헥사코드**로 입력하고 테스트용으로 입력하는 임시 색상은 영문명으로 입력해야 한다.
### 자주 이용하는 CSS 속성 값과 기본값 
* `letter-sapcing`자간 설정  | 기본값 0 | 사용 예시 letter-spacing : -0.02rem;
* `line-height` 행간 | 1 또는 100% | line-height :1.5;
* `font-size` 글자 크기 | 16px (1em)| font-size : 1.2rem;
* `color` 글자색상 | |color #f00 color :rgba(0,0,0,0.5);
* `background-color` 배경색상 | | background-color :#000;
* `width` 가로 크기 | |width : 100px;
* `height` 세로 크기 | |height :200px;
* `margin` 바깥쪽여백 | |margin-top : 50px;
* `border-radius` 모서리 둥글기| |border-radius : 10px;
* `font-weight` 글자 굵기 | | font-weight: 400
* `font-family` 글꼴 설정 | |font-family :'대표글꼴', '보조글꼴', sans-serif;