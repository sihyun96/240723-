# 공부일지 (240723 - 241220)
## 241211
### react
- 리액트 스와이퍼 적용하기
1. npm i swiper 인스톨
2. npm i sass 인스톨 (다운받은거 확인하려면 package.json 파일 확인)
3. 스와이퍼에 이미지 첨부
   1) assets에 img를 가져오려면 import로 불러와야함 그리고 img태그에 참조변수 사용
   2) public에 img를 가져오려면 {process.env.PUBLIC_URL + "절대경로"}로 사용 
   3) const path = process.env.PUBLIC_URL {path(변수명) + "절대경로"}도 사용가능 
   4) background-image scss에 작성 (중첩 작성가능)
       assets이미지 파일을  background: url(../assets/images/bg4.png); 작성
   5) 플러그인의 버튼 변경시 변수를 가져와 변경
       --swiper-theme-color: orange;
4. build해서 github에 올리기
   1) 컨트롤 + C 눌러 작업 종료
   2) 해당되는 경로에서  npm run build
   3) build index.html 경로 수정
   4) build폴더만 github에 업로드

## 241210
### react
- 리액트 웹앱 만들기 연습
1. 컴포넌트 만들어 웹 페이지 만들기
2. npm run build입력 하여 git에 올릴 수 있게함
3. build에 index파일 경로 수정하기
3. git에 업로드하기

## 241209
### react
- react 사용방법 복습
1. 폴더 만들기
2. basic 파일 복사해서 붙여넣기
3. 터미널 cmd 오픈
4. 폴더로 경로 이동
5. npm i 로 인스톨
6. 인스톨 완료후 npm start 가상서버 오픈

- assets style 적용 방법 
1. src폴더 안에 assets생성
2. 적용할 font index.css안에 @import url(); 작성
3. StyleModule.jsx 생성
4. 적용할 css "import styles from './StyleModule.module.css';" imprt 변수 from url 작성
5. return 안에  <section className={styles.wrapper}> 변수+적용할 css 스타일 작성
6. style 여러개 적용시   
   1) className={`${styles.bg} ${styles.fontSize}`}
   2) className={`styles.listStyle ${styles.underline}`} 
   3) className={[styles.listStyle, styles.underline].join(" ")}
7. css에 :global 작성 모든 페이지에서 사용가능 일반 css문서 적용방법처럼 사용

- SCSS 스타일 적용
1. 파일명.scss / 파일명.module.scss
2. 변수 작성시 $변수명 : style; / 지역변수 스타일 안에 작성
3. jsx 파일에 import styles from "./SCSS.module.scss"; 작성
4. return 안에  <section className={styles.wrapper}> 변수+적용할 css 스타일
5. 터미널에서 npm i sass 입력해서 설치
6. npm start 입력

- 하위 스타일 적용
1. .wrapper .title {} -> .wrapper { .title {} }
2. hover적용시 스타일 중가로 안에 $:hover 작성

- styled-components
1. 터미널에서 npm install styled-components 패키지 설치
2. 적용방법
   1) const 컴포넌트명 = styled(참조변수명).태그명`css 적용값`;
   2) const 컴포넌트명 = styled.('태그명')`css 적용값`;
3. ainmation 적용방법
   1) 실행 컴포넌트 앞에 작성
   2) const mov = keyframes`css 작성 방법과 같음`;

##241206
## react
- set함수를 이용하여 데이터 업데이트에 대해 배웠다.

## 241205
### react
1. vscode 터미널 열기 cmd ( command prompt)
2. npx create-react-app 폴더이름 입력
3. 만들어진 폴더에 들어가서 npm start 입력
4. readme파일, 삭제
5. App.js 안에 내용지우고 "rs"' 단축키 사용(reactjs code snippets 설치)
6. return 안에 내용 작성
7. src 안에 components폴더 생성 StyleCom1.jsx 생성
8. 작성한 파일은 App.js에 연결 
   1) JS영역에 import StyleCom1 from './components/StyleCom1'; 작성
   2) JSX영역에 <StyleCom1 />작성

- JSX 문법 삼항연산자 논리연산자에 대해 배웠다

## 241204
### react
- 노드파일설치와 프롬프트로 확인하는 방법을 배웠다.
- 리액트 파일설치와 vscode에서 작성 방법에 대해 배웠다.

## 241203
### react
- kakaoAPI를 이용하여 데이터를 가져오고 출력하는것에 대해 배웠다. 
- 구조분해할당, map, 삼항연산자, 단락회로평가, filter, spread연산자에 대해 배웠다.

## 241202
### react
- JSON에 대해 배웠다.
- Fetch, async+await, jQueryAjax에 대해 배웠다.

## 241129
### gsap
- 흐르는 글자 만들기

## 241126-241128
### gsap
- gsap를 이용한 홈페이지 만들기 연습

## 241125
### gsap
- onepage 만드는 예제를 연습했다.
- gsap에대해 배웠다

### 241122
## jq 
- horizontalScrolling에 대해 배웠다.
- onepage 만드는 예제를 연습했다.

## 241121
### jq
- swiper 이용하여 슬라이드 만들기
- resize에 대해 배웠다.
- 마우스좌표에 대해 배웠다.

## 241120
### jq
- 반응형 웹사이트 구조 만들기 연습
- vegas 플러그인 사용하여 이미지 슬라이드 만들기 

## 241119
### jq
- scrollY와 offset을 이용해 메뉴가 content까지 스크롤을하면 안보이게 숨기는 예제를 연습했다.
- scrollTo를 이용한 up-btn 만들기

##241118
### jq
- scrollTop ,scrollLeft, scrollTo, scrollBy, scrollIntoView에 대해 배웠다.
- window 객체사이즈에 대해 배웠다.

## 241115 
### jq
- setInterval을 이용한 auto슬라이드 만들기

## 241114
### jq
- delay로 애니메이션 대기 후 실행에 대해 배웠다.
- animate 배운것들을 토대로 5가지 예제를 연습했다.

## 241113
### jq
- hasClass 기준요소에 해당 클래스가 있으면 true, 없으면 false반환에 대해 배웠다.
- prependTo 부모인 a의 자식들 중 b를 자식들 중 제일 처음으로 이동, appendTo는 제일 마지막으로 이동에 대해 배웠다.
- jquery-ui 적용에 대해 배웠다.

## 241112
### jq
- html, text, attr, addClass, removeClass, toggleClass에 대해 배웠다.
- 사진을 클릭하면 메인화면에 사진이 나오는 예제와 탭 메뉴를 만드는 예제를 연습햇다.

## 241111
### jq
- fadeIn, fadeOut, fadeToggle, show, hide, toggle에 대해 배웠다.
- 메뉴를 클릭하면 서브메뉴가 나오는 예제를 연습했다.

##241108
### jq
- jq의 기본구조에 대해 배웠다.
- css에서 DOM을 탐색하는법에 대해 배웠다.
- eventMetgod에 대해 배웠다.
- 버튼을 클릭하면 모달창이 나오는 예제를 연습했다.

## 241107
### js
- 이벤트 제어 전달에 대해 배웠다.
- script링크에 defer를 적용하는 것에대해 배웠다.
- jQuery 스크립트 파일 로컬버전 작성하는 것에대해 배웠다.

## 241106
### js
- DOM객체-탐색, 표준속성에 대해 배웠다.
- js에서의 클래스 선택자를 제어하는 것을 배웠다.
- 버튼을 클릭하면 이벤트가 일어나고 클래스가 나왔다 없어졋다 하는것을 배웠다.

## 241105
### js
- 함수표현식을 작성하여 함수 예제 연습했다.
- 함수와 배열을 이용하여 버튼을 클릭하면 console에 나오는 예제를 연습했다.
- 한 줄 작성시 값이 나오지만 두 줄 일경우 return 키워드로 값을 반환해야하는 화살표 함수에 대해 배웠다.
- this키워드에 대해 배웠다.
- setTimout으로 정해진 시간뒤에 실행하고, setInterva로 반복실행에 대해 배웠다.

## 241104
### js
- String객체와 배열Array에대해 배웠다.
- 호출하여 실행되는 함수 function에 대해 배웠다.

## 241101
### js
- break키워드: 이 키워드를 만나는 즉시 구문을 빠져 나옴
- continue 키워드: 이 키워드를 만나면 그 뒤의 구문을 건너띄고 반복문 처음으로 돌아감
- while 반복문 초기값, 증감식에 대해 배웠다.
- 객체Object: 객체, 함수, 배열, 정규 표현식 등 변형 가능한 데이터들의 집합
- Date객체: 날짜와 시간을 생성하는 내장 객체이자 생성자 함수
- Math 객체: 수학과 함수를 위한 속성을 제공하는 내장객체 

## 241031
### js
- for반복문 초기값, 조건식, 증감식에 대해 배웠다.
- 변수scope let과 var에 대해 배웠다.

## 241030
### js
- if조건문에 논리연산자를 이용하여 설정한 값을 출력하는 예제를 풀었다.
- 특정 값과 비교하여 실행하는 switch 선택문에 대해 배웠다.

## 241029
### js
- 비교연산자, 대입연산자, 논리연산자에대해 배웠다.
- if 조건문, else-if 조건문에 대해 배웠다. 
- 변수에 입력창을 대입하여 if 조건문 예제를 풀었다.

## 241028
### js
- 데이터타입 String, Number, Bollean, undefined, null, object, Function, Array, typeof에 대해 배웠다.
- 문자열연산자, 산술연산자, 증감연산자에대해 배웠다.

## 241025
### js
- 자바스크립트 대해 배웠다.
- 자바스크립의 내부선언과 외부선언에 대해 배웠다.
- Dialog의 다양한 사용자 입출력, 알림에 대해 배웠다.
- variable 변수에대해 배웠다. 

## 241024
### reponsiveWeb
- 아이콘에 hover하면 tranform: translateY 를 이용하여 위로 올라가는 애니메이션 효과를 적용해보았다.
(overflow: hidden을 이용해 지정된 구역을 넘으면 아이콘이 보이지 않게 하였다.)
- 애니메이션 효과를 줄때 영역을 넘어가 떨리는 현상이 생기는데 상위에 overflow:hidden을 넣어 중첩되는 이벤트들의 문제를 해결하였다.
- codpen 사용방법에대해 배웠다.

## 241023
### reponsiveWeb
- class에 active를 넣어 css 종속선택자로 값을 미리 적용시키는것을 배웠다.
- svg에 fill을 이용하여 색상을 변경해보았다.
- pc버전 웹 만들기
- 포지션 초기화하는 방법 복습을 하였다.
position: static;

## 241022
### reponsiveWeb
- 지역 변수 선언에 대해 배웠다.
- backdrop-filter 요소 뒤로 그래픽 효과 적용에 대해 배웠다.
- swiper 스크립트 적용에 대해 배웠다.

## 241021
### reponsiveWeb
- 모바일버전 웹 만들기.
- css 변수에 대해 배웠다.

## 241017-241018
### web
- 반응형 웹 만들기 과제를 내주셔서 지금까지 배운내용으로 홈페이지를 보고 따라 만드는 활동을 했다.

## 241016
### mq
- 미디어쿼리 선언방식을 배웠다. 

## 241014
### mq
- viewport가 있는 페이지와 없는 페이지의 차이점을 확인했다.
- 미디어쿼리란? 
화면 해상도, 기기 방향 등의 조건으로 HTML에 적용하는 스타일을 전환할 수 있는 CSS3의 속성 중의 하나이다.

## 241011
### grid
- grid 예제 연습했다.

## 241010
###grid
- grid container, grid item 속성에 대해 배우고 행/열 추가, 정렬 기능을 연습했다.

## 241004-241008
### web
- 반응형 웹 만들기 연습

## 241002-241003
### web
- pc버전 웹 만들기 과제를 내주셔서 지금까지 배운 내용을 활용해 웹 사이트를 따라 만드는 활동을 했다.

## 241001
### ani
-  animation 예제 연습했다.

## 240930
### ani
- css로 animation 효과를 적용하는 법을 배웠다.

## 240929
### trans
- transform 배운것을 활용하여 이미지 메뉴 만들기 과제를 만들었다.

## 240927
### trans
- transform을 활용해 움직이는 메뉴, 버튼 등을 제작하는 연습을 했다.

## 240926
### trans
- 움직임 속성인 transform 기준축, 크기, 기울기, 회전, 이동에 대해 배웠다.
- tranform을 이용하여 포지션 중앙정렬 하는 방법을 배웠다.

##240925
### layout
- 이미지나 비디오 비율을 object-fit으로 조절하는 방법을 배웠다.
- aspect-ratio로 비디오 비율 조절하는 방법을 배웠다.

##240924
### layout
- header nav의 레이아웃 구성을 해 보았다.

## 240923
### position 
- 스크롤 바를 설정하는 방법과 position-sticky, 요소 계층 순위를 결정하는 z-index에 대해 배웠다.

## 240919
### position 
- 요소의 배치를 설정하는 position(static, relative, absolute, fixed, sticky)를 배웠다.

## 240913
### layout
- html과 css에서 배운 내용을 활용해 웹페이지 레이아웃 구성을 해 보았다.
- webFont css에 적용하는 방법을 배웠다.
- common, header, footer css를 분류하여 스타일에 적용시켜 보았다.
 
## 240912
### layout
- html과 css에서 배운 내용을 활용해 웹페이지 레이아웃 구성해 보았다.

## 240911
### layout
- header contents footer의 레이아웃을 구성하여 웹에 적용하는법에 대해 배웠다.

## 240910
### layout
- grow로 비율 설정하는 방법과 order로 우선순위를 설정하는법을 배웠다.
- gradient의 방향과 색상을 적용시키는 방법을 배웠다.

## 240909
### layout
- 배경 이미지 위치 설정과 사이즈 비율을 설정하는 방법을 배웠다.

## 240906
### layout
- inline flex 적용법과 수열 선택자에 대해 배웠다.

## 240905
### layout
- 다양한 flex 속성을 form에 적용하는 법과 이미지, 텍스트 정렬에 대해 배웠다.

## 240904
### layout
- flex 속성으로 레이아웃을 구성하는 방법에 대해 배웠다.

## 240902
### layout
- gap, flex flow, justify, align 등 flex 속성에 대해 배웠다.

## 240829
### layout
- em, rem, viewport 단위와 계산법에 대해 배웠다.
- display로 메뉴 버튼을 제작해보았다.

## 240828
### box
- 요소의 성격을 변경하는 display, visivility, opacity에 대해 배웠다.
- box-sizing 중 content-box와 border-box의 차이를 배웠다.

## 240827
### box
- margin과 padding 배운 내용으로 마우스이벤트, 새창이동, 중앙정렬 예제를 만들었다.

## 240826
### box
- overflow로 넘치는 컨텐츠 제어하는법을 배웠다.
- boder-radius로 둥근 모서리 만드는법을 배웠다.

## 240823
### css
- 박스와 콘텐츠 영역 사이 여백인 padding, 박스의 테두리 border, 박스 모델 간의 여백 margin에 대해 배웠다.

## 240822
### css
- css 상속, style으로 form의 텍스트 설정하는 법을 배웠다.
- 의사 클래스와 의사 요소, 속성 선택자, 형제 선택자를 배웠다.

## 240821
### css
- 줄 바꿈, 폰트, 색상, 정렬, 그림자 등 css를 활용한 텍스트 설정에 대해 배웠다.

## 240820
### css
- css 우선순위와 color에 대해 배웠다.

## 240819
### html
- favicon, 설정에 대해 배웠다.
- 문서가 담고 있는 내용, 키워드를 확인할 수 있는 오픈그라피에 대해 배웠다.
인스타그램, 카카오톡, 트위터 등 각종 SNS별로 다른 오픈그라피 등록 방법을 배웠다.

## 240816
### html
- form 관련 태그(minlength, required, checked, disabled 등)와 작성법에 대해 배웠다.
- 오디오, 비디오를 html로 첨부하는 방법을 배웠다.

## 240814
### html
- 페이지안에서 특정위치로 이동하는 방법을 배웠다.
- html에 이미지를 첨부하고 사이즈를 조정하는 법, 인라인 성격에 대해 배웠다.

### 피그마
- 도형안에 이미지 넣는법을 배웠다.
- 아이콘 터치영역 프레임에대해 배웠다.
- 오토레이아웃으로 정렬하는법을 배웠다.

## 240813
### a
- 절대경로 구조를 만들고 html로 각 경로를 작성하는 연습을 했다.

### 피그마
- 넛지, 그리드, 프레임에 대해 배웠다.

## 240812
### a
- 중첩 목록, 절대경로, 상대경로, 하이퍼텍스트 작성법을 배웠다.

### 포토샵
- 선명도, 색상보정에대해 배웠다.
- gif 만드는법을 배웠다.

## 240809
### html
- 블록요소 ol, ul에 대해 배웠다.

### 포토샵
- 카드뉴스를 만들어보고 글자레이어에 효과를 적용하는법을 배웠다.

## 240808
### html
- html에서 사용되는 태그들에 대해 배웠다. (h, p, br, hr, cite, strong, em 등)

### 포토샵
- 스마트오브젝트에 대해 배웠다.
- 패턴 만드는법을 배웠다.

## 240807
### html
- html의 기본 구조에 대해 배웠다.
- git hub requests 하는 방법을 배웠다.

### 포토샵
- 이미지 선택영역 지정하는 방법 배웠다.

## 240806 
### git
- git 과 git hub 연결하고, 충돌에 대해 배웟다.
- 마크업 문서 생성 및 내용작성을 하였다.

### 포토샵
- 캔버스 , 이미지 사이즈 조정 방법을 배웠다.
- contents aware으로 변형 없이 이미지를 조정하는 법을 배웠다.

## 240805
### git
- 로컬 git 과 온라인 github 연결하기에대해 배웠다.

### 일러스트
- 일러스트 툴 배운것을 활용하여 이벤트 배너를 만들었다.

## 240725
### git
- 브랜치의 개념을 배워 main / sub / dev 브랜치를 생성하고 이동해보았다.

### 일러스트
- 패스파인더를 활용해 패스를 합치고 나누는 법을 배웠다. (divide, trim, merge, crop, outline 등)
- 정렬 도구 align으로 오브젝트를 정렬하는 법을 배웠다.

## 240724
### git
- git  저장소 만들기와  git 명령어에대해 배웠다.

### 일러스트
- 펜툴 방향선 이동, 기준점을 추가/삭제해 패스를 변형하는 법을 배워 패스 그리는 연습을 했다.

## 240723
### git
- git 프로그램을 설치했다. add, commit, status, log 등의 명령어를 활용해 파일을 생성, 병합, 삭제하는 법을 배웠다.

### 일러스트
- 일러스트 툴 활용법과 단축키, 펜툴 사용법을 배웠다.
