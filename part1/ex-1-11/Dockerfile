FROM amazoncorretto:latest

EXPOSE 8080

WORKDIR /usr/src/app

COPY pom.xml ./
COPY mvnw ./
COPY .mvn/wrapper .mvn/wrapper/
COPY src ./src

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
