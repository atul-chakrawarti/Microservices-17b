# Microservices-17b

# Dockerized Microservices Application

## Objective
To containerize a Node.js microservices application using Docker and Docker Compose.

## Services

| Service | Port | Description |
|---|---:|---|
| User Service | 3000 | User API |
| Product Service | 3001 | Product API |
| Order Service | 3002 | Order API |
| Gateway Service | 3003 | API Gateway |

## Technologies Used
- Node.js
- Express.js
- Docker
- Docker Compose

## Project Structure
- `user-service/`
- `product-service/`
- `order-service/`
- `gateway-service/`
- `docker-compose.yml`

## How to Run

```bash
docker compose up --build -d
```

## Verify Containers

```bash
docker compose ps
```

## Health Check URLs
- http://localhost:3000/health
- http://localhost:3001/health
- http://localhost:3002/health
- http://localhost:3003/health

## Gateway API URLs
- http://localhost:3003/api/users
- http://localhost:3003/api/products
- http://localhost:3003/api/orders

## Stop Services

```bash
docker compose down
```
