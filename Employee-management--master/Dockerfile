# Use Java 17
FROM openjdk:17-jdk-slim

# Copy project files
COPY . /app
WORKDIR /app

# Build project
RUN apt-get update && apt-get install -y maven
RUN mvn clean install

# Run app
CMD ["java", "-jar", "target/employee-management-0.0.1-SNAPSHOT.jar"]
