# Virtual Education Institute (VEI) Management System

A full-stack **Database Management Systems (DBMS)** semester project for FAST-NUCES that models and manages the academic operations of a virtual education institute.

## Overview

VEI is a database-driven management system covering students, teachers, courses, registrations, enrollments, attendance, sibling relationships, and course posts. The project combines relational database design with a JavaScript web backend and frontend interface.

## Features

- Student and teacher management
- Course and enrollment management
- Student registration and approval workflows
- Attendance tracking and automated attendance calculations
- Sibling relationship management
- Course posts and academic information
- Relational integrity using primary/foreign keys and constraints
- REST-style backend endpoints
- Database triggers and procedures for automated workflows

## Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Node.js, Express.js |
| Database | PostgreSQL / Supabase |
| Database Client | `@supabase/supabase-js` |
| Supporting Tools | Git, GitHub, dotenv, CORS |

## Database Design

The system follows a relational model with interconnected entities for students, teachers, courses, registrations, enrollments, attendance, siblings, and course posts. Foreign keys and constraints maintain referential integrity, while database-side automation handles recurring business rules.

```text
Students ── Registrations ── Courses ── Teachers
    │              │
    ├── Siblings   └── Enrollments ── Attendance
    │
    └── Student Profile

Courses ── Course Posts
```

## Architecture

The web application communicates with an Express.js backend, which interacts with the PostgreSQL database through Supabase. Environment variables are used for database configuration, keeping credentials outside the source code.

## Getting Started

```bash
git clone https://github.com/Mahad-Khan-14/DBMS_AI_PROJECT_REPO.git
cd DBMS_AI_PROJECT_REPO
npm install
```

Create a `.env` file with the required Supabase configuration, then start the project's configured Node.js entry point.

```env
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
```

## Academic Context

**Course:** Database Management Systems  
**Semester:** Spring 2026  
**Institution:** FAST-NUCES, Karachi

## Contributors

- **Muhammad Mahad Khan** — 24K-0961
- **Muhammad Samad Siddiqui** — 24K-1039
- **Muhammad Shahbaz Hassan** — 24K-0884

## Learning Outcomes

This project demonstrates practical experience with relational schema design, database constraints, SQL, triggers, stored procedures, CRUD operations, backend API development, and database-driven web applications.
