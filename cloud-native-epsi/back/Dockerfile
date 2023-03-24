FROM docker.io/maven:adoptopenjdk

COPY pom.xml .
COPY src ./src

RUN mvn verify

EXPOSE 8080

CMD ["java","-Xmx8m","-Xms8m" ,"-jar", "/target/words.jar"]
