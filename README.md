# 🚀 Inventory Management System

A backend inventory management system built using **Spring Boot, PostgreSQL, and Docker**, designed to simulate real-world backend architecture and deployment.

---

## 🛠️ Tech Stack

* Java 17
* Spring Boot
* Spring Data JPA
* PostgreSQL
* Docker & Docker Compose
* REST APIs
* Maven

---

## ✨ Features

* Create, update, delete, and retrieve products
* RESTful API design
* Layered architecture (Controller, Service, Repository)
* PostgreSQL integration using JPA
* Dockerized backend application
* Containerized database using Docker Compose

---

## 📡 API Endpoints

| Method | Endpoint           | Description       |
| ------ | ------------------ | ----------------- |
| GET    | /api/products      | Get all products  |
| GET    | /api/products/{id} | Get product by ID |
| POST   | /api/products      | Create product    |
| PUT    | /api/products/{id} | Update product    |
| DELETE | /api/products/{id} | Delete product    |

---

## 🧪 Sample Request

```json
{
  "name": "Laptop",
  "category": "Electronics",
  "quantity": 10,
  "price": 899.99
}
```

---

## 🐳 Run with Docker (Recommended)

```bash
docker-compose up --build
```

Access API:
http://localhost:8081/api/products

---

## ⚙️ Run Locally

```bash
mvn spring-boot:run
```

---

## 📦 Build JAR

```bash
mvn clean package
```

---

## 🔮 Future Improvements

* Low stock alert system
* Search and filtering APIs
* Pagination
* Authentication & authorization
* Cloud deployment (GCP / AWS)

---

## 💡 Key Learnings

* Docker container networking
* Backend architecture design
* Database integration with JPA
* Environment-based configuration
