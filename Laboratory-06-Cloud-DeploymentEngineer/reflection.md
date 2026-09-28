# Mission 6 Reflection

## 1. How does writing a docker-compose.yml file make a cloud engineer's job easier compared to manually typing commands?

Writing a `docker-compose.yml` file makes deployment easier because the configuration is saved in one file. Instead of repeatedly typing commands for every container, the engineer can use one Compose command to deploy the whole application. It also helps keep the deployment organized and consistent.

## 2. What happens if you make an indentation error (like using a Tab instead of Spaces) in a YAML file?

An indentation error can cause the YAML file to become invalid. Docker Compose may fail to read the configuration correctly and the deployment command can produce an error. This showed me why spacing is important when working with YAML files.

## 3. Why did we use environment variables (like MYSQL_PASSWORD) in the Compose file?

Environment variables provide configuration values that the containers need to work together. For example, `MYSQL_PASSWORD` gives Nextcloud the database password needed to connect to MariaDB. They also make important configuration values easier to manage in the Compose file.

## 4. How did it feel to deploy a fully functional enterprise cloud storage system (Nextcloud) in just a few minutes?

It felt satisfying because the deployment was completed much faster than I expected. Seeing Nextcloud become available through the browser showed me how Docker Compose can simplify the deployment of a multi-container application.

## 5. How has your understanding of Cloud Computing evolved since Mission 1?

Since Mission 1, my understanding of Cloud Computing has grown from learning basic cloud concepts to actually deploying and managing cloud-based systems. I learned about infrastructure, containers, storage, and now multi-container applications. This mission helped me understand how Infrastructure as Code can make cloud deployment more organized and repeatable.

