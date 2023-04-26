# 🍝 HongEat-Deploy

홍대 근처 맛집 한줄 리뷰 서비스 HongEat 배포 레포지토리입니다

<br/>

## 🏛 Architecture Diagram
![hongeat](https://user-images.githubusercontent.com/62806067/233274477-7980b38e-e7c8-42c7-851c-8204d29ad428.png)


<br/>

## 💻 배포 과정

1. deploy/main 브랜치로의 push를 감지하면 Github Actions 실행
2. deploy.sh 를 통해 리모트 서버의 docker, docker-compsoe 설치 여부를 확인 및 설치
3. ssh 를 통해 리모트 서버의 docker-compose 실행

<br/>

## :hammer: 환경 변수

Settings -> Secrets -> Actions 탭에서
EC2 서버 ip, SSH key, Hostname, .env 등의 환경 변수를 지정합니다

<br/>


