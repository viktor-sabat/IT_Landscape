Welcome to the IT_Landscape wiki!

# Main Page

## Introduction to Docker
- Docker is a platform that allows you to package, distribute, and run applications in containers.
- It provides a consistent environment for running applications, ensuring they behave the same way regardless of the underlying infrastructure.

## Installation Instructions
- **Windows**: Visit the Docker website and download the Docker Desktop installer. Follow the installation wizard to complete the installation process.
- **macOS**: Install Docker Desktop from the Docker website by downloading the installer and following the installation instructions.
- **Linux**: Install Docker Engine using the official installation script provided by Docker. Follow the instructions on the Docker documentation page for your specific Linux distribution.

## Basic Commands
- **docker run**: Used to run a Docker container based on a specific image.
  Example: ```docker run -d -p 8080:80 nginx
- **docker build**: Builds a Docker image from a Dockerfile.
  Example: `docker build -t myapp .`
- **docker ps**: Lists all running containers.
  Example: `docker ps`
- **docker images**: Lists all Docker images on the host system.
  Example: `docker images`

## Dockerfile
- A Dockerfile is a text document that contains instructions for building a Docker image.
- Each instruction in the Dockerfile adds a new layer to the image, representing a change to the image's filesystem.
- Example Dockerfile:
  ```dockerfile
  FROM node:alpine
  WORKDIR /app
  COPY . .
  CMD ["node", "app.js"]
