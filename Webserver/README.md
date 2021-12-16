# Web Server

## Nginx

* <https://www.nginx.com/blog/5-performance-tips-for-node-js-applications/>
* <https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/>

## How to handle large traffic?

* [Naver](https://d2.naver.com/helloworld/6070967)
  * 로드 밸런서를 사용하는 일반적인 3계층(3-Tier) 분산 처리 모델
    * Load Balencer
    * Web Server
    * Web Application Service (WAS)
    * Database
  * Naver's Style
    * Global CDN (GCDN)
      * 공통적으로 호출되는 리소스(JS, CSS, IMG)의 부하 분산을 위해 GCDN을 사용한다.
      * GSLB
    * Server Side Inclusion
      * 서버에 있는 특정 파일을 읽어오거나 특정 쿠키 유무의 판별 등 간단한 기능을 실행할 수 있다.
    * Apache Custom Module
      * [Apache Portable Runtime](https://apr.apache.org/)
    * Microservice
      * circuit breaker
        * 외부 서비스의 장애로 인한 연쇄적 장애 전파를 막기 위해 자동으로 외부 서비스와 연결을 차단 및 복구하는 역할을 한다. 
      * service discovery
        * 동적으로 생성, 삭제되는 서버 인스턴스에 대한 IP 주소와 포트를 자동으로 찾아 설정할 수 있게 하는 기능이다.

* [Load Balencer](https://d2.naver.com/helloworld/605418)
* [HAProxy](https://d2.naver.com/helloworld/284659)
