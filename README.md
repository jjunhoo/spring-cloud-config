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
   - localhost:9090/myapp/dev 응답 
   ````java
   {
      "name": "myapp",
      "profiles": [
         "dev"
      ],
      "label": null,
      "version": "7c5e3fbc3accf27538cc5cd85fe3e3e0f16f955d",
      "state": null,
      "propertySources": [
         {
            "name": "https://github.com/jjunhoo/spring-cloud-config-repository/myapp-dev.yml",
            "source": {
               "junho.profile": "DEV Environment",
               "junho.text": "DEV Config"
            }
         }   
      ]
   }

   ````
