### Launch the container
```
docker run --rm -it -v "$(pwd)":/code amarella/c-dev:latest /bin/bash
```

### Common Issues
Add the current working directory to File Sharing from Docker -> Preferences... -> File Sharing
```
docker: Error response from daemon: Mounts denied: o.
.

The path ...
is not shared from OS X and is not known to Docker.
You can configure shared paths from Docker -> Preferences... -> File Sharing.
See https://docs.docker.com/docker-for-mac/osxfs/#namespaces for more inf.
ERRO[0000] error getting events from daemon: net/http: request canceled 
```
