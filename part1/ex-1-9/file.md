```
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  toucch ex-1-9.txt
`zsh: correct 'toucch' to 'touch' [nyae]? y
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  ls
` ex-1-9.txt   'Welcome to Kumpula campus! ｜ University of Helsinki [DptFY_MszQs].mp4'
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  docker run -v "$(pwd)/ex-1-9.txt:/usr/src/app/text.log" devopsdockeruh/simple
`-web-service
`Starting log output
`Wrote text to /usr/src/app/text.log
`Wrote text to /usr/src/app/text.log
`Wrote text to /usr/src/app/text.log
`Wrote text to /usr/src/app/text.log
`^C%                                                                                                                                        
`✘ wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp  bat ex-1-9.txt  
`───────┬─────────────────────────────────────────────────────────────────────────────────────────────────`──────────────────────────────────
 ``     │ File: ex-1-9.txt
`───────┼─────────────────────────────────────────────────────────────────────────────────────────────────`──────────────────────────────────
 `` 1   │ 2024-08-30 15:57:54 +0000 UTC
 `` 2   │ 2024-08-30 15:57:56 +0000 UTC
 `` 3   │ 2024-08-30 15:57:58 +0000 UTC
 `` 4   │ 2024-08-30 15:58:00 +0000 UTC
``───────┴───────────────────────────────────────────────────────────────────────────────────────────────`────────────────────────────────────
`wlemp@DESKTOP-OO5ESTO  ~/dev/devops-with-docker/part1/tmp 
```
