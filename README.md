# linux-toolbox
Docker image with useful linux tools for troubleshooting and perf analysis.

# Build Image
Build docker image with `linux-toolbox:v1` as name:tag:
```
docker build -t linux-toolbox:v1 . -f linux-tools.dockerfile
```

# Running Container
Run docker container in privileged mode:
```
docker run -it --pid=host --privileged --network=host -v /sys/kernel/debug:/sys/kernel/debug localhost:5000/linux-toolbox:v1 /bin/bash
```
