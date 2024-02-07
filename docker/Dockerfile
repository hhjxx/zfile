FROM amazoncorretto:8u402-alpine3.19-jre

USER root
WORKDIR /home/zfile/

EXPOSE 8080
ADD ./target/*.jar app.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]