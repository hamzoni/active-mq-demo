FROM openjdk:8-jdk-alpine
MAINTAINER taquy <taquy.se@gmail.com>
VOLUME /tmp
EXPOSE 8081
ARG JAR_FILE=target/service-a-0.0.1-SNAPSHOT.jar                                            
ADD ${JAR_FILE} service-a.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/service-a.jar"]

