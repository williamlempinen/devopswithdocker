```
✘ wlemp@DESKTOP-OO5ESTO  ~  docker run -d training-api:latest
`1b4e9da0999ad34fcc8b33ad4d605f443de2b07321058c92c845b303c39f47e4
`wlemp@DESKTOP-OO5ESTO  ~  docker ps                         
`CONTAINER ID   IMAGE                 COMMAND                  CREATED         STATUS         PORTS      NAMES
`1b4e9da0999a   training-api:latest   "/tini -- docker-ent…"   5 seconds ago   Up 5 seconds   8000/tcp   exciting_pare
`c9196aa05047   nginx                 "/docker-entrypoint.…"   2 minutes ago   Up 2 minutes   80/tcp     awesome_swanson
`wlemp@DESKTOP-OO5ESTO  ~  docker ps
`CONTAINER ID   IMAGE                 COMMAND                  CREATED          STATUS          PORTS      NAMES
`1b4e9da0999a   training-api:latest   "/tini -- docker-ent…"   41 seconds ago   Up 41 seconds   8000/tcp   exciting_pare
`c9196aa05047   nginx                 "/docker-entrypoint.…"   2 minutes ago    Up 2 minutes    80/tcp     awesome_swanson
`wlemp@DESKTOP-OO5ESTO  ~  docker run jwilder/whoami:latest  
`Listening on :8000
`^C%                                                                                                                                  
`✘ wlemp@DESKTOP-OO5ESTO  ~  docker run -d jwilder/whoami:latest
`0edfe30d207eb6a28758275535f1560944ee15770aaaaf1eac37ae1fd8dfbc94
`wlemp@DESKTOP-OO5ESTO  ~  docker ps                           
`CONTAINER ID   IMAGE                   COMMAND                  CREATED              STATUS              PORTS      NAMES
`0edfe30d207e   jwilder/whoami:latest   "/app/http"              3 seconds ago        Up 3 seconds        8000/tcp   fervent_knuth
`1b4e9da0999a   training-api:latest     "/tini -- docker-ent…"   About a minute ago   Up About a minute   8000/tcp   exciting_pare
`c9196aa05047   nginx                   "/docker-entrypoint.…"   3 minutes ago        Up 3 minutes        80/tcp     awesome_swanson
`wlemp@DESKTOP-OO5ESTO  ~  docker stop 0e 1b4
`0e
`1b4
`wlemp@DESKTOP-OO5ESTO  ~  docker ps          
`CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS         PORTS     NAMES
`c9196aa05047   nginx     "/docker-entrypoint.…"   3 minutes ago   Up 3 minutes   80/tcp    awesome_swanson
`wlemp@DESKTOP-OO5ESTO  ~ `

```
