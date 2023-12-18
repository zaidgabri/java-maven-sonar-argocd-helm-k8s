

# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM adoptopenjdk/openjdk11:alpine-jre

# Simply the artifact path
ARG JAR_FILE=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy the JAR file into the container at /opt/app
COPY ${JAR_FILE} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
