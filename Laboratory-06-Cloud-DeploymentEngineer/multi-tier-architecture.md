# Two-Tier Architecture

## What is a Two-Tier Architecture?

A Two-Tier Architecture is an application structure divided into two main parts: the Web/Application Tier and the Database Tier. In this activity, the Web/Application Tier uses Nextcloud, while the Database Tier uses MariaDB.

## The Web/Application Tier

The Web/Application Tier is responsible for serving the user interface and handling HTTP requests from users. In this activity, the Nextcloud container provides the web application that users access through a browser.

## The Database Tier

The Database Tier is responsible for storing persistent data, including user accounts and other information needed by the application. In this activity, MariaDB is used as the database container for Nextcloud.

## Why Separate Them?

Separating the web server and database into different containers makes the application easier to manage and maintain. Each container has a specific role, so the web application and database can be managed independently instead of placing everything inside one container.

