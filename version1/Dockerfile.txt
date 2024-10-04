FROM openjdk:17-jdk-slim

WORKDIR /app

# Copy your Java server file
COPY . .

# Compile the server file
RUN javac Server.java

# Command to run the server on startup
CMD ["java", "Server"]
