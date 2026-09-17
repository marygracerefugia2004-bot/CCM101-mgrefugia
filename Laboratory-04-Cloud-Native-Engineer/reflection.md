# Mission Reflection

## 1. How does the boot time and setup process of a Docker container compare to installing an operating system on a Virtual Machine?

Docker containers start faster because they do not need a full operating system. A Virtual Machine needs to run its own operating system, so it takes more time. Docker is lightweight and runs applications.

## 2. Why is port mapping (-p 8080:80) necessary when running a web server inside a container?

Port mapping lets the host access the web server inside the container. Port 8080 is the host port, while port 80 is used by Nginx. Without port mapping, I cannot access Nginx using localhost:8080.

## 3. What happens to the data inside a container when you use the docker rm command?

The docker rm command removes a stopped container. Data stored only inside the container can be removed. Important data should be stored using persistent storage when needed.

## 4. How do you think containerization changes the way software developers and IT operations teams work together (DevOps)?

Containerization helps developers and IT operations teams work together because applications can be packaged with needed files and settings. This makes applications more consistent between environments and makes deployment easier.

## 5. How is your GitHub portfolio evolving?

My GitHub portfolio is improving as I add laboratory activities, Markdown files, screenshots, and documentation. I am becoming more comfortable organizing folders and recording work. I found this activity easier than the previous one because the Docker commands were direct. I also learned to be careful with command spacing and formatting.

