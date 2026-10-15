# Mission 8: The Cloud Security Engineer

## 1. Mission Overview

Congratulations! My proactive approach to system monitoring has earned me a spot on the Cloud Security Team at CloudNova Technologies.

In cloud computing, leaving a server unsecured can lead to brute-force attacks and data breaches. In this mission, I applied the security concepts from Chapter 8 by protecting a server using a host-based firewall.

Using the KillerCoda Playground, I deployed an Nginx web application, checked the server's network ports, and configured the Uncomplicated Firewall (UFW). I applied the Default Deny policy and allowed only the required traffic for SSH and the web application on port 8080.

This mission helped me understand that server security requires proper configuration, careful monitoring, and regular maintenance.

## 2. Mission Objectives

At the end of this laboratory activity, I aimed to:

- Understand the concept of Attack Surface and the Principle of Least Privilege (PoLP).
- Perform a basic security audit of active network ports on a Linux server.
- Configure the Uncomplicated Firewall (UFW) with a Default Deny policy.
- Implement specific firewall rules to allow SSH and web application traffic on port 8080.
- Document firewall rules and security best practices using Markdown.
- Continue expanding my GitHub Cloud Computing Portfolio.

## 3. Commands Executed

### Deploy the Web Application

```bash
docker --version
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
```

### Configure the Firewall

```bash
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
```

### Allow the Web Application Port

```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl http://localhost:8080
```

## 4. Skills Learned

- Deploying a web server using Docker.
- Testing a web application using curl.
- Configuring firewall rules with UFW.
- Applying the Default Deny security policy.
- Managing network access and documenting technical work in Markdown.
