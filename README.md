# 부동산 매물 관리 웹사이트🏠 
![부동산 매물 메인페이지](https://user-images.githubusercontent.com/57031319/182023527-b8a4d910-7e3f-4c7b-8d84-bd352b8dd56b.png)

## ✏프로젝트 소개
1. 일반회원, 중개사회원, 관리자로 나누어서 서비스를 제공하는 사이트입니다. 
2. 일반회원은 위치 기반 매물 조회 및 매물 계약을 할 수 있습니다. 
3. 중개사는 매물을 등록할 수 있으며 회원과의 매물 계약을 진행할 수 있습니다. 
4. 비대면으로도 계약서를 주고받고 계약까지 이루어질 수 있도록 제공하였습니다.

## 📆개발 기간
2022.07.11 ~ 2022.07.22

<h2> 개발환경 </h2>
- Oracle Database 11g
- Java 11, Eclipse
- 개발 언어: JAVA, JSP, HTML5, CSS3, JS ES6

<br>
<h2> ⚙핵심 기술 </h2>
- MVC 패턴 사용
- Open API - 카카오 맵 API(좌표 찍기, 편의 시설, 클러스터러), 주소 검색API, 메일 인증API, 부동산중개업사무소정보조회API
- 라이브러리 - chart.js(막대 그래프), cos.jar(파일 업로드), bootsrap(디자인 활용), mail.jar, activation.jar(이메일 인증 구현)

<br>

<h2>핵심 업무</h2>
  <h3>회원</h3>
  
  
  - 매물 조회 : 회원은 위치에 따른 매물을 조회할 수 있으며 선택한 매물에 대한 상세 정보를
확인할 수 있다. 또한 지도를 통한 매물 주변 편의시설을 확인할 수 있다. 
  - 상담 신청 : 회원은 상담하고 싶은 매물을 선택해 중개사에게 상담을 요청할 수 있다. 
  - 허위 매물 신고 : 회원은 허위 등록된 매물에 대하여 허위 매물 신고를 할 수 있다. 
  - 후기 게시판 : 회원은 자신이 거래했던 매물에 대하여 후기 게시판을 작성할 수 있으며 수정, 
삭제도 가능하다. 또한 다른 사용자가 등록한 후기 게시판 글도 조회할 수 있다. 
  - 매물 거래 : 회원은 원하는 매물을 선택해 입주 날짜를 선택하고 중개사에게 매물 거래를 요
청할 수 있다. 중개사가 거래 요청을 승인한다면, 중개사가 전송한 계약서에 정보 작성 후 서
명을 하고 거래가 완료된다. 
  - 본인이 요청한 계약의 목록과 계약 상태를 확인할 수 있다.
  - 본인이 요청한 상담 목록을 조회 할 수 있고 상담이 완료되면 별점 후기를 남길
수 있다.
  
  <h3>중개사</h3>
    
  - 매물등록 : 중개사 회원은 매물 정보를 등록할 수 있다.
  - 매물관리 : 중개사 회원은 매물 정보를 삭제 할 수 있으며, 계약 상태를 확인 할 수 있다.
  - 비대면 계약 : 중개사는 회원의 계약 요청을 승인, 거절 할 수 있다.
  - 마이페이지-거래목록 : 중개사는 중개사의 계약이 성사된 매물의 정보와 계약서를 조회 할 수 있고, 임대인, 매수인이 후기를 남긴 경우 매물 거주 후기를 조회할 수 있다.
  - 마이페이지-상담목록 : 중개사는 일반 회원이 요청한 상담을 처리 할 수 있고, 중개사의 모든 상담 목록과 처리여부를 조회할 수 있다.
  - 후기 게시판 조회 : 중개사는 회원이 등록한 후기 게시판을 조회할 수 있으며 자신의 매물에 등록된
후기 게시판만 선택적으로 조회할 수도 있다. 


<br>


### 1. 아이디 중복 검사 및 이메일 중복 검사 
- ajax를 이용하여 아이디 중복 검사, 유효성 검사 및 이메일 중복 검사를 실시하였습니다. 
- 유효성 검사는 정규화 표현식을 사용하였습니다. 
<br>
<img src="https://user-images.githubusercontent.com/57031319/182016081-2d632b23-8720-4472-a779-df1f3a40329b.gif" style="width:600px"></img>

<br>

### 2. 메일 인증 API 사용 화면
- '인증 메일 보내기'를 선택하면 ajax를 이용하여 인증번호를 전송하고, js function으로 인증 체크 폼을 생성되게 하였습니다.
- 인증번호를 입력했을 때 일치하면 메일 인증이 완료됩니다. 
<br>
<img src="https://user-images.githubusercontent.com/57031319/182016136-b3284ab6-723d-46eb-94bb-15852d6c81b4.gif" style="width:600px"></img>

<br>

### 3. 주소 검색 API 사용 화면
- 주소 검색 API를 사용하여 도로명 주소를 검색한 후 선택한 
<br>
<img src="https://user-images.githubusercontent.com/57031319/182016185-57bcd82d-d836-4033-a11f-f4fb7c69acf5.gif" style="width:600px"></img>

<br>

### 4. 중개사 회원가입 시 중개사무소 조회 API 사용 화면
- 부동산중개업사무소정보조회API를 사용하여 국가공간정보포털의 부동산중개업 정보에 등록된 정보를 모두 조회할 수 있게 하였습니다.
- 조회하려던 중개사무소 회원가입 양식에 자식창에서 부모창으로 값을 옮겨서 자동 입력되게 하였습니다. 
<br>
<img src="https://user-images.githubusercontent.com/57031319/182016241-a10dba1c-5b58-42f8-b0c8-9a5a8c5a82de.gif" style="width:600px"></img>

## 제작 후기
- 같은 사이트를 여러 명이서 구현하다 보니 여러 번의 회의를 통해 공통 디자인 양식을 처음에 정하고 갔었다. 글씨 크기, 버튼 디자인, 글씨체 모두 하나하나 맞춰서 미리 공통css에 제작해놓고 정해놓은 것만 가져가서 쓰게 하였다. 그래서 전체적인 사이트 분위기를 통일할 수 있었다. 
- MVC 패턴에 대한 개념이 머릿속에는 있어도 실제로 구현해보기 전에는 크게 와닿지 않았는데 직접 구현해보니까 MVC 패턴에 따른 전체적인 웹사이트 제작 흐름을 더 자세히 알 수 있었다. 
- ajax 비동기 통신에 대해서 더 많은 연습이 필요할 것 같다. 현재 만든 결과물에 만족하지 않고 코드를 더 발전시켜 나갈 계획이다. 

