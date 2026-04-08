FROM openjdk:17-jdk-slim

COPY . /app
WORKDIR /app

RUN apt-get update && apt-get install -y maven
RUN mvn clean install

CMD ["java", "-jar", "target/employee-management-0.0.1-SNAPSHOT.jar"]
