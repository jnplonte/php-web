# LARAVEL WEB
[![license](https://img.shields.io/github/license/mashape/apistatus.svg)]()

## Version
**v1.0.0**

## Dependencies
* php [https://php.net/](https://php.net/)
* laravel: [https://laravel.com/](https://laravel.com/)
* docker: [https://www.docker.com/](https://www.docker.com/)


## start docker
* build docker image by running `docker-compose build`
* running docker image by running `docker-compose up`
* start docker image by running `docker-compose start`

* check docker inforation by running `docker-compose ps`
* identify the docker inforation by running `docker inspect <docker-name>`


## stop docker
* stop docker image by running `docker-compose stop`
* killing docker image by running `docker-compose kill`
* removing docker image by running `docker-compose rm`
* down docker image by running `docker-compose down --volumes`


## explore docker filesystem
* `docker run -t -i laravel-web_laravel_1 /bin/bash`


## check docker information
* `docker inspect laravel-web_laravel_1 | grep "IPAddress"`
* `docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' laravel-web_laravel_1`
