# Docker Container Lifecycle

## 1. List Running Containers

```bash
docker ps
```

This command lists the Docker containers that are currently running.

## 2. Stop the Running Container

```bash
docker stop cfa2eb2639cc
```

This command stops the running Nginx container using its container ID.

## 3. Verify the Container Is Stopped

```bash
docker ps
```

This command verifies that the Nginx container is no longer listed among the running containers.

## 4. Remove the Container

```bash
docker rm cfa2eb2639cc
```

This command completely removes the stopped Nginx container from the Docker environment.

