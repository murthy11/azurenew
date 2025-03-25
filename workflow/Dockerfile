# To pull the base image  lolhens/baseimage-openjre

FROM  openjdk:8-jdk-alpine

# To set environment variables
WORKDIR /app
#To set environment variables
ENV  JAR_NAME=bookpoint-order-processor-0.0.1-SNAPSHOT.jar

# Run To execute the commands
RUN npm install
# Copy the application JAR file
Copy target/${JAR_NAME} ./app.jar

# Run the application
EXPOSE 8080
#To provide default for an executing container

CMD sh ./startproject.sh
