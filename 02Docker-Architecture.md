# 🐳 Docker Architecture – Quick Notes

## 🔹 What is Docker?

Docker is a **containerization platform** that helps developers package apps with dependencies and run them anywhere, ensuring **portability, speed, and scalability** ⚡

---

## 🏗️ Docker Architecture Components

### 1️⃣ Docker Client 🖥️

- CLI tool (`docker run`, `docker build`, etc.)
- Sends commands to **Docker Daemon** via REST API

### 2️⃣ Docker Daemon (dockerd) ⚙️

- Runs on the host machine
- Builds, runs, and manages containers
- Listens for Docker API requests

### 3️⃣ Docker Engine 🔥

- Combination of **Client + Daemon + APIs**
- Core service that enables Docker to work

### 4️⃣ Docker Objects 📦

- **Images** → Blueprints for containers
- **Containers** → Running instances of images
- **Volumes** → Persistent data storage
- **Networks** → Communication between containers

### 5️⃣ Docker Registry 🌍

- Stores Docker images
- **Docker Hub** (default) or private registries
- Used for `docker pull` & `docker push`

---

## 📊 Docker Architecture Flow

```
👨‍💻 Docker Client
|  (REST API commands)
v
⚙️ Docker Daemon (dockerd)
|  (manages)
v
📦 Docker Objects → Images | Containers | Volumes | Networks
|
v
🌍 Docker Registry (Docker Hub / Private)
```

---

## 📌 Key Takeaways

- 🧩 **Client-Server Model** → Client sends commands, Daemon executes.
- 🚀 **Fast & Lightweight** → Containers start in seconds.
- 🔄 **Images → Containers** with persistence using Volumes.
- ☁️ **Registry (Hub)** makes images shareable & portable.
