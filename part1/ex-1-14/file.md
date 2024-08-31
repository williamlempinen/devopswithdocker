```
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-frontend   main  docker build . -t exam
`ple-frontend:v3`

`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-frontend   main  docker run -d -p 127.0
`.0.1:5000:5000 example-frontend:v3`

`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-backend   main  docker build . -t examp
`le-backend:v2`

`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp/material-applications/example-backend   main  docker run -p 127.0.0.1
`:8080:8080 example-backend:v2`
```
