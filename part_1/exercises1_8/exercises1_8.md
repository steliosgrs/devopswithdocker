
```sh
docker build . -t web-server
docker run -it web-server
```

```dockerfile
# Start from the alpine image
FROM devopsdockeruh/simple-web-service:alpine

CMD server
```