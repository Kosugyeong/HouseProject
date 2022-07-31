# HouseProject
JSP Model 2를 이용한 부동산 매물 관리 웹사이트입니다. 

## 구현 기능

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

