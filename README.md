# linux-toolbox
Docker image with useful linux tools for troubleshooting and perf analysis

# Build Image
```

```

# Running container
``
docker run -it --pid=host --privileged --network=host -v /sys/kernel/debug:/sys/kernel/debug localhost:5000/linux-toolbox:v1 /bin/bash
```
