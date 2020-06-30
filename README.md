# Docker Workshop

## get started

To start the project:

`npm install`

`node server.js`

Navigate to localhost:8000

## useful commands:

build a docker image, give it the tag

`docker build --tag hello-docker-image:1 .`

list your docker images

`docker images`

build and start a docker container with the name hello-docker-container, using the image hello-docker-image:1. Run in a detached state.

`docker run --name hello-docker-container -d hello-docker-image:1`

list your running docker containers

`docker container ls`

list all your docker containers (running and stopped).

`docker container ls -a`

stop a docker container immediately (in 0 second)

`docker stop -t 0 hello-docker-container`

start a docker container

`docker start hello-docker-container`

remove a docker container

`docker rm hello-docker-container`

build and start a docker container with the name hello-docker-container, using thing image hello-docker-image:1. Run in a detached state. Also deal with port bindings!

`docker run --name hello-docker-container -d -p 8080:1000 hello-docker-image:1`
