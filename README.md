app.js file
console.log('Hello Docker');

Dockerfile file
FROM node:alpine
COPY . /app
WORKDIR /app
CMD node app.js

Command
node app.js  

Command
docker build -t hello-docker .  
docker image ls
docker run hello-docker

https://hub.docker.com/
Create Repository
Name:firstname [repository name]


Command
docker tag hello-docker abusayediit/firstimage:hello-docker
docker push abusayediit/firstimage:hello-docker

https://labs.play-with-docker.com/
docker push abusayediit/firstimage:hello-docker
docker run abusayediit/firstimage:hello-docker    
