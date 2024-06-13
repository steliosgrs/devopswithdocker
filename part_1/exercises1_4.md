
I use `` tildas because windows 
```sh
 docker run -it --rm --name exer1_4 ubuntu sh -c "apt update && apt install -y curl && apt upgrade -y && sleep 2 && while true; do echo 'Input website:'; read website; echo 'Searching..`$website`'; sleep 1; curl http://`$website`/; done"
```

```txt
Unpacking libudev1:amd64 (255.4-1ubuntu8.1) over (255.4-1ubuntu8) ...
Setting up libudev1:amd64 (255.4-1ubuntu8.1) ...
Processing triggers for libc-bin (2.39-0ubuntu8.2) ...
Input website:
helsinki.fi
Searching..$website
<html>
<head><title>301 Moved Permanently</title></head>
<body>
<center><h1>301 Moved Permanently</h1></center>
<hr><center>nginx/1.22.1</center>
</body>
</html>
Input website:

```