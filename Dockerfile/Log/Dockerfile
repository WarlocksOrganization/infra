FROM openjdk:17-jdk

WORKDIR /app

COPY . .

RUN ./gradlew clean build -x test

FROM openjdk:17-jdk

WORKDIR /app

COPY --from=builder /app/build/libs/*.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java","-jar","app.jar"]
