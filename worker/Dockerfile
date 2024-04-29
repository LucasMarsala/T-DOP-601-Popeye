FROM maven:3.9.6-eclipse-temurin-21-alpine AS builder

EXPOSE 80/tcp

WORKDIR /builder

COPY . .

RUN mvn dependency:resolve

RUN mvn package

FROM eclipse-temurin:21-jre-alpine AS run

EXPOSE 80/tcp

WORKDIR /builder

COPY --from=builder /builder/target/worker-jar-with-dependencies.jar .

CMD ["java", "-jar", "worker-jar-with-dependencies.jar"]
