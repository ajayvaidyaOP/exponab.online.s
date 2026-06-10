# Exponab Invoice & Agreement Management System

## Overview

Exponab Invoice & Agreement Management System is a web-based business management platform designed to manage invoices, agreements, user accounts, pricing information, and related business operations efficiently.

The application is built using a modern full-stack architecture with React, Spring Boot, and MySQL.

---

## Live Application

Frontend:
https://exponab.online

Backend API:
https://exponab.online/api

---

## Technology Stack

### Frontend

* React.js
* TypeScript
* Vite
* Tailwind CSS
* Axios

### Backend

* Java 21
* Spring Boot 3
* Spring Security
* Spring Data JPA
* JWT Authentication

### Database

* MySQL 8

### Deployment

* Ubuntu Server
* Nginx Reverse Proxy
* SSL/TLS (HTTPS)
* Git & GitHub

---

## Features

### Authentication

* Secure Login System
* JWT Based Authentication
* Role-Based Access Control

### User Management

* Create Users
* Update User Information
* Manage User Roles

### Invoice Management

* Create Invoices
* Manage Invoice Records
* PDF Generation

### Agreement Management

* Create Agreements
* Store Agreement Data
* Agreement Tracking

### Pricing Management

* Product Pricing
* Price List Management
* Dynamic Updates

### Document Management

* Upload Documents
* Download Documents
* PDF Support

---

## Project Structure

```text
Frontend (React + Vite)
│
├── Components
├── Pages
├── Services
├── Context
└── Assets

Backend (Spring Boot)
│
├── Controllers
├── Services
├── Repositories
├── Entities
├── Security
└── Configuration
```

---

## Environment Configuration

### Backend

application.properties

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/exponab
spring.datasource.username=exponab
spring.datasource.password=********

server.port=8080

jwt.secret=********
jwt.expiration=86400000
```

---

## Local Setup

### Clone Repository

```bash
git clone <repository-url>
```

### Backend

```bash
cd backend

chmod +x gradlew

./gradlew clean build

java -jar build/libs/invoice-0.0.1-SNAPSHOT.jar
```

### Frontend

```bash
cd frontend

npm install

npm run dev
```

---

## Production Deployment

### Frontend

```bash
npm run build

cp -r dist/* /var/www/exponab/
```

### Backend

```bash
java -jar build/libs/invoice-0.0.1-SNAPSHOT.jar
```

### Nginx

```nginx
location /api/ {
    proxy_pass http://localhost:8080/api/;
}
```

---

## Security

* HTTPS Enabled
* JWT Authentication
* Password Encryption
* Secure API Access
* CORS Configuration

---

## Monitoring & Maintenance

* Application Logs
* Nginx Logs
* MySQL Monitoring
* Server Health Monitoring

---

## Contributors

Exponab Development Team

---

## License

Private Internal Business Application.
All Rights Reserved.
