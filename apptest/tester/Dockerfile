FROM openjdk:13-alpine
RUN apk add --no-cache git && git clone https://github.com/jfrog/partner-integration-tests.git
WORKDIR partner-integration-tests
RUN ./gradlew dependencies &> /dev/null
ENTRYPOINT ["./gradlew"]
