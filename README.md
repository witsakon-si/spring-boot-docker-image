## Getting Started
* Run
```mvn spring-boot:run```
http://localhost:8080
* Fix error "connection refused" on Windows
```
Docker Setting >>> General >>> [X] Expose daemon on tcp://localhost:2375 without TLS
```
* Pack & Build image
```
mvn package dockerfile:build
```
* Check & Run
```
docker images
docker run -d -p 9000:8080 witsakon/hello-docker:0.0.1-SNAPSHOT          # -d = background process
```
* Check service http://localhost:9000
