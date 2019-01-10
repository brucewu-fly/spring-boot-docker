# Spring boot docker

## Build images
Run the following commands to build images.
```
# For non-optimized
docker build -t com.aliyun/spring-boot-docker-avoid:1.0.0 -f dockerfiles/avoid/Dockerfile .

# For multi-stage
docker build -t com.aliyun/spring-boot-docker-multi-stage:1.0.0 -f dockerfiles/multi-stage/Dockerfile .

# For distroless 
docker build -t com.aliyun/spring-boot-docker-distroless:1.0.0 -f dockerfiles/distroless/Dockerfile .

# For alpine 
docker build -t com.aliyun/spring-boot-docker-alpine:1.0.0 -f dockerfiles/alpine/Dockerfile .
```

## Run containers
Run the following commands to start containers.
```
docker run -it --rm -p 8080:8080 com.aliyun/spring-boot-docker-avoid:1.0.0

docker run -it --rm -p 8081:8080 com.aliyun/spring-boot-docker-multi-stage:1.0.0

docker run -it --rm -p 8082:8080 com.aliyun/spring-boot-docker-distroless:1.0.0

docker run -it --rm -p 8083:8080 com.aliyun/spring-boot-docker-alpine:1.0.0
```

