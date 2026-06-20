# MITWPU CSE Connect

## Overview

MITWPU CSE Connect is a web-based department management system designed to centralize and manage information related to students, clubs, achievements, and departmental announcements. The platform provides a structured way to store, retrieve, and maintain departmental records through a single interface.

## Features

- JWT-based authentication with role-based access control (ADMIN, TEACHER, STUDENT)
- Student management with CRUD, bulk CSV import, academic records
- Teacher management with panel assignment
- Club management with membership tracking and notices
- Achievement submission and verification workflow
- Announcements with audience targeting
- Audit logging for all mutations
- Soft-delete pattern for data preservation
- Glassmorphism UI with responsive design
- Charts and analytics dashboards
- File upload support for achievement proofs

## Main Modules

### Student Management

* Add student records
* View student details
* Update student information
* Delete student records

### Club Management

* Create and manage clubs
* Maintain club member information
* Store club-related details and activities

### Achievement Management

* Record and manage student achievements
* Maintain achievement history
* Verify submitted achievements

### Announcements

* Create and publish department announcements
* Display important notices and updates

### Dashboard

* View key departmental information
* Access records from a centralized interface

---

## Technology Stack

### Backend

* Java 17
* Spring Boot
* Spring Data JPA
* Hibernate
* MySQL

### Frontend

* React
* Vite
* Tailwind CSS

### Tools

* Maven
* Git
* GitHub

### Database

The application uses MySQL to store and manage:

* Student Records
* Club Information
* Achievement Records
* Announcements

---
## System Architecture

React Frontend

↓

Spring Boot REST APIs

↓

JPA / Hibernate

↓

MySQL Database

---
## Setup

### 1. Database

```sql
CREATE DATABASE cse_connect;
```

### 2. Backend

```bash
cd backend
# Update database credentials in src/main/resources/application.properties if needed
mvn spring-boot:run
```

The backend starts on `http://localhost:8080`.

### 3. Frontend

```bash
cd frontend
npm install
npm run dev
```

The frontend starts on `http://localhost:5173`.

## Default Login Credentials

| Role    | Email                          | Password      |
|---------|--------------------------------|---------------|
| Admin   | admin@mitwpu.edu.in            | Admin@1234    |
| Teacher | sunita.sharma@mitwpu.edu.in    | Teacher@1234  |
| Student | ria.modak@mitwpu.edu.in        | Student@1234  |

---

