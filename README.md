
# CRUD App (Dockerized 3-Tier Architecture)

A fully Dockerized **3-tier CRUD application** with:
- **PostgreSQL** database
- **Node.js** backend API
- **React** frontend

This project demonstrates containerized deployment using **Docker Compose**, making it easy to set up and run anywhere.

---

## 🚀 Tech Stack
- **Frontend:** React
- **Backend:** Node.js + Express
- **Database:** PostgreSQL
- **Containerization:** Docker & Docker Compose

---

## 📂 Folder Structure

crud-app/</br>
├── database/</br>
│ └── init.sql # Database initialization script
├── docker-compose.yml # Docker Compose configuration

---

## 🛠 Prerequisites
Make sure you have installed:
- Latest docker version
- Do not have any containers running on port 5000,5500,5432

---

## ⚡ Running the Application

1. **Clone the repository**
git clone https://github.com/abhuu123/crud-app.git
cd crud-app

Start the containers

docker-compose up -d

Access the app

Frontend: http://instance-ip:5500


🛑 Stopping the Application
docker-compose down
📦 Useful Commands

View running containers:
docker ps

View logs:
docker-compose logs -f

Remove all containers:
docker rm -f $(docker ps -aq)

📌 Notes
The database will be preloaded with data from database/init.sql.

Environment variables are set in docker-compose.yml.

Uses app-network Docker bridge for internal service communication.
