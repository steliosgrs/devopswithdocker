# Start from the alpine image
FROM amazoncorretto:8

WORKDIR /path/java/app/

COPY ./spring-example-project .

RUN ./mvnw package

EXPOSE 8080

ENTRYPOINT [ "java", "-jar", "./target/docker-example-1.1.3.jar" ] 