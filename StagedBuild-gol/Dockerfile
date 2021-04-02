FROM maven:3-openjdk-8 as mvn
RUN git clone https://github.com/pbeenaveni/game-of-life.git && cd game-of-life && mvn package 

FROM tomcat:8
LABEL author="Parikshith"
COPY --from=mvn /game-of-life/gameoflife-web/target/gameoflife.war /usr/local/tomcat/webapps/gameoflife.war
EXPOSE 8080