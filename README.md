This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).

Below you will find some information on how to perform common tasks.<br>


## How to Run React-App on Docker


-> Need to create a react-app on server by using following commands

$ sudo apt install npm

$ npm install -g create-react-app

$ npx create-react-app <app-name>(React-docker)
  
$ cd React-docker

-> after this we need to create a Dockerfile to build The app and ready for Run.This file already on Repo

## Now you need to build the project

$ docker build -t <tag-you need>  .

Docker image will be Built ypu can check with $ docker image ls

Now run the below command to run the react app on docker container

docker run -itd -v ${PWD}:/var/www -p 3000:3000 <image-name>
  
now check with server ip:3000 your app will be running 



