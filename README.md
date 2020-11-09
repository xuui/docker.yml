# docker.yml

Ye! Everything is docker-compose.yml. hahaha~~~!!!

The's docker-compose.yml Configuration.

Base for alpine linux

```
$ docker ps // 查看所有正在运行容器
$ docker stop containerId // containerId 是容器的ID

$ docker ps -a // 查看所有容器
$ docker ps -a -q // 查看所有容器ID

$ docker stop $(docker ps -a -q) // stop停止所有容器
$ docker rm $(docker ps -a -q) // remove删除所有容器
```

## Pull Docker Base image:
```
docker pull alpine:3.12
docker pull debian:buster-slim
docker pull ubuntu:bionic   #18.04
docker pull ubuntu:focal    #20.04
docker pull nginx:1.19.1-alpine
docker pull php:7.3.22-fpm-alpine3.12
docker pull php:7.4.10-fpm-alpine3.12

```

## Dockerfile Mirrors:
Alpine:
```
FROM alpine:3.12
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.ustc.edu.cn/g' /etc/apk/repositories;
```
Debian:
```
FROM debian:buster-slim
RUN sed -i 's/deb.debian.org/mirrors.ustc.edu.cn/g' /etc/apt/sources.list;
```
Ubuntu:
```
FROM ubuntu:focal
sudo sed -i 's/archive.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list
```

## Docker compose.yml 映射
如果 docker-compose.yml 里面的 volumes: 组所映射的文件路径不纯在。那就用 docke exec -it <容器ID> /bin/bash 进去容器，自己找的位置来处理。

