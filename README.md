#

> docker compose开发环境编排,mongodb, mysql, nginx, php, redis

## 依赖环境

- Docker [install](https://www.docker.com/community-edition#/download)
- Docker compose [install](https://docs.docker.com/compose/install/)

## 安装
```shell
$ git clone https://github.com/AugusLarry/docker-mmnpr.git
$ cd docker-mmnpr
$ docker-comopse up -d
```

## 目录说明
```shell
|- docker-mmnpr
    |- mongo
        |- data mongodb数据库存储目录
    |- mysql
        |- data mysql数据库存储目录
        |- etc
            |- my.cnf mysql配置文件
    |- nginx
        |- etc
            |- conf.d 站点配置文件
            |- nginx.conf nginx基础配置文件
        |- html
    |- php
        |- etc
            |- php.ini php配置文件
        |- Dockerfile php Dockerfile
    |- redis
        |- data redis data存储目录
    |- docker-compose.yml docker compose文件
```

## 其他说明
- php默认开启xdebug,redis,mysqli,pdo_mysql,gd,openssl,SimpleXml,mcrypt,zlib,curl,bz2,ftp等等...