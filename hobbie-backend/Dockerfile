# Use the official OpenJDK 11 base image
FROM openjdk:11

# Set the working directory in the container
WORKDIR /app

# Copy the JAR file from the local filesystem into the container
COPY target/*.jar app.jar
VOLUME /tmp
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar
# Set the entry point to run the JAR file
ENTRYPOINT ["java", "-jar", "app.jar"]
