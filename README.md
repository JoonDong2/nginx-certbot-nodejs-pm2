# 주요 기능
1. docker-compose.yml 파일에 입력한 도메인의 SSL 인증서 자동 발급 및 갱신  
2. `sudo docker-compose up -d` 명령어를 실행하는 즉시 docker-compose.yml 파일에 입력된 도메인으로 HTTPS 접속하면 pm2/src/app.js 프로그램의 결과를 받을 수 있다.  
  
# 기본 사용법
1. 호스트 80번 포트와 443번 포트 열기  
2. docker, docker-compose 설치  
3. docker-compose.yml 파일에 이메일 입력  
4. conf.d/nginx.conf 파일에 도메인 입력  
5. pm2 폴더에 있는 json 파일의 주석 제거  
6. pm2/src/app.js 작성  
7. 프로젝트의 루트 경로에서 `sudo docker-compose up -d` 명령어 실행  
  
# 상세 설명
http://joondong.tistoy.com/164  
  
# 참조
[staticfloat/docker-nginx-certbot](https://github.com/staticfloat/docker-nginx-certbot)  
[keymetrics/docker-pm2](https://github.com/keymetrics/docker-pm2)  
동빈나님의 [도커(Docker) 활용 및 배포 자동화 실전 초급](https://www.youtube.com/watch?v=HbKCxBFT2wk&list=PLRx0vPvlEmdChjc6N3JnLaX-Gihh5pHcx)  
  
# 라이센스
복붙한 거라 라이센스라고 할 것까지도 없지만... MIT  