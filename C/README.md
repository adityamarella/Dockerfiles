### Launch the container
```
docker run --rm -it -v "$(pwd)":/code amarella/c-dev:latest /bin/bash
```

### Demo
```
docker run --rm -it -v "$(pwd)":/code amarella/c-dev:latest /bin/bash
root@1b2f08d8498f:/# cd /code
root@1b2f08d8498f:/code# ls
C
root@1b2f08d8498f:/code# cd C/
root@1b2f08d8498f:/code/C# ls
Dockerfile  README.md  hello.c
root@1b2f08d8498f:/code/C# gcc -o hello hello.c
root@1b2f08d8498f:/code/C# ./hello
hello
root@1b2f08d8498f:/code/C# vim hello.c
root@1b2f08d8498f:/code/C# vim hello.c
root@1b2f08d8498f:/code/C# 

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
