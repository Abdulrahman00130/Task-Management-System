# Task Management System

> A production-grade task management API built with ASP.NET Core, demonstrating Clean Architecture, CQRS, JWT auth, SignalR, Redis caching, and comprehensive testing.

## 🌟 Project Overview
A robust web application designed for comprehensive team collaboration, task tracking, and real-time communication. Built with a strict focus on scalability, high performance, and enterprise-level engineering principles.

## 🏗️ Architecture

> *[Clean Architecture diagram — Placeholder]*
> 
> *(Detailed explanation of the architectural decisions, layers, and patterns like CQRS and Unit of Work will be documented here after thorough research and implementation.)*

## 🛠️ Tech Stack
- **Backend Framework:** ASP.NET Core 8 Web API
- **Database & ORM:** Entity Framework Core + SQL Server
- **Security:** ASP.NET Core Identity + JWT Authentication
- **Real-Time & Background Jobs:** SignalR, Hangfire
- **Caching & Performance:** Redis
- **DevOps & Infrastructure:** Docker, Nginx, GitHub Actions
- **Testing & Load Profiling:** xUnit, Moq, k6, JMeter

## 🚀 Key Features

### 👥 Team & Role Management
* **Workspaces:** Users can create dedicated teams and automatically become Team Admins.
* **Role-Based Access Control (RBAC):** Admins can assign specific roles and authorities to team members.
* **Delegation:** Authorized members can assign tasks to individuals or groups within the team.

### ✅ Advanced Task Tracking
* **Comprehensive Details:** Track tasks by Title, Description, Due Date, Status, and Priority.
* **Task Extensions:** When a task is past due, assigned users must submit a reason/excuse. Admins can review and grant time extensions (marked clearly as "Extended past due").
* **Time Tracking:** Integrated start/pause/stop timer for each task to accurately calculate the actual time spent by developers.

### 💬 Real-Time Communication
* **Threaded Task Chats:** Every task has an isolated, threaded chat environment to keep context clear.
* **Pacing Control:** Implemented "Slow Mode" (e.g., 30-minute intervals between messages per user) to reduce noise and encourage thoughtful communication.
* **Live Notifications:** Instant updates via SignalR for new assignments, status changes, approaching deadlines (24h/half-date), and overdue alerts.

### 📊 Dashboard & Analytics
* **Unified View:** Personalized dashboard displaying upcoming, in-progress, and overdue tasks.
* **Advanced Filtering & Search:** Filter by status, priority, or dates. Deep search across titles, descriptions, and assigners.
* **Calendar View:** Visual representation of task deadlines and timelines.

## 🔌 API Endpoints Overview
The system provides a robust RESTful API. Key endpoint categories include:
* `/api/auth/*` - Registration, Login, and Token management.
* `/api/tasks/*` - CRUD operations, status updates, and time-tracking triggers.
* `/api/teams/*` - Team creation, member invites, and role management.
* `/api/notifications/*` - SignalR hub endpoints for real-time data broadcasting.

## 🚀 Getting Started
*(Instructions on how to set up the project locally using Docker/CLI will be added here as the CI/CD pipeline is finalized.)*
