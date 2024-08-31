```
`✘ wlemp@DESKTOP-OO5ESTO  ~  docker images                
`REPOSITORY                          TAG       IMAGE ID       CREATED       SIZE
`ubuntu                              latest    edbfe74c41f8   4 weeks ago   78.1MB
`devopsdockeruh/simple-web-service   ubuntu    4e3362e907d5   3 years ago   83MB
`devopsdockeruh/simple-web-service   alpine    fd312adc88e0   3 years ago   15.7MB
`wlemp@DESKTOP-OO5ESTO  ~ `
`✘ wlemp@DESKTOP-OO5ESTO  ~  docker start  brave_lewin   
`brave_lewin
`wlemp@DESKTOP-OO5ESTO  ~  docker exec -it brave_lewin sh
`/usr/src/app # ls
`server    text.log
`/usr/src/app # tail -f ./text.log  
`2024-08-30 11:24:27 +0000 UTC
`2024-08-30 11:24:29 +0000 UTC
`2024-08-30 11:24:31 +0000 UTC
`2024-08-30 11:24:33 +0000 UTC
`2024-08-30 11:24:35 +0000 UTC
`Secret message is: 'You can find the source code here: https://github.com/docker-hy'
`2024-08-30 11:24:37 +0000 UTC
`2024-08-30 11:24:39 +0000 UTC
``^C
`/usr/src/app #`
`✘ wlemp@DESKTOP-OO5ESTO  ~  docker ps -a                   
`CONTAINER ID   IMAGE                                      COMMAND                 CREATED             STATUS                      POR
`TS     NAMES
`4ae69a461f34   devopsdockeruh/simple-web-service:alpine   "/usr/src/app/server"   7 minutes ago       Up About a minute              
``      brave_lewin
`f28bf88fa3ff   devopsdockeruh/simple-web-service:ubuntu   "/usr/src/app/server"   About an hour ago   Exited (2) 54 minutes ago      
``      ex-1-3
`wlemp@DESKTOP-OO5ESTO  ~  docker start ex-1-3       
`ex-1-3
`wlemp@DESKTOP-OO5ESTO  ~  docker exec -it ex-1-3 bash
`root@f28bf88fa3ff:/usr/src/app# ls
`server  text.log
`root@f28bf88fa3ff:/usr/src/app# tail -f ./text.log  
`2024-08-30 11:26:33 +0000 UTC
`2024-08-30 11:26:35 +0000 UTC
`2024-08-30 11:26:37 +0000 UTC
`2024-08-30 11:26:39 +0000 UTC
`Secret message is: 'You can find the source code here: https://github.com/docker-hy'
`2024-08-30 11:26:41 +0000 UTC
`2024-08-30 11:26:43 +0000 UTC
`2024-08-30 11:26:45 +0000 UTC
`2024-08-30 11:26:47 +0000 UTC
`2024-08-30 11:26:49 +0000 UTC
`Secret message is: 'You can find the source code here: https://github.com/docker-hy'
`2024-08-30 11:26:51 +0000 UTC
`^C
`root@f28bf88fa3ff:/usr/src/app# read escape sequence
`✘ wlemp@DESKTOP-OO5ESTO  ~ `
```
