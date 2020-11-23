# atlassians.yml
基于 docker-compose.yml 的 Atlassians 全家桶

先拉取基础镜像，试验用的镜像和版本如下：
```
docker pull atlassian/bitbucket-server:7.6.1
docker pull atlassian/confluence-server:7.8.1
docker pull atlassian/jira-software:8.0.2
```

## 启动 atlassians
编译镜像，这步只需执行一次。
```
docker-compose up -bulid
```

以后只需执行下面命令来启动了。
```
docker-compose up -d
```

停止
```
docker-compose stop
```

启动后优先访问 jira 来配置 jira 的账号，然后 confluence 和 bitbucket 就可以直接关联过去实现这 3 个系统的统一登录了
