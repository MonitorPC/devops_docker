FROM amazoncorretto:8-alpine3.18

EXPOSE 8000

WORKDIR /usr/src/app 

COPY . .

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"] 

