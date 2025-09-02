# 📦 Docker Image – Quick Notes

## 🔹 What is a Docker Image?

- A **read-only template** used to create containers.
- Contains **application code + libraries + dependencies + OS packages**.
- Built using a **Dockerfile**.
- Stored in **Docker Registry (Docker Hub or Private)**.

---

## 🏗️ Structure of a Docker Image

### 1️⃣ Base Image 🏗️

- Starting point (e.g., Ubuntu, Alpine, Node, Python).

### 2️⃣ Layers 🧱

- Each command in Dockerfile = a new **layer**.
- Layers are **stacked** and **cached** for efficiency.

### 3️⃣ Metadata 🗂️

- Info like default command (`CMD`), ports, environment variables.

---

## ⚡ Lifecycle of Docker Image

1. **Write Dockerfile** 📝
2. **Build Image** → `docker build -t myapp .` 🔨
3. **Store Image** → in local system or Docker Hub 📂
4. **Run Container** → `docker run myapp` ▶️

---

## 📊 Docker Image Flow

```

📝 Dockerfile
↓  (docker build)
📦 Docker Image
↓  (docker run)
🐳 Docker Container

```

---

## 📌 Key Points

- 📦 Image = Blueprint | 🐳 Container = Running instance
- 🧱 Images are built in **layers** (reusable & efficient).
- 🌍 Stored & shared via **Docker Registry**.
- 🔄 Images can be **tagged & versioned**.
- ⚡ Lightweight & portable across environments.
