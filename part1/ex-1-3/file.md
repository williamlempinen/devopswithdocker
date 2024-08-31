```

`wlemp@DESKTOP-OO5ESTO  ~  docker ps                   
`CONTAINER ID   IMAGE                                      COMMAND                 CREATED              STATUS              PORTS     
`NAMES
`99fac31b588d   devopsdockeruh/simple-web-service:ubuntu   "/usr/src/app/server"   About a minute ago   Up About a minute             
`ex-1-3
`wlemp@DESKTOP-OO5ESTO  ~  docker stop 99
`99
`wlemp@DESKTOP-OO5ESTO  ~  docker container rm ex-1-3
`ex-1-3
`wlemp@DESKTOP-OO5ESTO  ~  docker run -d --name ex-1-3 devopsdockeruh/simple-web-service:ubuntu
`f28bf88fa3ff5f4bdd1118d66b0249f76711f4198b8a7fed38dad8dca676dfc4
wlemp@DESKTOP-OO5ESTO  ~  docker exec -it ex-1-3 bash                                          
`root@f28bf88fa3ff:/usr/src/app# ls
`server  text.log
`root@f28bf88fa3ff:/usr/src/app# tail -f ./text.log  
`2024-08-30 10:22:42 +0000 UTC
`2024-08-30 10:22:44 +0000 UTC
`2024-08-30 10:22:46 +0000 UTC
`2024-08-30 10:22:48 +0000 UTC
`Secret message is: 'You can find the source code here: https://github.com/docker-hy'
`2024-08-30 10:22:50 +0000 UTC
`2024-08-30 10:22:52 +0000 UTC
`2024-08-30 10:22:54 +0000 UTC
`2024-08-30 10:22:56 +0000 UTC
`2024-08-30 10:22:58 +0000 UTC
`Secret message is: 'You can find the source code here: https://github.com/docker-hy'
`2024-08-30 10:23:00 +0000 UTC
`2024-08-30 10:23:02 +0000 UTC

`root@f28bf88fa3ff:/usr/src/app#

```
