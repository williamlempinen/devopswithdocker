FROM ubuntu:latest

RUN apt update && apt install -y git bash

COPY ../ex-3-3/builder.sh ./

RUN chmod +x ./builder.sh

ENTRYPOINT ["./builder.sh"]
