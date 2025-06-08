# Use official OpenJDK 17 Alpine image for lightweight Java runtime
FROM openjdk:17-jdk-alpine

# Set working directory in container
WORKDIR /app

# Copy the built jar file into container at /app/app.jar
COPY target/email-writer-sb-0.0.1-SNAPSHOT.jar app.jar

# Expose the port that Railway will assign (default 8080)
EXPOSE 8080

# Command to run the jar file
ENTRYPOINT ["java", "-jar", "app.jar"]