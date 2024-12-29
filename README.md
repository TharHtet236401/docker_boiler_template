# Docker Node.js Express Boilerplate

A simple Docker boilerplate for Node.js Express applications with hot-reloading using Nodemon.

## Features

- Node.js 16 Alpine base image
- Express.js server
- Nodemon for hot-reloading
- Docker configuration
- Simple API endpoint

## Prerequisites

- Docker installed on your machine
- Docker Compose (optional)

## Project Structure

- api/: Contains the Node.js Express application code.
- Dockerfile: Defines the Docker image configuration.
- .dockerignore: Specifies files and directories to be ignored by Docker.
- readMe.md: This file.
# docker_boiler_template

## Docker Commands

Here are some useful Docker commands for working with this project:

### Building Images

docker build -t my-test-app .
docker build -t my-test-app:latest .

### Running Containers with Hot Reloading using Nodemon
### Replace "C:/Users/Thar_Htet/Desktop/docker-self/api" with your project path
docker run --name my_app_c_nodemon -p 4000:4000 --rm -v /path/to/your/project/api:/app -v /app/node_modules myapp:nodemon

### Example:
### Windows: docker run --name my_app_c_nodemon -p 4000:4000 --rm -v C:/Users/YourUsername/project/api:/app -v /app/node_modules myapp:nodemon
### Mac/Linux: docker run --name my_app_c_nodemon -p 4000:4000 --rm -v /Users/YourUsername/project/api:/app -v /app/node_modules myapp:nodemon


### Running in Bash
### For Windows users with Git Bash or WSL, or Mac/Linux users:
docker run --name my_app_c_nodemon -p 4000:4000 --rm -v "/$(pwd)/api":/app -v /app/node_modules myapp:nodemon

### Note: $(pwd) gets replaced with your current working directory path

##sample command
docker run --name my_app_c_nodemon -p 4000:4000 --rm -v C:/Users/Thar_Htet/Desktop/docker-self/api:/app -v /a
pp/node_modules myapp:nodemon


