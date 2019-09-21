# 웹 애플리케이션 서버
## 진행 방법

## 우아한테크코스 코드리뷰

### 1단계 
    * GET으로 페이지 요청을 했을 때 그 헤더를 읽는다.
    * 그 읽은 파일의 Path를 찾아서 읽는다.
    * 읽은 html을 클라이언트에 응답한다.

### 2단계 
    * 회원가입 할 때의 데이터를 ? 기준으로 spilit 한다.
    * URL 에서 이름, 값을 추출해 Map에 담는다.
    * 담은 Map의 Data를 바탕으로 Domain을 생성한다.  
    * 생성한 Domain을 DB에 Add한다.
    
### 3단계
    * /usr/form 에 있는 signup 요청을 GET -> Post로 변경한다.
    * Post에 대한 분기처리를 실행한다.
    * Response 로 200 OK가 아닌 3XX Redirect와 그 URL을 전달한다.