# spring-cloud-config

- spring-cloud-config-server 프로젝트

- config reference repository : https://github.com/jjunhoo/spring-cloud-config-repository

> 사용 방법

1. Spring-Boot Application 실행
2. [GET] localhost:9090/myapp/dev 또는 localhost:9090/myapp/prod 호출 및 config - response 확인
   - https://github.com/jjunhoo/spring-cloud-config-repository 내 yml 파일명을 resource 로 입력 및 호출
   - 예 : myapp-dev.yml
     - [GET] localhost:9090/myapp/dev
   - 예 : myapp-prod.yml
     - [GET] localhost:9090/myapp/prod
