# 🎬 AI Video SaaS Platform

An AI-powered video generation platform built with **ASP.NET Core**, **Next.js**, and **Clean Architecture**.

Users can generate AI videos such as **Face Swap**, **Talking Photo**, and **Text-to-Video**, manage credits, purchase subscriptions, and track video generation history.

---

# ✨ Features

* 🔐 JWT Authentication & Refresh Token
* 👤 User Profile Management
* 🎥 Face Swap
* 🗣️ Talking Photo
* 🎬 Text-to-Video
* 💳 Stripe & Iyzico Payments
* 💰 Credit System
* 📜 Video History
* ⚡ Real-time Notifications (SignalR)
* ☁️ Cloudflare R2 Storage
* 🔄 AI Provider Factory (Replicate, Fal, Runway, Kling)
* 🐳 Docker Support
* 🧪 Unit & Integration Tests

---

# 🛠 Tech Stack

## Frontend

* Next.js 15
* React
* TypeScript
* Tailwind CSS
* TanStack Query
* Axios
* SignalR Client

## Backend

* ASP.NET Core
* C#
* Entity Framework Core
* Clean Architecture
* CQRS
* MediatR
* FluentValidation
* SignalR
* Serilog

## Database & Infrastructure

* SQL Server
* Redis
* Cloudflare R2
* Docker
* Nginx

## AI Providers

* Replicate
* Fal AI
* Runway
* Kling

---

# 📁 Project Structure

```text
ai-video-saas-platform
│
├── frontend
│   ├── src
│   │   ├── app
│   │   ├── components
│   │   ├── hooks
│   │   ├── services
│   │   ├── context
│   │   ├── lib
│   │   ├── schemas
│   │   ├── constants
│   │   └── types
│
├── backend
│   ├── SASS.WebApi
│   ├── SASS.Application
│   ├── SASS.Domain
│   ├── SASS.Infrastructure
│   └── Tests
│
├── deployment
├── docs
└── docker-compose.yml
```

---

# 🏗 Architecture

```text
Next.js
      │
      ▼
ASP.NET Core Web API
      │
      ├────────► SQL Server
      ├────────► Redis
      ├────────► SignalR
      ├────────► Cloudflare R2
      ├────────► Stripe / Iyzico
      └────────► AI Provider Factory
                     │
      ┌──────────────┼──────────────┐
      ▼              ▼              ▼
 Replicate        Fal AI         Runway
                                   │
                                   ▼
                                Kling
```

---

# 📦 Backend Layers

## SASS.WebApi

* Controllers
* Middleware
* SignalR Hubs
* API Configuration

## SASS.Application

* CQRS
* Commands
* Queries
* DTOs
* Validators
* Interfaces

## SASS.Domain

* Entities
* Enums
* Value Objects
* Domain Events
* Specifications

## SASS.Infrastructure

* Entity Framework Core
* Authentication
* AI Providers
* Payments
* Redis Cache
* Background Jobs
* Storage

---

# 🚀 Getting Started

## Clone Repository

```bash
git clone https://github.com/yourusername/ai-video-saas-platform.git
```

## Backend

```bash
cd backend
dotnet restore
dotnet run
```

## Frontend

```bash
cd frontend
npm install
npm run dev
```

---

# 🐳 Docker

```bash
docker-compose up -d
```

---

# 📌 Roadmap

* [ ] AI Image Generation
* [ ] AI Voice Cloning
* [ ] Team Workspace
* [ ] Admin Dashboard
* [ ] Analytics
* [ ] Subscription Plans
* [ ] Mobile Responsive Dashboard
* [ ] Multi-language Support

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Ömer Faruk Gülden**

Computer Engineering Student

Backend Developer (.NET)

AI & SaaS Enthusiast
