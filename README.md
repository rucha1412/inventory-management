# Inventory Management System

A backend inventory management application built with Spring Boot, PostgreSQL, and Docker.

## Tech Stack
- Java
- Spring Boot
- Spring Data JPA
- PostgreSQL
- Docker

## Features
- Create product
- Get all products
- Get product by id
- Update product
- Delete product
- Persistent storage using PostgreSQL
- Dockerized backend setup

## API Endpoints
- `GET /api/products`
- `GET /api/products/{id}`
- `POST /api/products`
- `PUT /api/products/{id}`
- `DELETE /api/products/{id}`

## Example Request
```json
{
  "name": "Laptop",
  "category": "Electronics",
  "quantity": 10,
  "price": 899.99
}
```
## Run Locally

### Prerequisites
- Java 17+
- Maven
- PostgreSQL

### Steps

1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/inventory-management-system.git
cd inventory-management-system
```
2. Configure database in application.properties
```
spring.datasource.url=jdbc:postgresql://localhost:5432/inventorydb1
spring.datasource.username=postgres
spring.datasource.password=your_passwordagsl

```
3. Run the application
```
mvn spring-boot:run
```

4. Access API
```
http://localhost:8080/api/products
```

---

## ⚙️ Build JAR

```markdown
## Build JAR

To package the application into a JAR file:

```bash
mvn clean package
```
The JAR will be generated in:

```agsl
target/inventory-management-0.0.1-SNAPSHOT.jar
```

---

## 🐳 Run with Docker

```markdown
## Run with Docker

### Build Docker Image
```bash
docker build -t inventory-management-app .

```
Run Container
```agsl
docker run -p 8081:8080 inventory-management-app
```
Access API:
```agsl
http://localhost:8081/api/products
```

---

## 🐳 Docker Compose (BEST PART 🔥)

```markdown
## Run with Docker Compose

Run both backend and PostgreSQL:

```bash
docker-compose up --build
```
Access API:
```agsl
http://localhost:8081/api/products
```
