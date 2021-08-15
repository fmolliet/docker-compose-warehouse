FROM openjdk:8-jdk-alpine

RUN addgroup -S spring && adduser -S spring -G spring
USER spring:spring

ARG JAR_FILE=target/*.jar
ADD ${JAR_FILE} app.jar

EXPOSE 8080
ENTRYPOINT ["java","-Xmx521m" ,"-jar", "/app.jar"]