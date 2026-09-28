# 🐳 Docker Test Page

A simple HTML page served using **Nginx inside a Docker container**.
This project is useful for learning and testing basic Docker concepts.

## 📁 Project Structure

```text
docker-test/
│
├── index.html
├── Dockerfile
└── README.md
```

## 🚀 How to Run

### 1. Build the Docker Image

```bash
docker build -t docker-test .
```

### 2. Run the Container

```bash
docker run -d -p 8080:80 --name docker-test-container docker-test
```

### 3. Open in Browser

Go to:

```text
http://localhost:8080
```

You should see:

> 🐳 Docker Test Page
> Hello from inside a Docker container!
> ✅ Container is running successfully

## 🔍 Useful Docker Commands

Check running containers:

```bash
docker ps
```

Stop the container:

```bash
docker stop docker-test-container
```

Start it again:

```bash
docker start docker-test-container
```

Remove the container:

```bash
docker rm docker-test-container
```

Remove the image:

```bash
docker rmi docker-test
```

## 🛠️ Technologies Used

* HTML
* Nginx
* Docker

## 🎯 Purpose

This project demonstrates how to:

* Create a Docker image
* Run an Nginx container
* Serve a static HTML page
* Map a container port to the host machine
* Manage Docker containers using basic commands
