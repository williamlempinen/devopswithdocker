FROM ubuntu:latest

EXPOSE 8080

WORKDIR /usr/src/app

RUN apt update && apt install -y curl

RUN curl -LO https://golang.org/dl/go1.23.0.linux-amd64.tar.gz \
    && tar -C /usr/local -xzf go1.23.0.linux-amd64.tar.gz \
    && rm go1.23.0.linux-amd64.tar.gz

ENV PATH=$PATH:/usr/local/go/bin

RUN go version

COPY . .
COPY go.* ./

RUN go build -o server .

ENV REQUEST_ORIGIN=http://localhost

RUN useradd -m appuser

RUN chown appuser .

USER appuser

CMD ["./server"]
