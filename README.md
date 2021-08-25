npm init -y
touch index.js
touch Dockerfile
touch README.md
npm install express

docker -v
Docker version 20.10.7, build f0df350

docker-compose -v
docker-compose version 1.29.2, build 5becea4c

touch .dockerignore
touch .gitgnore

docker build -t maquina/dockernode .
docker run -p 3000:3000 -d maquina/dockernode
docker ps

docker ps
CONTAINER ID   IMAGE                COMMAND                  CREATED          STATUS          PORTS                                       NAMES
1ba5a18a7f53   maquina/dockernode   "docker-entrypoint.s…"   26 seconds ago   Up 24 seconds   0.0.0.0:3000->3000/tcp, :::3000->3000/tcp   charming_jang


npm install nodemon
docker build -t maquina/dockernode .
docker run -p 3000:3000 -d maquina/dockernode
docker-compose up


## parar pois já estava sendo utilizada
docker ps
docker stop 1ba5a18a7f53

docker-compose up
docker build -t maquina/dockernode .