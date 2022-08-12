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





------------------------------------------
------------------------------------------
# Running Postgres via Docker

**To check docker install properly**

> docker

**To run a posgres container**

> docker run --name postgres-nest -p 5432:5432 POSTGRES_PASSWORD=rajesh -d postgres

"docker" is docker

"run" means I want to run a container

"--name postgres-nest" means how I want to name my container

"-p 5432:5432" means container's port is :5432 and I want to host/map it to my current machine port 5432:

"-e POSTGRES_PASSWORD=rajesh" -e means environment variable. I wantto tell the docker container of the postgres to set the POSTGRES_PASSWORD to 'rajesh'

"-d" means detached mode, that means docker will running after closingthe cli

"postgres" this is the actual container name stored on the cloud 


**To ensure the container is running**

> docker container ls

***To stop a container*

> docker container stop <container-name>

> docker container stop postgres-nest


