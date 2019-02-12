# docker-postgres

## MOST UPDATED

````text
 docker run --name pg-docker -e POSTGRES_PASSWORD=123456 -d -v datadir:/var/lib/postgresql/data postgres
 docker-compose -f docker-compose.yml up
````

## COMMANDS

````text
* List/Stop/Remove running container:
$ docker container ls
$ docker stop <container>
$ docker rm <container>
$ docker system prune
````

## OTHERS

````
 docker run --name 11.1 -e POSTGRES_PASSWORD=123456 -d postgres
 docker run --name 11.1 -e POSTGRES_PASSWORD=123456 -d -v datadir:/var/lib/postgresql/data postgres

WORKING
 docker run --name pg-docker -d -p 5432:5432 postgres
 docker-compose -f docker-compose.yml up


 docker run --name some-postgres -v /my/own/datadir:/var/lib/postgresql/data -d postgres:tag
 docker run --name 11.1 -v /Temp/datadir:/var/lib/postgresql/data -d postgres
 docker run --name 11.1 -v c:\Git\docker.postgres\datadir:/var/lib/postgresql/data -d postgres

 docker pull postgres
 docker run --rm --name pg-docker -e POSTGRES_PASSWORD=123456 -d -p 5432:5432 -v datadir:/var/lib/postgresql/data  postgres
 docker run --name pg-docker -d -p 5432:5432 postgres
````

## REFERENCES

* [PostgreSQL](https://hub.docker.com/_/postgres)
* [Don’t install Postgres. Docker pull Postgres](https://hackernoon.com/dont-install-postgres-docker-pull-postgres-bee20e200198)
* [Docker for Windows : Startup Errors](https://rominirani.com/docker-for-windows-startup-errors-fb5903431eda)
* [How To Remove Docker Images, Containers, and Volumes](https://www.digitalocean.com/community/tutorials/how-to-remove-docker-images-containers-and-volumes)