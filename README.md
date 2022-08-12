# Docker 
### Download Docker
https://www.docker.com/products/docker-desktop/

### CLI

> docker --help

> docker pull postgres:alpine

### [postgres docs](https://hub.docker.com/_/postgres/)

> docker images 

> docker run --name postgres-0 -e POSTGRES_PASSWORD=password -d -p5432:5432 postgres:alpine

> docker ps

> docker exec -it postgres-0 bash

**Now you are in actual container**
> pwd

> ls

>  psql --help

> psql -U postgres   // -U for username

**Now you are inside of postgres**

**To see the actual user that you have inside postgres**

> \du

**Create a Database**

> create database test;

**To view Database**

> \l

**To connect database "test" as user "postgres"**

> \c test

Referrence from [here](https://www.youtube.com/watch?v=aHbE3pTyG-Q)


