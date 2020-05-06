README.md

1) gap 분석
  -. REST API 개념
  -. embedded Database ( ex. H2)
       => 
  -. github
  -. json

2) 과제 유형 2를 선택하게 된 배경
  -. 주어진 과제 1,2를 모두 확인하였으나
     과제 2가 요구사항들이 좀더 명확하게 정의 되어 있었음

3) 구현된 내용
  -. unit 테스트를 위한 콘솔 입력
      . 테스트 데이터를 통한 기본 기능 확인
  -. 카드결제, 결제 취소, 결제 정보 조회 프로세스       
      . 결제, 결제 취소의 관리번호(Unique ID는 각각 생성되도록 구현) / payment.java , calcel.java
	  . 조회용 모듈 inquiry.java
	  . 암호화 모듈( EncyptionUtil.java)
	      => AES를 통한 암호화는 구현하였으나, 시간관계상 복호화는 구현하지 못함
  -. 데이터 저장,처리용 String 모듈 ( DataDef.java)		  
  -. 데이터 유형에 따른 validation 모듈 ( validationCheck.java ) 
  

4) 구현되지 못한 내용
  -. DB를 이용한 데이터 연계
  -. 트랜젝션 데이터 괸리 부분
  -. MultiThread 환경에대한 대비
      semaphore(세마포어)를 구현하여 카드, 결제건에 대한 제어를 생각하였으나
      구현하지 못함	  
  -. 추가 구현 과제
  -. json format 입출력에 대한 대응

5) 아쉬운점
  -. 주어진 과제를 모두 해내지 못한 부분
  -. json 입출력에 대한 인터페이스 모듈을 구현하지 못함.
       더 많은 테스트를 해볼수 있는 기회를 잃어 버림

6) 실행 방법
  -. eclipse에서 Run을 수행한 후 console 입력을 통해 테스트 수행
  
    1: 카드결제
    2: 결제취소
    3: 결제정보조회
    8: String 변환
    9: 단위 테스트 종료