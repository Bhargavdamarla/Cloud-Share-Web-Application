# Cloud Share - SaaS File Sharing Platform

Cloud Share is a full-stack file sharing application that allows users to securely upload, manage, and share files. The platform includes authentication, subscription-based credits, and secure file access, providing a simple and scalable cloud storage experience.

## Overview

The goal of this project was to build a modern file-sharing platform with a clean user experience and secure backend architecture. Users can upload files, manage their storage, and control file visibility while using a credit-based system for premium features.

## Features

- Secure user authentication and session management
- Upload and manage files
- Public and private file sharing
- Credit-based subscription model
- Razorpay payment integration
- User dashboard for managing uploads
- Responsive and user-friendly interface
- RESTful backend APIs

## Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Axios

### Backend
- Spring Boot
- Java
- REST APIs

### Database
- MongoDB

### Authentication
- Clerk

### Payment Gateway
- Razorpay

## Architecture

```text
Client (React)
       ↓
Spring Boot REST APIs
       ↓
MongoDB Database
       ↓
Clerk Authentication
       ↓
Razorpay Payment Services
```

## Project Structure

```text
Cloud-Share-Web-Application
│
├── frontend
│
├── backend
│
├── README.md
│
└── .env
```

## Key Functionalities

### User Authentication
- Sign up and login
- Session management
- Protected routes

### File Management
- Upload files
- Delete files
- View uploaded files
- Share files securely
- Public and private access control

### Subscription System
- Purchase credits
- Razorpay integration
- Credit usage tracking

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/Bhargavdamarla/Cloud-Share-Web-Application.git
```

### Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

### Backend Setup

```bash
cd backend

./mvnw spring-boot:run
```

## Environment Variables

### Frontend

```env
VITE_CLERK_PUBLISHABLE_KEY=
```

### Backend

```env
MONGODB_URI=
RAZORPAY_KEY_ID=
RAZORPAY_SECRET=
```

## Future Improvements

- Folder organization support
- Drag-and-drop uploads
- Email sharing
- Search and filtering
- Cloud storage integration
- Admin dashboard
- File analytics and usage tracking

## Learning Outcomes

Through this project, I gained practical experience in:

- Building full-stack applications with React and Spring Boot
- Designing REST APIs
- Working with MongoDB and NoSQL databases
- Implementing authentication and authorization
- Integrating third-party payment gateways
- Managing client-server communication
- Deploying and maintaining scalable applications
