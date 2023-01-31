FROM maven:3.8.4-jdk-11-slim AS builder

EXPOSE 80/tcp

WORKDIR /builder

COPY . .

RUN mvn dependency:resolve

RUN mvn package

FROM openjdk:11-jre-slim AS run

EXPOSE 80/tcp

WORKDIR /builder

COPY --from=builder /builder/.env .

COPY --from=builder /builder/target/worker-jar-with-dependencies.jar .

CMD ["java", "-jar", "worker-jar-with-dependencies.jar"]
