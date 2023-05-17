FROM openjdk:8

EXPOSE 8080

WORKDIR /usr/src/app

# Copy source code
COPY . .

# Build the project
RUN ./mvnw package

# Run the application
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

# Docker command to build and run container:
# docker build . -t java-project && docker run -p 127.0.0.1:8080:8080 java-project
