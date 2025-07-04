# 🐳 Node.js Microservices Docker Demo

This is a simple microservices-based demo application built with **Node.js**, containerized using **Docker** and orchestrated with **Docker Compose**. It includes multiple services such as:

- 📚 `book-service` – Manages book data
- 💰 `loan-service` – Handles book loans
- 🌐 `nginx` – Acts as a reverse proxy for routing traffic to services

Each service runs in its own container, ensuring isolation and scalability for easier development, testing, and deployment.

---

## 🧱 Tech Stack

- **Node.js** – Backend framework
- **Nginx** – Reverse proxy for load balancing and routing
- **Docker** – Containerization
- **Docker Compose** – Multi-container orchestration
---

## 🚀 Getting Started

### 1. Clone the repository
git clone <your-repository-url>
cd <your-repository-folder>

### 2. Build and run the services
docker-compose up --build
