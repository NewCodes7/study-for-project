### API (AWS 포스팅 참고)
- API: Application Programming Interface
  - Application: 소프트웨어를 의미함.
  - Interface: 두 애플리케이션 간의 서비스 계약
    - 계약: 요청과 응답을 사용하여 두 애플리케이션이 서로 통신하는 방법을 정의함.
- 의미: 정의 및 프로토콜 집합을 사용하여 두 소프트웨어 구성 요소가 서로 통신할 수 있게 하는 메커니즘
- 종류
  - SOAP API 
  - RPC API
  - Websocket API
    - 의미: JSON 객체를 사용하여 데이터를 전달하는 최신 웹 API
    - 특징: 클라이언트 앱과 서버 간의 양방향 통신을 지원
      - 서버가 연결된 클라이언트에 콜백 메시지를 전송할 수 있어 REST API보다 효율적
  - REST API
    - REST(Representational State Transfer): 소프트웨어 프로그램 아키텍처의 한 형식
      - 의미: 클라이언트가 서버 데이터에 액세스하는 데 사용할 수 있는 GET, PUT, DELETE 등의 함수 집합을 정의함.
    - 클라이언트와 서버는 HTTP를 사용하여 데이터를 교환함.

### REST
- 의미: 자원을 이름으로 구분하여 해당 자원의 상태를 주고 받는 모든 것
  - 월드 와이드 웹 (WWW) 과 같은 분산 하이퍼미디어 시스템을 위한 소프트웨어 개발 아키텍처의 한 형식
  - 웹의 기존 기술과 HTTP 프로토콜을 그대로 활용하기 때문에 웹의 장점을 최대한 활용할 수 있는 아키텍처 스타일
- 구성
  - 자원
    - Resource
    - 모든 자원에는 id가 있고, 이 자원은 서버에 존재함.
    - 자원을 구별하는 ID는 /orders/order_id/1 와 같은 HTTP URI
  - 행위 (프론트 성격)
    - Verb
    - Http 프로토콜의 Method를 사용함.
    - HTTP 프로토콜은 GET, POST, PUT, DELETE와 같은 메서드를 제공함.
  - 표현 (백 성격)
    - Representaion of Resource
    - 클라이언트가 자원에 대한 조작을 요청하면, 서버는 이에 적절한 응답을 전송함.
    - 하나의 자원은 JSON, XML, TEXT, RSS 등의 여러 형태로 표현 가능함.
    - 현재는 JSON으로 주고 받는 것이 대부분.

- HTTP(HyperText Transfer Protocol): 웹에서 클라이언트와 서버 간에 이루어지는 요청/응답 프로토콜
- URI(Uniform Resource Identifier): 웹 서버가 자원을 고유하게 식별할 수 있도록 하는 것
  - URL: 특정 서버의 한 자원에 대해 구체적인 위치 서술
  - URN: 자원이 어디에 있든 찾을 수 있는 방식 

- 스프링부트: 스프링(프레임워크) + 톰캣(서버) + 여러 편의 기능

- Servlet: 서버에서 웹페이지를 동적으로 생성하거나 데이터 처리를 수행하기 위해 자바로 작성된 프로그램
  - 자바 코드 안에 html 태그가 삽입됨.
  - 자바 코드 작성이 편리함.
- JSP(Java Server Pages): 자바 
  - html 안에 자바 코드가 작성됨.
  - Html 태그 사용이 용이함.
  - JSP가 실행되면 servlet으로 변환됨.