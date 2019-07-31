# Building a RESTful Web Service

[Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)

## Build

`mvn clean package`

## Test run locally

`java -jar target/gs-rest-0.1.0.jar`

`curl localhost:8080/greeting`

## Create manifest.yml

```
---
applications:
# Application
- name: gs-rest
  instances: 1
  memory: 1024M
  path: target/gs-rest-0.1.0.jar
```

## Deploy to SAP Cloud Foundry

`cf push`
