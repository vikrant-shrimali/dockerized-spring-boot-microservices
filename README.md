# Dockerized Spring Boot Microservices

A complete microservices architecture built with Spring Boot, containerized using Docker and Docker Compose. This project demonstrates a scalable, distributed system with service discovery, API gateway, and authentication patterns.

## 📋 Overview

This architecture consists of five core services:

| Service | Purpose | Features |
|---------|---------|----------|
| **micro-api-gateway** | API Gateway Service | Request routing, load balancing, centralized entry point |
| **micro-eureka-server** | Service Discovery | Service registration and discovery for microservices |
| **micro-auth-service** | Authorization Service | Authentication and authorization, dual database support |
| **micro-item-service** | Item/Resource Service | Manages item resources, dual database support |
| **micro-sales-service** | Sales/Resource Service | Manages sales operations, dual database support |

### Key Features

- ✅ Microservices architecture with Spring Boot
- ✅ Service discovery using Netflix Eureka
- ✅ API Gateway for centralized request handling
- ✅ Docker containerization for all services
- ✅ Docker Compose orchestration
- ✅ Support for both local and Docker database connections
- ✅ MySQL database integration

## 🛠️ Prerequisites

Before you begin, ensure you have the following tools installed:

| Tool | Version | Purpose |
|------|---------|---------|
| Maven | 3.0+ | Build tool |
| JDK | 1.8 or higher | Java runtime |
| Docker | 19.0+ | Container runtime |
| Docker Compose | 1.27.4+ | Orchestration tool |
| MySQL Server | Local or Docker | Database |

## 🚀 Quick Start

### Step 1: Build All Services

```bash
# Build the entire project with Maven
mvn clean install

# Or build individual services
cd micro-api-gateway && mvn clean install
cd ../micro-eureka-server && mvn clean install
cd ../micro-auth-service && mvn clean install
cd ../micro-item-service && mvn clean install
cd ../micro-sales-service && mvn clean install
