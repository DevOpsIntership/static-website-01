## BUILD
```
docker build \
    --tag adkwolek/hello:latest \
    .
```
## RUN    
```
docker run -d \
    --name hello\
    --publish 8000:80\
    adkwolek/hello:latest
```

## CLEAN
```
docker stop hello
docker rm hello
docker rmi adkwolek/hello:latest
```