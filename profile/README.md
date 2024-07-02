![header](https://capsule-render.vercel.app/api?type=venom&color=gradient&customColorList=6&animation=fadeIn&fontColor=E3DAFF&height=300&section=header&text=티끌%20모의%20태산&fontSize=90) 


# 프로젝트 소개 📢
<br/>

 
  ### <img src="https://github.com/1-screeningHumanity/.github/assets/141290308/fbea4842-c339-4b99-977a-bee4742e09ba" alt="tmt" width="25" height="25"> 티끌 모의 태산 
  - 서비스 URL : https://screeninghumanity.store/
  <br/>
  
  ### 🗓️ 프로젝트 기간  
  - 2024.04.18 ~ 2024.07.04
  - 총 **`2024.02.21~2024.04.14`**

  <br />

 ### 📌 서비스 소개 
  > **티끌모의태산은?** 
  - **시니어를 대상**으로 한 **주식모의투자서비스** 티끌모의태산 입니다.
  - 주식을 입문하는 시니어분들의 시행착오를 줄여주고자 `간편한UI`, `음성인식`, `매매 가이드라인` 기능을 제공하였습니다.
  - `랭킹`, `퀴즈` 등을 추가하여 사용자의 즐거움 요소를 추가하였습니다. 
  - 실전투자에 입문하기 전 모의투자를 통해 **주식투자의 길잡이**가 되어드립니다.

  <br/>
  
  

<br/>

# 목차 📚
<br/>

 ### [1. 기능](#기능)<br/>
 ### [2. 화면소개](#화면소개)<br/>
 ### [3. 기술스택](#기술스택)<br/>
 ### [4. 팀원소개](#팀원소개)<br/><br/>

 
 # 기능

### 1.  회원가입 / 로그인
- 시니어층을 대상하기 떄문에 전화번호, 이름 , 비밀번호로 가입 가능합니다
- 닉네임의 경우 랜덤으로 설정 가능하게 헀습니다.

  <img src="https://github.com/1-screeningHumanity/TMT-FE/assets/141290308/e53ae3ce-a022-44e8-b5ff-5538a44335bf" alt="쉬운 간편 로그인 기능" width="300" />

<hr/>

### 2. 주식 / 회원 검색 
- 시니어를 위한 음성인식 기능 추가
- Elastic Stack 을 추가하여 빠른 응답, 필터링을 활용한 유연한 검색 엔진
- 기존 MySql 쿼리를 이용한 query 461ms -> 57ms

<img src="https://github.com/1-screeningHumanity/TMT-FE/assets/141290308/d9536625-7156-4a05-ac0b-3dfb8ce56ec9" alt="쉬운 간편 로그인 기능" width="300" />
<hr/>

### 3. 실시간 차트, 종목 토론방 제공
- 한국투자증권 API 를 사용하여 실시간 차트를 제공하여 실시간 가격을 제공
- SSE 방식을 선택하여 실시간 데이터 수신 
  

<img src="https://github.com/1-screeningHumanity/TMT-FE/assets/141290308/54a4dde5-8980-404c-9965-454a98891cad" alt="쉬운 간편 로그인 기능" width="300" />
<hr/>

### 4. 매매 체결, 알림 발생
- 구매를 원하는 가격과 매매 가격이 같으면 체결
- FCM을 이용한 알림 토큰 발생 및 전송 
- 카프카를 통한 예약 매수 체결과 연동된 기기 알림 서비스

<hr/>


### 5. 퀴즈 제공
- 주식 입문자를 위해 퀴즈를 제공하여 지식을 늘리고 즐거움 요소를 더 함

<img src="https://github.com/1-screeningHumanity/TMT-FE/assets/141290308/25a2d7d8-eec1-4a78-8a33-18ed66176c56" alt="퀴즈" width="300" />
<hr/>

### 6. 랭킹 서비스 제공
- 스프링 배치를 이용하여 데이터를 집계
- 자산, 수익률 (일, 주, 월) 랭킹을 확인 가능 
<img src="https://github.com/1-screeningHumanity/TMT-FE/assets/141290308/d39b4a72-f67f-4fb4-9eaa-039ca2c4260c" alt="랭킹" width="300" />



 # 화면소개
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/06152507-a414-418f-a219-7f48a781dcbe" alt="메인페이지1" />
       <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/6fbd4b02-4851-4558-9fc1-6a8e3a67107e" alt="메인페이지2"/>
       <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/b2ae64a8-8d83-4b9a-a5da-9eb19f7260b6" alt="로딩페이지"/>
       <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/a49d4782-58bb-407c-a322-3c4782b905ac" alt="not-found페이지"/>
         
   </tr>
   <tr>
     <td colspan="2" align="center">메인페이지</td>
     <td align="center">로딩페이지</td>
     <td align="center">not-found 페이지</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/0368e2fa-251a-41a8-8060-aec234a8ecf5" alt="로그인페이지" />
       <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/3a679fdb-0530-4b6d-9428-03138d5fe26a" alt="회원가입페이지"/>
       <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/1095d1a6-e2b5-46b9-bc72-f109ac581837" alt="비밀번호 찾기 페이지"/>
         
   </tr>
   <tr>
     <td align="center">로그인</td>
     <td align="center">회원가입</td>
     <td align="center">비밀번호찾기</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/e37ae001-07eb-46ea-8002-f4c3a56104aa" alt="카테고리1" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/68285285/8d34bb48-9959-4afb-a351-c7b88f842cbd" alt="카테고리2"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/68285285/5949d063-e680-4210-8ee9-f285db27adb3" alt="카테고리3"/>
   </tr>
   

   <tr>
     <td colspan="3" align="center">카테고리</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/bb83764a-5438-4293-9a78-c4cb8dcdcfb9" alt="검색페이지1" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/939372d7-df9b-4f74-8aaf-37c14094d78b" alt="검색페이지2"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/79a09dd2-86b4-447c-b5a3-9d40a2ebfc4c" alt="알림페이지"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/267ba66a-3560-48c0-ac6e-c3359c16d4e1" alt="급등/급락주페이지"/>
   </tr>
   <tr>
     <td colspan="2" align="center">검색</td>
     <td align="center">알림</td>
     <td align="center">급등/급락주</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/68285285/47187460-5de6-473e-8a77-ed482f4343c2" alt="카테고리1" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/712bca12-004e-4bb2-84ef-b0a58ef0ec33" alt="카테고리2"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/fab3a4d5-cc78-490d-a43a-1d27c6cdf86c" alt="카테고리3"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/0708d619-b6cf-4319-af79-fd032c43cbe7" alt="카테고리3"/>
   </tr>
   <tr>
     <td colspan="4" align="center">종목 상세</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/a5305ce8-c10a-4c63-bc74-f2c2efe91b6d" alt="랭킹페이지1" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/a54467ad-ca62-4e40-98c6-ae2f093391ed" alt="랭킹페이지2"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/7e2ff372-972b-4e49-a84e-a34160913c3a" alt="마이페이지1"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/d0bc324a-3796-472e-bd0e-3e49293b93b2" alt="마이페이지2"/>
   </tr>
   <tr>
     <td colspan="2" align="center">랭킹</td>
     <td colspan="2" align="center">마이페이지</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/1a44f765-169f-4ed0-8771-298442b3074b" alt="타인프로필(구독전)" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/4b1319b9-06a2-4a3b-a381-c8cbefc825a2" alt="타인프로필(구독후)"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/0f88381b-a3a2-49dd-88a6-0f710791ce96" alt="구독하기페이지"/>
   </tr>
   <tr>
     <td  align="center">타인프로필(구독전)</td>
     <td  align="center">타인프로필(구독후)</td>
     <td  align="center">구독하기</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/61f42629-4e19-46da-943d-414f1d85f9c7" alt="매수/매도목록페이지" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/e65b97b5-8477-4344-b07b-0c2f6c219b13" alt="예약매수/매도목록페이지"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/94597a0a-c295-48a8-816c-613c31cbc163" alt="구독자목록페이지"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/ac1ec3fc-d8fb-4731-92dc-771fdbd95db4" alt="나를구독한사람목록페이지"/>
   </tr>
   <tr>
     <td align="center">매수/매도목록</td>
     <td align="center">예약매수/매도목록</td>
     <td align="center">구독자목록</td>
     <td align="center">나를구독한사람목록</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/cef35b84-0e12-47cd-aa43-0ec27a4ff61e" alt="즐겨찾기목록페이지" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/d5eb5525-d6cf-4dbf-9f77-38fde4327bf5" alt="결제내역페이지"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/02997865-2c7c-45ae-ad96-c2b4c5a8cf09" alt="비밀번호변경페이지"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/c271c92f-b2b3-4adf-90fd-0aee16472203" alt="비밀번호변경완료페이지"/>
   </tr>
   <tr>
     <td align="center">즐겨찾기목록</td>
     <td align="center">결제내역</td>
     <td align="center">비밀번호변경</td>
     <td align="center">비밀번호변경완료</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/f17cf834-0f9e-482f-aeb0-d4f43305b857" alt="결제비밀번호변경페이지" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/6ac7973a-297c-4111-98b8-1961ddfd15ab" alt="결제비밀번호확인페이지"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/90653039-3ddf-4ff9-af8c-9868a278e4cb" alt="결제비밀번호변경완료페이지"/>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/85f9f281-4614-43c0-a0fd-3809ccff54bd" alt="닉네임변경페이지"/>
   </tr>
   <tr>
     <td align="center">결제비밀번호변경</td>
     <td align="center">결제비밀번호확인</td>
     <td align="center">결제비밀번호변경완료</td>
     <td align="center">닉네임변경</td>
   </tr>
 </table>
 <table>
   <tr>
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/3e647db1-6946-45c8-ad8a-34b5acd18278" alt="결제페이지" />
     <td width="300" bgcolor=#FFFFFF><img src="https://github.com/1-screeningHumanity/.github/assets/141290308/f11a9db1-0f8f-4e99-b070-96fdeda45330" alt="금액교환하기페이지"/>
   </tr>
   <tr>
     <td align="center">결제페이지</td>
     <td align="center">금액교환하기</td>
   </tr>
 </table>

 
 # 기술스택
![image](https://github.com/1-screeningHumanity/.github/assets/141290308/9d89ada8-3158-4485-a72d-a7fcb1d2964f)

# 팀원 소개
 <table>
<tbody>
<tr>
<td align="center"><a href="https://github.com/jmlee119"><img src="https://github.com/hyobin0726/hyobin0726/assets/140376727/8376e174-415d-40c0-abcc-e9cd8d71cccd"width="100px;" alt=""/><br /><sub><b>FE | 팀장 : 이지민</b></sub></a><br /></td>
<td align="center"><a href="https://github.com/hyobin0726"><img src="https://github.com/hyobin0726/hyobin0726/assets/140376727/65855eee-eb9b-42c2-bda3-615c59cb6450"width="100px;" alt=""/><br /><sub><b>FE | 팀원 : 박효빈</b></sub></a><br /></td>
<tr/>
<td align="center"><sub>회원가입, 로그인, 마이페이지, 장바구니, 주문, 배송지</sub></td>
<td align="center"><sub>카테고리, 홈, 상품리스트, 상품상세, 리뷰, 최근 본 상품</sub></td>
</tr>
</tbody>
</table>

