# d-python-files

simple lightweight python files server.

```
python3 -m http.simple -b 127.0.0.1 -p 8081
```

This listens for local requests on port 8081.

This service is reverse-proxied by nginx.
Users send requests to `files.charlesreid1.X/file
and they are rewritten on the backend to 
`127.0.0.1:8081/file`.

This uses `debian:stretch-slim` (same as [nginx Dockerfile](https://github.com/nginxinc/docker-nginx/blob/4f5bae5928baee89433ecb20a50283546f217dfa/mainline/stretch/Dockerfile)).

