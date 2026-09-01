# MERN Stack Docker Boilerplate

A production-ready boilerplate for containerizing a full-stack **MERN** (MongoDB, Express.js, React.js, Node.js) application using **Docker** and **Docker Compose**. This setup streamlines the development workflow by ensuring environment consistency across different machines.

## 🚀 Features

- **Multi-Container Architecture:** Separate containers for Frontend, Backend, and Database.
- **Hot Reloading:** Docker volumes are configured for local development to reflect code changes instantly.
- **Environment Management:** Centralized configuration using environment variables.
- **Orchestration:** Single-command setup to build and run the entire ecosystem.

## 📂 Project Structure

```text
├── backend/            # Node.js & Express server source code
├── frontend/           # React.js client-side application
├── env/                # Environment configuration files (.env)
└── docker-compose.yaml # Docker Compose configuration file
```

## 🛠️ Prerequisites

Before running this project, ensure you have the following installed:
- [Docker Desktop](https://docker.com)
- [Docker Compose](https://docker.com)

## 🏁 Getting Started

Follow these steps to get the application up and running locally:

### 1. Clone the Repository
```bash
git clone https://github.com
cd mern-docker
```

### 2. Configure Environment Variables
Navigate to the `env/` directory and set up your environment variables for both frontend and backend (e.g., database URIs, ports, API keys).

### 3. Build and Run the Containers
Run the following command in the root directory to build the images and start the services:
```bash
docker compose up --build
```

Once the build is complete, you can access the applications via your browser (typically `http://localhost:3000` for frontend and `http://localhost:5000` for backend, depending on your custom configuration).

### 4. Stopping the Application
To stop and remove the containers, networks, and volumes created by compose, use:
```bash
docker compose down
```

## 🏷️ Keywords
`docker` `docker-compose` `nodejs` `react` `mern-stack`
