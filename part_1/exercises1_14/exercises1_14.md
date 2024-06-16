
```sh
docker build . -t backend
docker run -d -p 8080:8080 backend 
docker build . -t frontend
docker run -d -p 5000:5000 frontend 
```

# Go to your browser
```txt
http://localhost:5000/
```