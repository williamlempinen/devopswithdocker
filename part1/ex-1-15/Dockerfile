FROM ubuntu:latest

EXPOSE 3000

WORKDIR /usr/src/app

RUN apt update && apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_20.x | bash
RUN apt install -y nodejs

COPY package*.json ./

RUN npm install 

COPY . .

CMD ["npm", "run", "dev"]
