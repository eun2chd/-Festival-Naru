# 프로젝트명 : 축제나루
이 프로젝트는 기본 HTML, CSS, JavaScript를 사용하여 구현된 웹페이지로
사용자에게 동적인 콘텐츠와 직관적인 인터페이스를 제공하는 데 중점을 두었습니다.

추가적으로 JSON 데이터를 사용하여 데이터를 내부적으로 보관하고 이를 웹페이지에 동적으로 반영하는 기능을 구현하였습니다.
* * *
# 팀 구성 및 역할
### 4인 1조로 진행된 팀 프로젝트입니다.<br/>
저의 주요 역할:<br/>
JSON 데이터를 처리하여 웹페이지에 동적으로 콘텐츠를 추가하고 관리.<br/>
달력 페이지 구현: 사용자가 날짜를 클릭하면 해당 날짜와 관련된 축제 데이터를 보여주는 기능<br/>
* * *
# 주요 기능
+ 정적 웹페이지 구현:<br/>
  + HTML, CSS, JavaScript를 활용한 기본 웹사이트 구조 설계.<br/>
+ JSON 데이터 처리:
  + 데이터를 JSON 형식으로 저장하고, JavaScript로 동적으로 불러오고 활용.<br/>
+ 달력 기능:
  + 날짜별 데이터를 표시하며, 클릭 시 관련 콘텐츠를 제공.<br/>
  + 사용자 인터페이스를 통해 월 단위 탐색 가능.<br/>
  + 동적 콘텐츠 관리:<br/>
    + JSON 데이터를 기반으로 이벤트 정보와 상세 내용을 화면에 표시.<br/>
* * *
# 사용된 기술
+ HTML: 페이지의 구조 설계.
+ CSS: 레이아웃과 스타일링 구현.
+ JavaScript: JSON 데이터 처리, DOM 조작 및 이벤트 핸들링.
+ JSON: 데이터 저장 및 데이터 불러오기
* * *
# 프로젝트 경험
이 프로젝트를 통해 다음과 같은 점을 배웠습니다:

JSON 데이터를 다루는 방법:<br/>
데이터를 읽고, 처리하고, UI에 반영하는 기술. <br/>
JavaScript로 DOM을 동적으로 조작하고 달력을 구현하는 방식. <br/>
팀 프로젝트에서 역할을 분담하여 작업을 진행하는 협업 경험. <br/>
UI와 데이터를 통합적으로 관리하는 방법. <br/>

# 추가 개선 사항
+ 달력에서 검색 및 필터 기능 추가.
+ JSON 데이터를 외부 API와 연동하여 실시간 데이터 가져오기.
+ 사용자 경험(UX)을 향상시키기 위한 추가 기능 구현.
+ 해당 달력에서 날짜 클릭 시 해당 축제 화면으로 자동 스크롤 기능
+ 데이터를 불러올때 데이터가 많을 때 의 데이터 처리 [ 페이징 ]
* * *
# 각 페이지별 소개
 ## 메인페이지
### 메인페이지 메인화면에 각 지역에 대표하는 축제를 사용자가 볼 수 있도록 화면에 보여주도록 처리하였습니다.
![image](https://github.com/user-attachments/assets/08be8b8b-283c-4634-b273-e1fb738e94e9)
각 지역 위치별로 어떤 축제들을 볼 수 있는지 모아놓은 카테고리 입니다.
![image](https://github.com/user-attachments/assets/7486c5b4-5574-4d33-9133-665ebca8e986)
+ ## 전국 축제 카테고리 페이지
### 사용자는 지역별로 원하는 축제들을 모아 볼 수 있는 페이지 입니다.
![image](https://github.com/user-attachments/assets/56a43d34-dd65-4d3f-bd59-7021c9db09b8)
+ ## 달력 페이지
### 사용자가 해당 날짜에 어떤 축제들이 있는지 모아 볼 수 있는 페이지 입니다.
![image](https://github.com/user-attachments/assets/d2f157b4-2cb6-4c1b-85bf-6f6527f1f9fc)
+ ## 상세페이지
  ### 해당 축제가 열리는 상세 정보를 확인할 수 있습니다.
![image](https://github.com/user-attachments/assets/323687ce-ecac-456a-a27a-bebce69151a6)
![image](https://github.com/user-attachments/assets/c6851cac-c6fd-4453-8684-d4e137bc7a67)
![image](https://github.com/user-attachments/assets/7ff76def-d026-4987-89c6-6e21d6a9f9c5)
* * *
# 코드 및 개발과정
![image](https://github.com/user-attachments/assets/c9676839-51af-488d-baf0-811cce6432b6)
### 문제1 <br/> 처음 JSON 코드를 내부 script 파일로 작성을 했었는데 이 과정이 너무 코드도 길어지고 파일을 관리하기가 너무 어렵다고 판단하였다.<br/> 그래서 json 데이터를 따로 보관하고 필요한 곳에서 불러오는 방식을 적용해보고 싶었다.
### 해결과정1 : <br/> 다른파일을 불러올때는 비동기 처리방법이 있다는 것을 구글링을 통해 알게되었고 진행하던 프로젝트에 적용시켜보았다.<br>

파일을 불러오는 과정에서 여러가지 네트워크 오류가 있을 수 있고 해당 파일이 없을 수 있는 경우가 있기에 다음과 같이 예외처리를 진행해 주고었고 해당 경로에 있는 파일을 가져올 수 있었다
![image](https://github.com/user-attachments/assets/79d76f1c-b282-42cb-b9bd-9073931afb45)

### 문제2 <br/> 이렇게 축제데이터가 많이 나올 때 어떻게 해야 하나의 페이지로만 구성해서 각기 다른 화면을 표시해줄지에 대한 고민이 있었다. <br/>
상세 페이지는 1개만 만들고 사용자가 해당 축제를 클릭하면 그 축제에 맞는 상세 정보가 나와야하기 때문이다.<br/>
데이터를 다루는 과정에서 고민한 결과 json 데이터에서 해당 축제마다 고유 ID 값을 줘보자 라는 아이디어가 떠올랐다.<br/>
### 해결과정<br/>
A 라는 축제에 ID 값은 1번<br/>
B 라는 축제에 ID 값은 2번<br/>

이렇게 주고 해당 사용자가 축제를 클릭할때 쿼리스트링을 이용하여 id=1 이렇게 주소로 전달하게 되면 그값이 일치한지 검사하고<br>
id 값이 맞다면 그 해당 데이터를 화면에 보여주도록 처리하였다.<br/>
![image](https://github.com/user-attachments/assets/943fbcb3-9fd7-4b5f-b3ee-79d175add906) <br>
쿼리스트링을 이용하여 id값 전달<br>
![image](https://github.com/user-attachments/assets/d3169fc3-9203-47b0-a007-b237fa652b69)<br>
받은 id값<br>
![image](https://github.com/user-attachments/assets/c5185b09-636b-4595-a568-bb08c124607b)<br>
받은 id값과 저장된 id값이 같은지 비교하교 그 같은 id값에 해당하는 data 들만 출력<br>
![image](https://github.com/user-attachments/assets/fcfdd1d1-b748-4f99-a0c0-50ab685de8db)<br>




