# Docker Compose Guide

## What does the `services:` block do?

The `services:` block defines the containers that are part of the application. In this deployment, it contains two services: `database` for MariaDB and `app` for Nextcloud.

## How did the Nextcloud app container find the database container?

The Nextcloud app container uses the `MYSQL_HOST` environment variable to identify the database service. The value `database` matches the name of the MariaDB service in the Compose file, allowing Nextcloud to connect to the database container.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is used to create and start an individual Docker container by specifying its configuration in a command. In contrast, `docker-compose up -d` uses a YAML configuration file to create and start multiple related containers as a single application stack in the background.

