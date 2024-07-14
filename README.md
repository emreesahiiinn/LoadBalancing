# Load Balancing with Docker and Nginx for ASP.NET Core Project

This project demonstrates how to set up load balancing for an ASP.NET Core application using Docker and Nginx.

## Project Overview

The project is an ASP.NET Core application that has been configured to run multiple instances using Docker containers. Nginx is used as a reverse proxy to distribute incoming requests across these instances, effectively balancing the load.

### Key Components

1. **ASP.NET Core Application**: A simple web application built with .NET 8.
2. **Docker**: Containerization of the application to run multiple instances.
3. **Nginx**: Used as a reverse proxy to load balance the traffic between the instances.

### Files Included

- **Dockerfile**: Instructions to build the Docker image for the ASP.NET Core application.
- **docker-compose.yml**: Configuration to run multiple instances of the application and Nginx.
- **nginx.conf**: Nginx configuration file for load balancing.
- **launchSettings.json**: Launch settings for the ASP.NET Core application.

## Running the Project

To run the project, ensure Docker and Docker Compose are installed on your machine. Use the following command to build and start the containers:

```sh
docker-compose up --build