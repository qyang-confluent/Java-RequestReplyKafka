# Java-RequestReplyKafka
## Compile and package
```
mvn clean
mvn package
```

## Start testing kafka environment
```
docker-compose up -d
```

## Test 
```
java -jar target/target/RequestReplyKafka-0.0.1-SNAPSHOT.jar
curl -d @request.json -H "Content-Type: application/json"  http://localhost:8080/sum
```

## Check result using Control Center ( http://localhost:9021)
