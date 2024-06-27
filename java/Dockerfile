# build
FROM gradle:8.8.0-jdk22 AS build

WORKDIR /app

COPY src/ .

RUN gradle build

# run
FROM amazoncorretto:22-jdk

WORKDIR /app

COPY --from=build /app/build/libs .

ENTRYPOINT ["java","-jar","payroll-0.0.1-SNAPSHOT.jar"]
