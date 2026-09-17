# Laboratory Activity 4 – The Cloud-Native Engineer

## Mission Overview

This activity focused on learning the basics of cloud-native technologies, especially Docker containers. I compared Virtual Machines and Containers and used the KillerCoda Playground to work with Docker. I also deployed an Nginx web server inside a container and practiced basic container management commands.

## Objectives

* Understand the difference between Virtual Machines and Containers.
* Use the KillerCoda Playground with Docker.
* Learn and use basic Docker commands.
* Pull and run an Nginx container.
* Stop and remove a Docker container.
* Document my Docker activities using Markdown.
* Continue improving my GitHub cloud computing portfolio.

## Docker Commands Executed

### Checkpoint 3 – Docker Playground

```bash
docker --version
docker info
```

### Checkpoint 4 – Nginx Deployment

```bash
docker pull nginx
docker run -d -p 8080:80 nginx
curl http://localhost:8080
```

### Checkpoint 5 – Container Lifecycle

```bash
docker ps
docker stop cfa2eb2639cc
docker ps
docker rm cfa2eb2639cc
```

## Skills Learned

* I learned the basic difference between VMs and Containers.
* I learned how to check if Docker is installed and running.
* I learned how to pull an image and run a container.
* I learned how port mapping works in Docker.
* I learned how to check, stop, and remove a container.
* I practiced writing technical information using Markdown.
* I also continously learned how to organize my activities in my GitHub portfolio.

## Challenges Encountered

One small challenge I had was making sure the Docker commands had the correct spacing and format, especially when using `-d` and `-p 8080:80`. I also had to make sure I used the correct container ID when stopping and removing the Nginx container. After following the commands and checking the output in the terminal, I was able to understand them better. Compared with the previous activity, I found this activity easier because the commands were more direct and I could immediately see the results.

