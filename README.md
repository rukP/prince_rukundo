# DevOps Express App

This is a simple Express.js application containerized using Docker and exposed via NGINX as a reverse proxy.

## 📁 Project Structure

```
devops_express_project/
├── app.js              # Express.js app
├── package.json        # Node.js dependencies
├── Dockerfile          # Dockerfile for Express app
├── nginx.conf          # NGINX reverse proxy configuration
└── docker-compose.yml  # Orchestrates app and NGINX containers
```

## ✅ Prerequisites

- Docker: https://docs.docker.com/get-docker/
- Docker Compose (included with Docker Desktop)
- Terminal or command prompt

## 🚀 How to Run the Project

### 1. Navigate to the project directory

```bash
cd path/to/devops_express_project
```

### 2. Build and start the containers

```bash
docker-compose up --build
```

### 3. Access the application

- In your browser: [http://localhost](http://localhost)
- Or use curl:

```bash
curl http://localhost
```

You should see:

```
Hello, DevOps!
```

## 🧪 Verify It's Working

Check running containers:

```bash
docker ps
```

Check logs:

```bash
docker-compose logs express-app
docker-compose logs nginx
```

## 🛑 Stop the App

- Press `Ctrl + C` to stop
- Or run:

```bash
docker-compose down
```

## 📌 Troubleshooting

- Ensure port 80 is free.
- Restart Docker if issues persist.
- Check logs for errors using `docker-compose logs`.

---