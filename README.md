## Services & Versions

* nginx
* laravel 8
* php 7.4
* node 14
* mysql 5.7


## Build

```
docker-compose up --build

docker-compose up -d

docker-compose up -d --build

docker-compose build && docker-compose up -d


docker-compose down
```

## Docker Commands
```
show system usage
==================

docker system df

PS E:\Projects\0.personal\docker_cmp> docker system df
TYPE            TOTAL     ACTIVE    SIZE      RECLAIMABLE
Images          6         5         1.699GB   67.11MB (3%)
Containers      5         5         19.1MB    0B (0%)
Local Volumes   2         1         433.2MB   210.3MB (48%)
Build Cache     160       0         8.974GB   8.974GB

```

## Run
1. http://cmpapi.localhost/
2. http://cmp.localhost:3000/
   1. cd .\app-frontend\
      1. npm start
         1. custom cause default WSL2 doesn't support changes npm start in windows but support in linux