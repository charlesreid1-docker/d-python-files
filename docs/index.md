# d-python-files

simple lightweight python files server.

```
python3 -m http.simple -b 127.0.0.1 -p 8081
```

This listens for local requests on port 8081.

This service is reverse-proxied by nginx.
Users send requests to `files.charlesreid1.X/file`
and they are rewritten on the backend to 
`127.0.0.1:8081/file`.

This uses `jfloff/alpine-python:recent` 
(see [jflof/alpine-python](https://github.com/jfloff/alpine-python)).

