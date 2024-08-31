```
`wlemp@DESKTOP-OO5ESTO  ~  docker run -it --name ubu ubuntu:latest
`root@e0d0e8620224:/# apt update`
`root@e0d0e8620224:/# apt install curl`
`root@e0d0e8620224:/# %                                                                                   wlemp@DE
`SKTOP-OO5ESTO  ~  docker ps                               
`CONTAINER ID   IMAGE           COMMAND       CREATED          STATUS          PORTS     NAMES
`e0d0e8620224   ubuntu:latest   "/bin/bash"   29 seconds ago   Up 28 seconds             ubu
`wlemp@DESKTOP-OO5ESTO  ~  docker exec -it ubu sh -c 'while true; do echo "Input website:"; read website; echo
`"Searching.."; sleep 1; curl http://$website; done'`
`Input website:
``helsinki.fi
`Searching..
`<html>
`<head><title>301 Moved Permanently</title></head>
`<body>
`<center><h1>301 Moved Permanently</h1></center>
<hr><center>nginx/1.22.1</center>
`</body>
`</html>
`Input website:
`read escape sequence
`✘ wlemp@DESKTOP-OO5ESTO  ~ `
```
