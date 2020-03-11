# docker-Yml

Ye! Everything is docker-compose.yml. docker-compose.yml Configuration. hahaha~~~!!!

base for alpine linux

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
docker pull alpine:3.11
docker pull debian:buster-slim
docker pull ubuntu:bionic
docker pull nginx:1.17.8-alpine
```
