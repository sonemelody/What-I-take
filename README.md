# What I Take

## 개인 사진전 사이트📸

### 1. Description
내가 직접 찍은 사진을 전시하는 갤러리  
게시판을 통해 사이트 방문객의 피드백 가능  
<br/>  
  
### 2. Use Case Diagram
![image01](https://github.com/sonemelody/What-I-take/assets/49124725/3c5d5a70-238c-4835-9960-b89f9eecb21b)
<br/>  

  
### 3. Develop Language
- Frond-end: Express.js
- Back-end: Node.js + MongoDB
- UI: Bootstrap
<br/>  

### 4. Web Contents  
**1. Home**

- 상단 가장 좌측에 프로젝트 이름 표시
- Home, Exhibiton, Board 메뉴 표시
- Sign Up, Login 메뉴 표시

![image02](https://github.com/sonemelody/What-I-take/assets/49124725/cb0f3161-b728-464d-98a5-a07be625a314)<br/>   
<br/>  

**2. Sign Up**

- Username, Name, Email, Password, Password Confirm의 다섯 가지 항목
- Username은 로그인 시 사용되는 아이디
- 별표 표시된 항목은 필수 입력
- Password와 Password Confirm이 같아야만 회원가입 가능
- Submit 버튼으로 회원가입

![image04](https://github.com/sonemelody/What-I-take/assets/49124725/ded37f88-c7df-4861-89ef-6169d57afb9d)<br/>  
<br/>  

**3. Login**

- Username과 Password 입력하여 로그인
- 데이터베이스에 존재하는 Username으로만 로그인 가능
- 비밀번호가 틀리면 로그인 불가
- Submit 버튼으로 로그인
- 로그인 성공 시에만 상단 헤더에 My Account와 Logout 표시

![image05](https://github.com/sonemelody/What-I-take/assets/49124725/0f0ef332-a97e-48e8-8a89-b27381e0fedf)<br/>  
<br/>  

**4. Logout**

- 현재 로그인된 계정에서 로그아웃
<br/>  

**5. My Account**

- 사용자 정보 확인 페이지
- 회원가입 시 입력했던 Name과 Email 표시
- Edit 버튼으로 사용자 정보 수정 가능

![image06](https://github.com/sonemelody/What-I-take/assets/49124725/ebf19fec-7289-4920-a13b-4151eb723913)<br/>  
<br/>  


**6. Edit User**  

- 사용자 정보 수정 페이지
- 현재 사용 중인 비밀번호를 입력하고, 그 비밀번호가 일치해야만 정보 수정 가능
- UserName, Name, Email, Password를 새로 설정 가능
- Back 버튼을 누르면 다시 My Account 페이지로 돌아감
- Submit 버튼으로 수정 사항 저장


![image07](https://github.com/sonemelody/What-I-take/assets/49124725/79f8efa9-6ad4-4233-a306-afce03d1c322)<br/>  
<br/>  


**7. Exhibition**  

- 사진전 감상 페이지
- 슬라이드형 갤러리
- 하단 썸네일 클릭하여 원하는 사진으로 이동 가능
- 마우스 우클릭 및 사진 저장 금지

![image03](https://github.com/sonemelody/What-I-take/assets/49124725/1f0daf15-fd42-44cb-9404-daf83ce7e1d0)<br/>  
<br/>  


**8. Board**  

- 커뮤니티 및 피드백 게시판
- 게시물 번호, 게시물 제목, 조회수, 작성자, 작성 날짜 표시
- New 버튼으로 새 게시물 작성 가능, 로그인 시에만 버튼 등장
- 비로그인 상태에도 게시물 열람 가능
- 게시물 제목 옆 댓글 및 첨부파일 아이콘 표시
- 조회수가 50 넘는 경우 hot! 아이콘 표시
- Show에서 화면에 표시될 게시물의 개수를 5, 10, 20개로 설정 가능
- 한 화면에 표시된 게시물 개수보다 작성된 게시물이 많은 경우 페이지 이동 버튼 등장
- Search에서 게시물 검색 가능
- 검색 옵션은 제목+내용, 제목, 내용, 작성자로 총 네 가지
- 각 게시물의 author 누르면 해당 아이디가 작성한 게시물만 표시


![image08](https://github.com/sonemelody/What-I-take/assets/49124725/bb7f7b1c-f133-45b5-ba0b-1556b7da39ca)<br/>  
<br/>  

**9. New Post**  

- 게시물 작성 페이지
- Title과 Body 필수 작성
- Attachment의 파일 선택 버튼으로 파일 첨부 가능
- 비로그인 상태에도 게시물 열람 가능
- Back 버튼을 누르면 다시 Board 페이지로 돌아감
- Submit 버튼으로 게시물 등록


![image09](https://github.com/sonemelody/What-I-take/assets/49124725/6ffa7773-3f83-45ec-8644-7fa76fc83149)<br/>  
<br/>  

**10. Post View**  

- 작성된 게시물 확인 페이지
- 게시물 번호, 제목, 조회수, 작성자 표시
- 파일이 첨부된 경우 파일 이름과 크기 표시
- 이미지, 동영상 첨부 파일은 게시물에서 바로 확인 가능
- 첨부 파일 이름 클릭하여 다운로드 가능
- 게시물 작성 날짜, 수정 날짜 표시
- Back 버튼을 누르면 다시 Board 페이지로 돌아감
- Edit과 Submit 버튼은 자신이 작성한 게시물일 경우에만 표시
- Edit 버튼으로 게시물 수정 가능
- Delete 버튼으로 게시물 삭제


![image10](https://github.com/sonemelody/What-I-take/assets/49124725/66968df8-8653-4dfb-9dc8-6dc3ef320906)<br/>  
<br/>  

**11. Comments**  

- 각 게시물마다 댓글 작성 가능
- 로그인 상태에만 댓글 작성 폼 활성화
- Add Comment 버튼으로 댓글 등록 가능
- 각 댓글마다 작성자 아이디, 댓글 내용, 작성 날짜 표시
- reply 버튼으로 답글 작성 가능, 답글에 답글을 다는 것도 가능
- Back 버튼을 누르면 다시 Board 페이지로 돌아감
- Edit과 Delete 버튼은 자신이 작성한 댓글일 경우에만 표시
- Edit 버튼으로 댓글 수정 가능
- Delete 버튼으로 댓글 삭제
- 댓글이 지워진 경우 (Deleted Comment)라는 흔적 생성 -> 답글의 원본 댓글이 삭제되었을 경우, 답글이 허공에 남는 경우 방지 위함


![image10](https://github.com/sonemelody/What-I-take/assets/49124725/66968df8-8653-4dfb-9dc8-6dc3ef320906)<br/>  
<br/>  



### 5. Database Structure
홈페이지의 게시물 및 댓글, 첨부파일 그리고 사용자 정보를 관리하기 위해 사용한 mongoDB의 구조  
comments, counters, files, posts, users로 이루어져 있으며 각각 댓글 내용, 게시물 번호, 첨부 파일, 게시물 내용, 회원가입한 사용자 정보를 관리

![image14](https://github.com/sonemelody/What-I-take/assets/49124725/396072bd-d909-4a61-a889-c950cc085556)<br/>  
<br/>  


### 6. How to Execute

$ npm init --yes  
$ npm install nodemon  
$ npm install --save ejs express mongoose body-parser method-override passport passport-local multer box-node-sdk  

cmd 실행
-> 프로젝트 폴더가 존재하는 경로로 이동
-> nodemon 입력으로 localhost 실행
