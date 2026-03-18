# Hello World Web 👋

[![Source on GitHub](https://img.shields.io/badge/source-GitHub-black?logo=github)](https://github.com/albertrodriguezdev/docker-hello-world-web) [![GitHub Repo stars](https://img.shields.io/github/stars/albertrodriguezdev/docker-hello-world-web)](https://github.com/albertrodriguezdev/docker-hello-world-web)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/albertrodriguezdev/hello-world-web/blob/main/LICENSE) [![Docker Pulls](https://img.shields.io/docker/pulls/albertrodriguezdev/hello-world-web)](https://hub.docker.com/r/albertrodriguezdev/hello-world-web) [![Docker Image Size](https://img.shields.io/docker/image-size/albertrodriguezdev/hello-world-web/latest)](https://hub.docker.com/r/albertrodriguezdev/hello-world-web)

🐙 **GitHub Repository:** [albertrodriguezdev/hello-world-web](https://github.com/albertrodriguezdev/docker-hello-world-web)  
🐳 **Docker Hub Image:** [albertrodriguezdev/hello-world-web](https://hub.docker.com/r/albertrodriguezdev/hello-world-web)

---

A lightweight Docker HTTP web server container exposing port 8080 and returning a simple "Hello World" response.

Ideal as a simple Docker example image, lightweight HTTP test container, or minimal web server for demos and workshops.

No configuration required — just run and open your browser.

## ✨ What is hello-world-web?

`hello-world-web` is a tiny containerized web server that:

- Exposes port `8080`
- Returns: `Hello World from Docker! 🚀`

It is intentionally small, predictable, and easy to run in any Docker environment.

Works out of the box with Docker Desktop and any modern Docker installation.

---

## ⚡ Run from Docker Hub

Use the prebuilt image published on Docker Hub.

### 🚀 Using Docker Compose (recommended)

Clone this repository and run:

```bash
docker compose up
```

Then open:

http://localhost:8080

Stop with:

```bash
Ctrl + C
```

### 🐳 Using Docker (alternative)

```bash
docker run -p 8080:8080 albertrodriguezdev/hello-world-web
```

To use a different host port:

```bash
docker run -p 3000:8080 albertrodriguezdev/hello-world-web
```

Then open in your browser:

- `http://localhost:8080` (default port mapping: `-p 8080:8080`)
- `http://localhost:3000` (if you used `-p 3000:8080`)

Stop with:

```bash
Ctrl + C
```

## 🛠 Run locally from source (advanced)

Build the image:

```bash
docker build -t hello-world-web .
```

Run the container:

```bash
docker run -p 8080:8080 hello-world-web
```

To use a different host port:

```bash
docker run -p 3000:8080 hello-world-web
```

Then open in your browser:

- `http://localhost:8080` (default port mapping: `-p 8080:8080`)
- `http://localhost:3000` (if you used `-p 3000:8080`)

Stop with:

```bash
Ctrl + C
```

## ✅ Example

```bash
curl http://localhost:8080
```

Response:

```
Hello World from Docker! 🚀
```

## 📁 Project structure

```
.
├── Dockerfile
├── docker-compose.yml
├── app.py
├── LICENSE
└── README.md
```

## 🧩 File overview

### Dockerfile
Defines how the image is built and how the server starts.

### docker-compose.yml
Defines the local service configuration and port publishing.

### app.py
Minimal Flask-based HTTP server returning `"Hello World"`.

---

Simple, predictable, and ready to use.
