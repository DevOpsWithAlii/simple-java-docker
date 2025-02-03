# simple-java-docker
A simple java app that runs on docker.

- # Dockerfile

# use openjdk 17 as a base image
- FROM openjdk:17-jdk-alpine

# set the working directory 
- WORKDIR /app

# copy the code 
- COPY src/Main.java /app/Main.java

# compile the java app(Libraries
- RUN javac Main.java

# Add entry point to run the Main class
- CMD ["java","Main"]
