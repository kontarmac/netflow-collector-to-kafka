FROM openjdk:8-jre-alpine
ADD target/netflow-collector-1.0.jar app.jar
EXPOSE 4445/udp
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-Dspring.profiles.active=container","-jar","/app.jar"]