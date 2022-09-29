문서정보 : 2022.09.29.~30. 작성, 작성자 [@SAgiKPJH](https://github.com/SAgiKPJH)

# Docker Infinite Mario Bros

- Docker로 Infinite Mario Bros 게임을 돌려본다.

<br>

## 차례

- [x] [1. Infinite Mario Bros Docker 설치](https://github.com/SagiK-Repository/Docker_Playground/blob/main/Infinite%20Mario%20Bros.md)
- [x] [2. Infinite Mario Bros Image 실행](https://github.com/SagiK-Repository/Docker_Playground/blob/main/Infinite%20Mario%20Bros.md#2-infinite-mario-bros-image-%EC%8B%A4%ED%96%89)

<br>

## 1. Infinite Mario Bros Docker 설치

- Docker Hub에 supermario라 검색하면 다음과 같은 [docker사이트](https://hub.docker.com/r/pengbai/docker-supermario)가 나온다.
  - https://hub.docker.com/r/pengbai/docker-supermario
- Docker Pull Command를 통해 Docker pengbai/docker-supermario(646MB)를 Pull 한다.
  ```bash
  docker pull pengbai/docker-supermario
  ```  
  ![image](https://user-images.githubusercontent.com/66783849/193149838-eaf3d1d0-0624-4671-abc7-098c541d1ec5.png)

  
<br>


## 2. Infinite Mario Bros Image 실행

- 설치된 이미지를 컨테이너로 만들어 돌린다.
  ```bash
  docker run -d -p 8080:8080 pengbai/docker-supermario
  ```  
  ![image](https://user-images.githubusercontent.com/66783849/193149955-112f7e20-89ec-4e52-9f7e-4826b64f37e5.png)
- 웹 브라우저를 통해 다음 사이트로 이동한다.
  - http://localhost:8080/  
  ![image](https://user-images.githubusercontent.com/66783849/193150014-ae319d9c-12f1-48ab-9d92-b441c5b57a7d.png)  
  ![image](https://user-images.githubusercontent.com/66783849/193150147-b9652c41-c092-4354-b91e-afad6f8bbcb4.png)

