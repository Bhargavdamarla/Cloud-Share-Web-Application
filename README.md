# Cloud Share - SaaS File Sharing Platform

Cloud Share is a full-stack file-sharing application built with React, Spring Boot, and MongoDB. It enables users to securely upload, manage, and share files while supporting a credit-based subscription system integrated with Razorpay.

## Features

* User authentication and authorization
* File upload and management
* Public and private file sharing
* Credit-based subscription model
* Razorpay payment integration
* Responsive UI
* RESTful API architecture
* Centralized exception handling

---

## Tech Stack

### Frontend

* React.js
* Tailwind CSS
* Axios

### Backend

* Spring Boot
* Java
* REST APIs

### Database

* MongoDB

### Authentication

* Clerk

### Payment Gateway

* Razorpay

---

# System Architecture

```text
React Frontend
       ↓
Spring Boot REST APIs
       ↓
Service Layer
       ↓
Repository Layer
       ↓
MongoDB
```

The backend follows a layered architecture to ensure separation of concerns and maintainability.

---

# Backend Structure

```text
backend
│
├── controller
├── service
├── repository
├── dto
├── model
├── exception
├── config
└── util
```

---

# API Endpoints

## Authentication

| Method | Endpoint           | Description   |
| ------ | ------------------ | ------------- |
| POST   | /api/auth/login    | Login user    |
| POST   | /api/auth/register | Register user |

## File Management

| Method | Endpoint          | Description         |
| ------ | ----------------- | ------------------- |
| POST   | /api/files/upload | Upload file         |
| GET    | /api/files        | Retrieve user files |
| DELETE | /api/files/{id}   | Delete file         |
| GET    | /api/files/{id}   | Get file details    |

## Payment APIs

| Method | Endpoint                  | Description           |
| ------ | ------------------------- | --------------------- |
| POST   | /api/payment/create-order | Create Razorpay order |
| POST   | /api/payment/verify       | Verify payment        |

---

# Error Handling

The application uses centralized exception handling to provide meaningful error responses.

Examples:

* Invalid credentials
* Unauthorized access
* File not found
* Insufficient credits
* Payment verification failures

Sample Response:

```json
{
  "timestamp": "2026-06-23T10:30:00",
  "status": 404,
  "message": "File not found"
}
```

---

# Design Decisions

### Layered Architecture

The application follows Controller → Service → Repository architecture to improve readability and maintainability.

### DTO Pattern

DTOs are used to separate API contracts from database entities and avoid exposing internal models.

### Centralized Exception Handling

Custom exceptions and global handlers ensure consistent API responses.

### Authentication

Clerk manages user authentication and session handling.

### Payment Processing

Razorpay is integrated to support secure credit purchases.

---

# Learning Outcomes

This project helped me gain practical experience in:

* Building scalable REST APIs
* Layered architecture design
* MongoDB data modeling
* Exception handling and validation
* Third-party integrations
* Payment gateway implementation
* Frontend-backend communication
* Full-stack application development

---

# Future Improvements

* Folder support
* Search functionality
* Email sharing
* Admin dashboard
* Analytics and monitoring
* Docker support
* CI/CD pipelines



