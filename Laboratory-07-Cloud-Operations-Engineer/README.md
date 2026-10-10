# Laboratory 7: Cloud Operations Engineer

## Mission Overview
I checked the health of a Linux server, ran an Nginx website, sent test visits to it, and used logs and metrics to show it works well.

## Objectives
- Check CPU, memory, and disk using Linux tools
- Run a web container and watch how much it uses
- Make web traffic and read the logs
- Write my results in Markdown

## Monitoring Commands Executed
- `free -h` : shows RAM
- `df -h` : shows disk space
- `top` : shows CPU and running programs
- `docker run -d --name client-website -p 8080:80 nginx` : starts the website
- `curl http://localhost:8080` : visits the website
- `curl http://localhost:8080/hidden-admin-page` : makes a 404 error
- `docker logs client-website` : shows the website logs
- `docker stats` : shows live CPU and memory

## Skills Learned
- Checking server resources
- Running a container
- Reading logs to find errors
- Reading container CPU and memory
- Writing reports in Markdown
