```
Message in browser :8000 -> {"message":"You connected to the following path: /","path":"/"}

`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  docker ps     
`CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  docker images
`REPOSITORY                          TAG       IMAGE ID       CREATED             SIZE
`yt-dlp                              latest    28eb243389c2   About an hour ago   175MB
`yt-dlp                              v2        f2f12d653e02   About an hour ago   175MB
`curler                              latest    4d76f1a602c6   2 hours ago         140MB
`hello-docker                        v2        afe2a2c06528   4 hours ago         7.4MB
`hello-docker-additional             latest    ff6d86cb79e3   4 hours ago         7.4MB
`hello-docker                        latest    641efce8ffc5   4 hours ago         7.4MB
`ubuntu                              22.04     53a843653cbc   2 weeks ago         77.9MB
`ubuntu                              latest    edbfe74c41f8   4 weeks ago         78.1MB
`devopsdockeruh/simple-web-service   ubuntu    4e3362e907d5   3 years ago         83MB
`web-server                          latest    e10a04f0292d   3 years ago         15.7MB
`devopsdockeruh/simple-web-service   alpine    fd312adc88e0   3 years ago         15.7MB
`devopsdockeruh/simple-web-service   latest    99f995eeaa58   3 years ago         10.1MB
`devopsdockeruh/pull_exercise        latest    d9854bc0e13a   5 years ago         75.3MB
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  docker run web-server
`[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

`[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
`- using env:   export GIN_MODE=release
`- using code:  gin.SetMode(gin.ReleaseMode)

`[GIN-debug] GET    /*path                    --> server.Start.func1 (3 handlers)
`[GIN-debug] Listening and serving HTTP on :8080
`^C%                                                                                                                                   
`✘ wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  docker ps             
`CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  docker run web-server -p 127.0.0.1:8000:8080


               The application accepts 1 argument "server". Use the argument server to run the server

               If no arguments are supplied the application will output log strings to a file.


`Arguments given: -p 127.0.0.1:8000:8080
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  docker run -p 127.0.0.1:8000:8080 web-server  
`[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

`[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
`- using env:   export GIN_MODE=release
`- using code:  gin.SetMode(gin.ReleaseMode)

`[GIN-debug] GET    /*path                    --> server.Start.func1 (3 handlers)
`[GIN-debug] Listening and serving HTTP on :8080
`[GIN] 2024/08/30 - 16:13:43 | 200 |      60.595µs |      172.17.0.1 | GET      "/"
`[GIN] 2024/08/30 - 16:13:43 | 200 |      21.763µs |      172.17.0.1 | GET      "/favicon.ico"
`^C%                                                                                                                                   
`✘ wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp `
```
