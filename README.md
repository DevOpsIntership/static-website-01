## BUILD
```
docker build \
    --tag adamkwolek/firstimage:latest \
    .
```
## RUN    
```
docker run -d \
    --name hello\
    --publish 8000:80\
    adamkwolek/firstimage:latest
```

## CLEAN
```
docker stop hello
docker rm hello
docker rmi adamkwolek/firstimage:latest
```
