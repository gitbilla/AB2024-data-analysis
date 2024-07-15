# Use a base image with OpenJDK
FROM openjdk:17-jdk-alpine

# Set the working directory
WORKDIR /app

# Copy the JAR file into the container
COPY target/greetings-1.0-SNAPSHOT.jar /app/app.jar

# Expose the port your application runs on
EXPOSE 8081

# Run the application
ENTRYPOINT ["java", "-jar", "/app/app.jar", "--server.port=8081"]

