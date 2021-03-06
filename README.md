# mashUp (4인 팀프로젝트)
## 구현동영상
https://youtu.be/nOvoq13RI1A
## 개요
- 서경대에 관심이 있는 일반인(학부모,예비서경인), 또는 재학생들에게 필요한 정보들을 담는 원페이지 사이트 개발
-	기존에 나와있는 API를 활용하여 다양한 정보를 원페이지에 담아 한번에 제공하여 원하는 정보를 쉽고 편하게 접근하도록 함
-	모바일 환경을 우선으로한 반응형 웹페이지 구현

## 기간 및 일정 
2018.06 ~ 2018.07 (한달)
## 기획

### 프로토타입
<div>
<img src="https://user-images.githubusercontent.com/50486476/77553462-2e8a9400-6ef8-11ea-9933-615f04d88503.png" width="30%" height="20%"></img>
</div>

## 개발환경
- windows10
- 모바일
  - Safari
  - 삼성브라우저
  - Naver app
  - Daum app
- 웹
  - Chrome
  - Internet Explorer

## 개발툴
- Sublime Text 3
- PyCharm

## 개발 언어
- JavaScript, JQuery, PHP, Python, Html, Css

## 사이트 구성요소
- D-DAY
- 공지사항 및 퀵 링크
- 날씨 
- 학식
- 버스
- 지도
- 도서관 좌석정보
- 인스타그램 피드

## 세부내용
### 지도 (맡은부분)
#### 목적
- 학교 주변 편의시설 등의 정보와 위치를 제공한다.
#### 내용
- 학교를 중심으로한 지도를 띄워 사용자들이 학교근처의 정보들을 우선적으로 볼 수 있게 한다.
- 학교 마커를 클릭하면 인포윈도우가 생성되고 그 안에 ‘서경대 길찾기’링크가 있는데,  해당 위치를 목적지로 지정한 상태의 길찾기 URL이 들어있다.
- 지도 안에 카테고리를 선택할 수 있는 버튼을 넣어 사용자들이 원하는 카테고리의 정보만 제공해준다.
- 컨트롤버튼으로 지도의 확대/축소를 쉽게 하도록 도와준다.
- drag on/off버튼을 추가하여 사용자가 모바일에서 사용할 때, 스크롤에 방해 되지 않게 한다. 

#### 구현방법

-	다음지도api의 key값을 발급받는다.
-	다음에서 제공하는 스크립트를 헤드에 포함시킨다.(지도 api키 입력)
-	다음에서 제공하는 라이브러리를 사용하여 javascript로 구현한다.
-	지도를 출력할 컨테이너를 설정한다.
-	위치객체와 지도객체를 생성하고 컨테이너에 삽입한다. 여기에 줌 컨트롤 객체,등 필요 정보 및 기능을 추가한다.
-	지도에 idle 이벤트를 등록하여 지도의 확대수준이 변경될 떄마다, 사용자가 선택한 카테고리에 해당하는 장소를 검색하여 마커로 표시한다.


#### 이슈
- 처음에 구글지도 api를 사용하려 했으나 정보가 부정확하고, 그 가짓수가 적어 다음지도 api로 교체함
- internet explorer와 chrome에서 카테고리 영역이 다르게 나타남
- ie전용 핵을 사용해 해결

## 보완점
- 아이폰 일정버전 이하의 경우 식단정보가 짤려서 표시됨
