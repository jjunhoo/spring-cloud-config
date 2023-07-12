# spring-cloud-config

- spring-cloud-config-server 프로젝트

- config reference repository : https://github.com/jjunhoo/spring-cloud-config-repository

> 사용 방법

1. Spring-Boot Application 실행
2. end-point 호출 및 config 확인
   - https://github.com/jjunhoo/spring-cloud-config-repository 내 yml 파일명을 resource 로 입력하여 호출
   - 예 : myapp-dev.yml
     - [GET] localhost:9090/myapp/dev
   - 예 : myapp-prod.yml
     - [GET] localhost:9090/myapp/prod
