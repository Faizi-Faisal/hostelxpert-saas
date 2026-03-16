# HostelXpert SaaS Platform

HostelXpert is enterprise SaaS platform for managing hostel operations including property management, student lifecycle, mess management, accounting systems, and operational workflows.

**Note**
The production source code for this system is maintained in a **private company repository** and cannot be shared publicly due to company confidentiality policies.
This repository highlights the **system architecture, feature design, and technology stack** used in the platform.

---

# Platform Overview

Managing hostels at scale requires handling multiple operational layers:

* Property administration
* Student management
* Employee operations
* Payroll Generation
* Attendence Management
* Leave Management
* Mess operations
* Inventory management
* Asset Management
* Financial accounting
* Complaint and maintenance management

HostelXpert centralizes these operations into a **single SaaS platform**, enabling hostel operators to manage **multiple hostels and thousands of students efficiently**.

---

# My Contribution

Key areas I worked on:

* SaaS backend system architecture
* REST API development
* Microservice-based system modules
* Real-time event communication using WebSockets
* Secure authentication using JWT
* Scalable service deployment using Docker
* API integration across multiple operational modules

---

# System Architecture

High-level architecture of the HostelXpert SaaS platform:

```
                    ┌─────────────────────┐
                    │   React Admin Panel │
                    │   (Frontend UI)     │
                    └─────────┬───────────┘
                              │
                              │ REST API
                              ▼
                    ┌─────────────────────┐
                    │   API Gateway       │
                    │   Express Server    │
                    └─────────┬───────────┘
                              │
          ┌───────────────────┼───────────────────┐
          │                   │                   │
          ▼                   ▼                   ▼
 ┌──────────────┐   ┌────────────────┐   ┌─────────────────┐
 │ Auth Service │   │ Core Services  │   │ Financial       │
 │ JWT Security │   │ Management     │   │ Accounting      │
 └──────┬───────┘   └───────┬────────┘   └────────┬────────┘
        │                   │                     │
        ▼                   ▼                     ▼
 ┌─────────────┐    ┌─────────────┐       ┌──────────────┐
 │ Redis Cache │    │ WebSocket   │       │ MongoDB      │
 │ Session     │    │ Real-Time   │       │ Database     │
 └─────────────┘    └─────────────┘       └──────────────┘
                              │
                              ▼
                      Dockerized Services
```

### Infrastructure Components

* Containerized services using **Docker**
* Distributed microservice architecture
* Redis caching layer
* Real-time updates using WebSockets
* RESTful API communication

---

# Technology Stack

### Frontend

* React.js
* Tailwind CSS

### Backend

* Node.js
* Express.js

### Database

* MongoDB

### Architecture

* Microservices Architecture
* SaaS Multi-tenant Architecture

### Infrastructure

* Docker Containerization
* Redis Caching

### Security

* JWT Authentication
* Secure API Authorization

### Communication

* REST APIs
* WebSocket Real-time Events

### Development Tools

* Git Version Control
* API Integration (180+ APIs across modules)

---

# Platform Modules

### Client Management
Manage multiple hostel clients and organizational data.

### Property Management
Support for managing **multiple hostel properties** within a single system.

### Floor & Room Management
Complete infrastructure mapping including:

* Floors
* Rooms
* Bed allocations

### Student Management
Handles full **student lifecycle operations**.

* Student registration
* Room allocation
* Student status management
* Fee management

### Employee Management
Staff record management including roles, responsibilities, Salary Management.

### Attendance Management
Track student and employee attendance across properties.

### Leave Management
Digital leave request and approval workflow.

### Mess Management
Daily mess operations including:

* Meal planning
* Meal Booking
* Mess usage tracking
* Meal Collecting QR

### Mess Booking
Manage student mess booking records and consumption tracking.

### Inventory Management
Track hostel inventory including supplies and consumables.

### Complaint & Maintenance Allocation
Maintenance issue tracking with assignment workflows.

### Onboard / Offboard Request Management
Automated workflows for:

* Student onboarding
* Student offboarding

### Asset Management
Track hostel assets including equipment and infrastructure.

### Accounts Management
Financial management system integrated into the platform with accountant page.

### Profit & Loss Tracker
Real-time financial analytics for hostel operations.

### Journal Entries
Accounting ledger system for financial records.

### Trial Balance Sheet
Financial summary reports.

### Expense Manager
Track operational expenses across hostel properties.

---

# Platform Capabilities

The system supports:

* Multi-property hostel management
* Scalable SaaS infrastructure
* Real-time operational updates
* Financial analytics and accounting workflows
* Operational automation

---

#  Source Code Availability

This project was developed as part of a **company product**.
Due to internal policies, the **production source code is private** and maintained in a restricted repository.

This repository exists to showcase:

* System architecture
* Product design
* Platform capabilities
* My development contributions

---

# Contact
If you'd like to discuss this system or my development work:

GitHub: https://github.com/Faizi-Faisal
LinkedIn: https://linkedin.com/in/faisalvahab
