# Poll Application

The aim of the project was to deploy a poll app using docker and compose

![docker logo](https://d1.awsstatic.com/acs/characters/Logos/Docker-Logo_Horizontel_279x131.b8a5c41e56b77706656d61080f6a0217a3ba356d.png)

A modern polling application built with Docker and Docker Compose, featuring a distributed architecture with Redis and PostgreSQL.

## 🛠️ Prerequisites

- Docker version 20 or higher
- Docker Compose

## ⚙️ Environment Setup

Create a `.env` file at the root of the project with the following variables:

```env
POSTGRES_HOST=db
POSTGRES_PORT=5432
POSTGRES_USER=postgres
POSTGRES_PASSWORD=password
POSTGRES_DB=postgres
REDIS_HOST=redis
```

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/LucasMarsala/T-DOP-601-Popeye.git
cd T-DOP-601-Popeye
```

2. Build and start the containers:
```bash
docker compose up --build
```

## 📁 Project Structure

```
.
├── poll/           # Poll service implementation
├── result/         # Results service implementation
├── worker/         # Worker service implementation
├── compose.yml     # Docker Compose configuration
└── schema.sql      # Database schema
```

## 🛠️ Technologies Used

- JavaScript (91.3%)
- HTML (3.0%)
- CSS (2.6%)
- Java (1.8%)
- Other (1.3%)

## 🔧 Features

- Distributed polling system
- Real-time results
- Redis for caching
- PostgreSQL for data persistence
- Docker containerization
- Microservices architecture

## 📊 Architecture

The application consists of three main services:
- **Poll Service**: Handles poll creation and voting
- **Result Service**: Processes and displays voting results
- **Worker Service**: Manages background tasks and data processing

## 🔐 Security

- Environment variables for sensitive configuration
- Secure database connections
- Container isolation

## 🐳 Docker Components

- PostgreSQL database
- Redis cache
- Multiple service containers
- Docker Compose orchestration

---
⭐ Don't forget to star this repository if you found it useful!
