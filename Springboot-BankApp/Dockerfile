FROM maven:3.8.3-openjdk-17 AS builder

WORKDIR /app

COPY . .

RUN mvn clean install -DskipTests=true

FROM gcr.io/distroless/java17

COPY --from=builder /app/target/*.jar /app/bankapp.jar

EXPOSE 8080

CMD ["/app/bankapp.jar"] 
