FROM ubuntu:18.04
LABEL Author=Parikshith
LABEL EMAIL=pb@123.com
LABEL Version=1.0
RUN apt update && apt install openjdk-8-jdk wget -y
ADD https://referenceappkhaja.s3-us-west-2.amazonaws.com/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar .
CMD [ "java", "-jar", "spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar"]
EXPOSE 8080