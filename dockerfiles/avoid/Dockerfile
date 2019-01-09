FROM maven:3.5-jdk-8
COPY src /usr/src/app/src
COPY pom.xml /usr/src/app
RUN mvn -f /usr/src/app/pom.xml clean package
ENTRYPOINT ["java","-jar","/usr/src/app/target/spring-boot-docker-1.0.0.jar"]