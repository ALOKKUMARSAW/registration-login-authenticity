FROM maven:3.8.5-openjdk-17 AS build
COPY . .
RUN mvn clean package -DskipTest

FROM openjdk:17.0.1-jdk-slim
COPY --from=build /target/registration-login-demo-0.0.1-SNAPSHORT.jar registration-login-demo.jar

EXPOSE 8081

ENTRYPOINT ["java", "-jar", "registration-login-demo.jar"]
