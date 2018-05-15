# d-python-files

This container runs a simple lightweight Python 
HTTP file server for files.charlesreid1.com.

Here's the one-liner:

```
python3 -m http.simple -b <docker-ip> -p <port>
```

This binds to the docker network and listens for requests on a port.
Requests for files.charlesreid1.com are reverse-proxied by the nginx 
frontend (see [d-nginx-charlesreid1](https://git.charlesreid1.com/docker/d-nginx-charlesreid1))
and passed along to the internal docker network.

This uses `jfloff/alpine-python:recent` 
(see [jflof/alpine-python](https://github.com/jfloff/alpine-python)).

## Links 

[documentation: d-python-files container](https://pages.charlesreid1.com/d-python-files/) (you are here)

[source code on git.charlesreid1.com: d-python-files](https://git.charlesreid1.com/docker/d-python-files)

[source code on github.com: charlesreid1-docker/d-python-files](https://github.com/charlesreid1-docker/d-python-files)


