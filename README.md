# Helping

주1회 3시간 진행하는 팀프로젝트로 PHP,Mysql,notepad를 사용하여 제작

팀장:박상우 팀원 : 김찬영 , 강재은

## 자세한 사항은 [최종보고서](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/commit/19236cc4d318d67ba16bfcc39468c792f896232f) 참조

### <1차 4/12> - Login.html(로그인) , Signup.html(회원가입) 기본틀 작성 , 아이콘 제작 , Main.html기본틀 제작
#
### <2차 4/19> - Login.html(로그인) , Signup.html(회원가입) 완성 , 아이콘 적용 , Main.html제작
#
### <3차 4/26> - 시험기간으로 인한 회의 미실시
#
### <4차 5/3>  - main.html을 로그인 전 후인 blogmain과 alogmain으로 분할 , User 데이터 베이스,매칭 데이터베이스 제작
#
### <5차 5/11>
### 강재은
#### -User.html, Umat.php, Vol.html, Vmat.php 업로드 완료현재 구인게시판 등록할 수 있으며 구직게시판 틀만 잡음(삭제)

### 박상우
#### -Signup.php와user.db연동하여 회원등록이 가능하게 제작완료

### 김찬영
#### -Guide.html(사이트소개) ,Vinfor.html(봉사현황),informch.html(정보수정), Vollookup.html(봉사활동 내역조회), informodlogin.html(내정보 비밀번호 입력), informod.html(내정보) 의 페이지 디자인 통합 및 수정
#
### <6차 5/17>

### 강재은
* notice.php, umat.php, vmat.php 회원 정보가 사용자, 봉사자에 따라 구인 및 구직게시판 띄워줌 
* umat vmat에 게시글 등록하면 notice.php로 돌아가게 했음
+ 다음주 목표
  + 구인구직 메뉴 클릭하면 notice.php로 갈수 있도록 변경해야됨
  + 세션 이용하여 현재 로그인되어있는 아이디 불러와 구인 구직 게시판 만들 수 있게 수정해야됨(다음주 umat.php vmat.php 수정함)

### 김찬영
* Vinfor.php 전체 회원수 출력 
* user.sql vincnt 테이블 추가 
* a/blogmain,signup 소스코드 수정
+ 다음 목표 
    + db 봉사활동 횟수 연동하여 Vinfor 에 출력, 등 미완성 페이지 작성

### 박상우
 * Login.php에서 함수를 제작하여 비밀번호동일여부와 아이디 중복여부를 판단하는 함수제작
 * logcheck.php아이디 중복여부를 판단하는 php 제작
 * Logcheck.php에서 세션을 적용하여 로그인 제작
 * Logtest.php에서 로그인된 사용자의 이름과 아이디 출력(test)
 * Logout.php에서 세션종료와 함께 로그아웃 실행

 + 다음 목표
    + 페이지 이동 최적화
#

### <7차 5/24> 임무변경 박상우,김찬영(작업량에 따른 2인팀 생성) ->매칭시스템 작성 // 강재은->메인화면 구성요소 작성

### 박상우,김찬영
 * 매칭시스템 코딩을 위해 데이터 베이스를 기존과 달리 외래키를 이용하여 제작
 * 사용자의정보-[user테이블](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/database/user.sql)/지원정보-[volapp테이블](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/database/volapp.sql)/봉사내용-[volcontents테이블](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/database/volcontents.sql)
 * 내가 생성한 봉사활동/내가 신청한 봉사활동 출력([mycreatevol.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/mycreatevol.php),[myappvol.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/myappvol.php))
 * 생성된 봉사의 제목 클릭시 get형식으로 정보 넘겨주어 출력하는 코드 작성

### 박상우(추가)
 * 테이블 출력을 위한 기본 css작성,상단 공백 제거를 위한 css작성 -내정보를 비밀번호를 입력해야만 들어갈 수 있도록 작성([informodlogin.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/informodlogin.php ))

### 강재은
 * 고객센터 페이지 제작,정보수정작성
#

### <8차 5/31>매칭시스템 마무리,최종 테스트 전 마지막 코드작성

### 박상우,김찬영
-지원하기 클릭시 volapp테이블 안에 봉사num과 지원자 아이디 등록하는 코드 작성([appvol.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/appvol.php ) ,[app_db.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/app_db.php ))
지원한 봉사활동을 수락할때 사용자가 선택할 수 있도록 라디오 버튼 생성, 수락하기 누를시 선택된 사람을 제외한 나머지 인원에게는 매칭실패를 알려줌([volunteers.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/volunteers.php),[choval.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/choval.php ))
매칭이 완료됨을 알리는 화면(봉사자의 정보를 사용자에게 보여주는 화면 ([matchingend_user.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/matchingend_user.php ))
선택된 봉사자는 마지막 확인버튼을 클릭하여 봉사활동에 지원한 모든 사용자들의 정보를 삭제([matchingend_vol.php](https://github.com/chanyoungkim1/HelpingProject_PHP-MYSQL/blob/main/matchingend_vol.php ))

강재은
-헤더파일 작성,주민번호->나이추출 알고리즘 작성
#

### <9차 6/7>최종 테스트
 * 고객센터 댓글시스템 오류발생(수정완료)
 * 매칭시스템 출력오류발생(수정완료)
 * 세션출력 헤더파일에 통합(추가완료)
 * 전체적인 헤더파일 링크수정(수정완료)
 * 완료된 봉사활동 출력버튼(삭제)
 * 매칭완료시 volcontents 테이블에 checka 값이 입력되지 않는현상(수정완료)
 * user테이블에서 주민번호 만으로 성별 나이값을 자동으로 입력(추가완료)
 * 소개,봉사현황 간단한 위치정리(수정완료)
 * 헬핑 설명서 작성(완료)
 * 헬핑 보고서 작성(완료)
