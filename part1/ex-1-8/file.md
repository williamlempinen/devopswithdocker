```
wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/ex-1-8  ls
` Dockerfile
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/ex-1-8  docker build . -t web-server                                  
`[+] Building 0.0s (5/5) FINISHED                                                                                      docker:default
`=> [internal] load build definition from Dockerfile                                                                            0.0s
`=> => transferring dockerfile: 99B                                                                                             0.0s
`=> [internal] load metadata for docker.io/devopsdockeruh/simple-web-service:alpine                                             0.0s
`=> [internal] load .dockerignore                                                                                               0.0s
`=> => transferring context: 2B                                                                                                 0.0s
`=> CACHED [1/1] FROM docker.io/devopsdockeruh/simple-web-service:alpine                                                        0.0s
`=> exporting to image                                                                                                          0.0s
`=> => exporting layers                                                                                                         0.0s
`=> => writing image sha256:e10a04f0292d811eb02da7d6526d1e215c8b8e62aa36cc69177ca4d072cee933                                    0.0s
`=> => naming to docker.io/library/web-server                                                                                   0.0s
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/ex-1-8  docker run -it web-server
`[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

`[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
`- using env:   export GIN_MODE=release
`- using code:  gin.SetMode(gin.ReleaseMode)

`[GIN-debug] GET    /*path                    --> server.Start.func1 (3 handlers)
`[GIN-debug] Listening and serving HTTP on :8080
`^C%                                                                                                                                  
`✘ wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/ex-1-8   
`✘ wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/ex-1-8 `
```
