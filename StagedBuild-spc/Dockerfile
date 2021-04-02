FROM maven:3-openjdk-11 as mvn
RUN git clone https://github.com/pbeenaveni/spring-petclinic.git && cd spring-petclinic && mvn package 

FROM openjdk:11
LABEL author="Parikshith"
COPY --from=mvn /spring-petclinic/target/spring-petclinic-2.4.2.jar /spring-petclinic-2.4.2.jar
CMD [ "java", "-jar", "/spring-petclinic-2.4.2.jar"]
EXPOSE 8080