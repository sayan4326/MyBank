#start with base image containing java libraries
FROM openjdk:21-slim

#info about who maintains the image
MAINTAINER EazyBank.com

#Copies the JAR you built with Maven (mvn package or mvn clean install) from your host machine into the Docker image.
#First part = source (target/accounts-0.0.1-SNAPSHOT.jar from host).
#Second part = destination (inside the container, root directory / by default).
COPY target/accounts-0.0.1-SNAPSHOT.jar app.jar


#Defines the default command to run when the container starts. for each space separator in command put in separate quote
ENTRYPOINT [ "java" , "-jar", "app.jar" ]