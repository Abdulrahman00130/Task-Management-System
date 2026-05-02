# 🚀 Task Management & Team Collaboration System

A production-grade, full-stack web application designed for comprehensive team collaboration, task tracking, and real-time communication. Built with a focus on clean architecture, scalability, and high performance.

## 🌟 Key Features

### 👥 Team & Role Management
* **Workspaces:** Users can create dedicated teams and automatically become Team Admins.
* **Role-Based Access Control (RBAC):** Admins can assign specific roles and authorities to team members.
* **Delegation:** Authorized members can assign tasks to individuals or groups within the team.
* **Individual Tasking:** Individual users can create tasks for themselves (self-assigned tasks).

### ✅ Advanced Task Tracking
* **Comprehensive Details:** Track tasks by Title, Description, Due Date, Status, and Priority.
* **Task Extensions:** When a task is past due, assigned users must submit a reason/excuse. Admins can review and grant time extensions (marked clearly as "Extended past due").
* **Time Tracking:** Integrated start/pause/stop timer for each task to accurately calculate the actual time spent by developers.

### 💬 Real-Time Communication (SignalR)
* **Threaded Task Chats:** Every task has an isolated, threaded chat environment to keep context clear.
* **Pacing Control:** Implemented "Slow Mode" (e.g., 30-minute intervals between messages per user) to reduce noise and encourage thoughtful communication.
* **Live Notifications:** Instant updates for new assignments, status changes, approaching deadlines (24h/half-date), and overdue alerts.

### 📊 Dashboard & Analytics
* **Unified View:** Personalized dashboard displaying upcoming, in-progress, and overdue tasks.
* **Advanced Filtering & Search:** Filter by status, priority, or dates. Deep search across titles, descriptions, and assigners.
* **Calendar View:** Visual representation of task deadlines and timelines.

## 🛠️ Technology Stack

* **Backend:** ASP.NET Core Web API, C#
* **Frontend:** ASP.NET Core MVC (or integrated SPA)
* **Database & ORM:** SQL Server, Entity Framework Core (Code First)
* **Security:** ASP.NET Core Identity, JWT Authentication
* **Real-Time Engine:** SignalR
* **Performance:** In-Memory Caching (Redis integration planned)

## 🏗️ System Architecture

This project is structured around **Clean Architecture** principles to ensure separation of concerns, testability, and maintainability:
* **Presentation Layer:** RESTful APIs and MVC Controllers.
* **Application Layer:** Business logic, DTOs, and Interfaces.
* **Domain Layer:** Enterprise entities and core business rules.
* **Infrastructure Layer:** Database context, Repositories, and External services.

## 🔌 API Endpoints Overview
The system provides a robust RESTful API. Key endpoint categories include:
* `/api/auth/*` - Registration, Login, and Token management.
* `/api/tasks/*` - CRUD operations, status updates, and time-tracking triggers.
* `/api/teams/*` - Team creation, member invites, and role management.
* `/api/notifications/*` - SignalR hub endpoints for real-time data broadcasting.

## 🚀 Getting Started
*(Instructions on how to set up the project locally using Docker/CLI will be added here as the CI/CD pipeline is finalized.)*
