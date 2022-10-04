# spring-pet-clinic
```
FROM openjdk:8u332-jdk
RUN git clone https://github.com/ikambarov/spring-petclinic.git
COPY spring-petclinic /app
WORKDIR /spring-petclinic/
RUN ./mvnw package
CMD "java", "-jar", "target/*.jar"

```