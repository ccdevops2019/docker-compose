FROM openjdk:8-jdk-alpine
RUN mkdir -p /app 
COPY spring-petclinic-2.1.0.BUILD-SNAPSHOT.jar /app/app.jar
EXPOSE 8080
ENTRYPOINT ["java", "-Dspring.profiles.active=mysql", "-Dspring.datasource.initialize=true", "-jar","/app/app.jar"]