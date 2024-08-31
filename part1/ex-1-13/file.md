```
✘ wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-backend   main  nv
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-backend   main  docker build . -t example
`-backend
`[+] Building 19.1s (13/13) FINISHED                                                                                    docker:default
`=> [internal] load build definition from Dockerfile                                                                             0.0s
`=> => transferring dockerfile: 451B                                                                                             0.0s
`=> [internal] load metadata for docker.io/library/ubuntu:latest                                                                 0.0s
`=> [internal] load .dockerignore                                                                                                0.0s
`=> => transferring context: 111B                                                                                                0.0s
`=> [1/8] FROM docker.io/library/ubuntu:latest                                                                                   0.0s
`=> [internal] load build context                                                                                                0.0s
`=> => transferring context: 499B                                                                                                0.0s
`=> CACHED [2/8] WORKDIR /usr/src/app                                                                                            0.0s
`=> CACHED [3/8] RUN apt update && apt install -y curl                                                                           0.0s
`=> [4/8] RUN curl -LO https://golang.org/dl/go1.23.0.linux-amd64.tar.gz     && tar -C /usr/local -xzf go1.23.0.linux-amd64.tar  7.1s
`=> [5/8] RUN go version                                                                                                         0.2s  
`=> [6/8] COPY . .                                                                                                               0.0s  
`=> [7/8] COPY go.* ./                                                                                                           0.1s  
`=> [8/8] RUN go build -o server .                                                                                              10.9s  
`=> exporting to image                                                                                                           0.8s  
`=> => exporting layers                                                                                                          0.8s  
`=> => writing image sha256:e6d9bac130c112cfac998d5bcdef4bfb95f2433e5ad70d3f9e34c69e882e309d                                     0.0s  
`=> => naming to docker.io/library/example-backend                                                                               0.0s  
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-backend   main  docker images
`REPOSITORY                          TAG       IMAGE ID       CREATED          SIZE
`example-backend                     latest    e6d9bac130c1   9 seconds ago    622MB
`example-frontend                    latest    908eebf6792b   19 minutes ago   610MB
`spring-project                      latest    6f1c716f8da9   39 minutes ago   435MB
`rails-project                       latest    dbc337757acc   56 minutes ago   992MB
`yt-dlp                              v2        f2f12d653e02   3 hours ago      175MB
`yt-dlp                              latest    28eb243389c2   3 hours ago      175MB
`curler                              latest    4d76f1a602c6   3 hours ago      140MB
`hello-docker                        v2        afe2a2c06528   6 hours ago      7.4MB
`hello-docker-additional             latest    ff6d86cb79e3   6 hours ago      7.4MB
`hello-docker                        latest    641efce8ffc5   6 hours ago      7.4MB
`ubuntu                              22.04     53a843653cbc   2 weeks ago      77.9MB
`ubuntu                              latest    edbfe74c41f8   4 weeks ago      78.1MB
`devopsdockeruh/simple-web-service   ubuntu    4e3362e907d5   3 years ago      83MB
`devopsdockeruh/simple-web-service   alpine    fd312adc88e0   3 years ago      15.7MB
`web-server                          latest    e10a04f0292d   3 years ago      15.7MB
`devopsdockeruh/simple-web-service   latest    99f995eeaa58   3 years ago      10.1MB
`devopsdockeruh/pull_exercise        latest    d9854bc0e13a   5 years ago      75.3MB
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-backend   main  docker run -p 127.0.0.1:8
`004:8080 example-backend  
`[Ex 2.4+] REDIS_HOST env was not passed so redis connection is not initialized
`[Ex 2.6+] POSTGRES_HOST env was not passed so postgres connection is not initialized
`[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

`[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
`- using env:   export GIN_MODE=release
`- using code:  gin.SetMode(gin.ReleaseMode)

`[GIN-debug] GET    /ping                     --> server/router.pingpong (4 handlers)
`[GIN-debug] GET    /messages                 --> server/controller.GetMessages (4 handlers)
`[GIN-debug] POST   /messages                 --> server/controller.CreateMessage (4 handlers)
`[GIN-debug] Listening and serving HTTP on :8080
`[GIN] 2024/08/30 - 17:30:33 | 404 |      26.095µs |      172.17.0.1 | GET      "/"
`[GIN] 2024/08/30 - 17:30:33 | 404 |      11.329µs |      172.17.0.1 | GET      "/favicon.ico"
`[GIN] 2024/08/30 - 17:30:40 | 200 |       7.416µs |      172.17.0.1 | GET      "/ping"
`^C%                                                                                                                                   
`✘ wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-backend   main  nv
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-backend   main  ..
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications   main `
```
