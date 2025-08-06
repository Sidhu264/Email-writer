FROM maven:3.9.6-eclipse-temurin-24-alpine

WORKDIR /app

COPY . .

RUN mvn clean package -DskipTests

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "target/email-writer-sb-0.0.1-SNAPSHOT.jar"]
