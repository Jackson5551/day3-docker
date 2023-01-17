
# Lab 3

## Docker Swarm Stack

### Source Image

<https://github.com/Jackson5551/day2-docker>

### Build Image

```bash
docker build -t myapp:latest
```

### Create Stack

```bash
docker stack deploy -c docker-compose.yaml myapp-stack
```

### Scale First Service

```bash
docker service scale myapp-stack_mywebsite1=7
```

```bash
docker service scale myapp-stack_mywebsite1=2
```

### Delete Stack

```bash
docker stack rm myapp-stack
```
