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