# Node.js Express Application with Docker Usage Guide

This repository contains a Node.js application built using the Express framework. The main objective is to provide a comprehensive guide on using Docker for containerization, including the creation and management of containers.

## Prerequisites

Before you begin, ensure the following prerequisites are met:

1. **Node.js**: Install Node.js by downloading it from the [official website](https://nodejs.org/).
2. **Docker**: Install Docker by following the instructions for your operating system from the [official Docker documentation](https://docs.docker.com/get-docker/).

## Getting Started

Follow the steps below to set up and use Docker for containerizing your Node.js Express application:

### 1. Clone the Repository

```bash
git https://github.com/eduardoraider/nodejs-express-docker-demo.git
cd nodejs-express-docker-demo
```

### 2. Build Docker Image

Navigate to the project directory and build a Docker image for your application:

```bash
docker build -t nodejs-express-app/app-node:1.0 .
```

### 3. Run Docker Container

Run a Docker container using the image you built:

```bash
docker run -p 9090:6000 -d nodejs-express-app/app-node:1.0
```

### 4. Access the Application

Open your web browser and go to `http://localhost:9090` to access the running Node.js Express application within the Docker container.

### 5. Manage Containers

You can manage your Docker containers using various commands. Here are some useful ones:

- List all running containers:
  ```bash
  docker ps
  ```

- Stop a container:
  ```bash
  docker stop container_id
  ```

- Remove a container:
  ```bash
  docker rm container_id
  ```

- List all images:
  ```bash
  docker images
  ```

- Remove an image:
  ```bash
  docker rmi image_id
  ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.

---

#### by Eduardo O Raider
🛠 🥋 **Software Engineer**