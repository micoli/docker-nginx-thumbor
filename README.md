# docker-nginx-thumbor

## build
```
docker rm docker-nginx-thumbor; \
docker kill docker-nginx-thumbor; \
docker build -t docker-nginx-thumbor . && \
docker run -it --rm \
    -v $(PWD):/app \
    -p 8000:80 \
    --env THUMBOR_DEFAULT_HOST=192.168.2.100 \
    --name docker-nginx-thumbor \
    docker-nginx-thumbor
    
```
