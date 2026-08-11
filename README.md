# Portfolio Platform

A **production-grade full-stack personal portfolio platform** built with Next.js, React, TypeScript, Node.js, Express, PostgreSQL, and Prisma. The platform is designed with a scalable architecture for presenting projects, managing content, providing authenticated administration, and supporting future AI-powered portfolio capabilities.

## 🚀 Overview

This project combines a modern frontend with a structured backend API and relational database.

```text
Portfolio Platform
│
├── frontend/
│   └── Next.js + React + TypeScript
│
├── backend/
│   └── Node.js + Express + TypeScript
│
├── backend/prisma/
│   └── Prisma schema + migrations + seed data
│
├── PostgreSQL
│   └── Application database
│
├── Redis
│   └── Caching / performance layer
│
└── Docker
    └── Local development orchestration
```

## ✨ Key Features

* Modern Next.js frontend
* React + TypeScript development
* Tailwind CSS styling
* SSR/SSG support
* Dynamic routing
* Theme system
* Performance optimizations
* Node.js + Express backend
* Clean architectural separation
* Versioned REST API
* PostgreSQL database
* Prisma ORM
* Redis caching support
* JWT authentication
* Refresh-token authentication
* Google OAuth support
* Role-based access control
* Admin/User roles
* Zod input validation
* API rate limiting
* Helmet security
* CORS configuration
* AI-powered service stubs
* AI content-generation foundation
* AI-powered search foundation
* Docker-based development environment
* CI/CD foundation
* ESLint configuration
* Prettier configuration
* Jest testing foundation

## 🏗️ Architecture

### Frontend

The `frontend/` application provides the user-facing portfolio experience.

Technologies include:

* Next.js
* React
* TypeScript
* Tailwind CSS
* Server-side rendering
* Static generation
* Dynamic routes

### Backend

The `backend/` application provides the API and business logic.

```text
Client
  │
  ▼
Next.js Frontend
  │
  ▼
REST API
/api/v1/...
  │
  ▼
Express Backend
  │
  ├── Authentication
  ├── Authorization
  ├── Validation
  ├── Business Logic
  ├── Logging
  └── Cache
       │
       ├── Redis
       │
       └── Prisma
             │
             ▼
         PostgreSQL
```

## 🔐 Security

The platform includes a foundation for secure production deployment:

* JWT authentication
* Refresh tokens
* Google OAuth
* Role-based authorization
* Zod request validation
* Rate limiting
* Helmet security headers
* CORS protection
* Environment-based secrets
* Protected API routes

> Production deployments should use properly configured secrets, HTTPS, secure cookies/tokens, OAuth credentials, database credentials, and infrastructure-level security controls.

## 🤖 AI Integration

The backend includes AI-oriented service stubs that can be extended with a real AI provider.

Potential capabilities include:

* Portfolio content generation
* Project description generation
* Semantic project search
* Intelligent portfolio discovery
* AI-assisted content management

The current architecture provides the foundation; a production AI provider still needs to be configured.

## 🗄️ Database

The project uses:

**PostgreSQL + Prisma**

Prisma is responsible for:

* Database schema
* Type-safe database access
* Migrations
* Seed data
* Application data modeling

Database-related files are located in:

```text
backend/prisma/
```

## ⚡ Redis

Redis provides a foundation for:

* API caching
* Frequently accessed data
* Performance optimization
* Future session or temporary-data workflows

## 🐳 Docker

Docker Compose is provided for local development.

The orchestration includes:

```text
PostgreSQL
Redis
Backend
Frontend
```

Start the development environment according to the repository's Docker configuration.

## 📁 Project Structure

```text
portfolio-platform/
│
├── frontend/
│   ├── app/
│   ├── components/
│   ├── public/
│   └── ...
│
├── backend/
│   ├── src/
│   ├── prisma/
│   │   ├── schema.prisma
│   │   ├── migrations/
│   │   └── seed/
│   └── ...
│
├── docker-compose.yml
├── package.json
├── .env.example
└── README.md
```

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd <repository-directory>
```

### 2. Configure Environment Variables

Copy the backend environment template:

```bash
cd backend
cp .env.example .env
```

On Windows PowerShell, you can use:

```powershell
Copy-Item .env.example .env
```

Configure the required values in `.env`.

### 3. Install Dependencies

From the repository root:

```powershell
npm.cmd run install:all
```

Or, in a shell where `npm` is available:

```bash
npm run install:all
```

### 4. Start Development

```powershell
npm.cmd run dev
```

Or:

```bash
npm run dev
```

### 5. Database & Redis

For the complete backend functionality, start:

* PostgreSQL
* Redis

Then run the required Prisma migrations from the `backend` directory.

Example:

```bash
npx prisma migrate dev
```

## 🧪 Testing

The project includes a Jest testing foundation.

Run the available test suite using the repository's configured test script.

```bash
npm test
```

## 🧹 Code Quality

The project includes:

* ESLint
* Prettier
* TypeScript
* Jest

Recommended workflow:

```text
Write Code
   ↓
Type Check
   ↓
Lint
   ↓
Format
   ↓
Test
   ↓
Build
```

## 🔄 API Versioning

Backend routes are versioned using:

```text
/api/v1/...
```

This allows future API versions to be introduced without unnecessarily breaking existing clients.

## 📊 Production Readiness

The architecture is designed with production-oriented principles:

* Separation of concerns
* API versioning
* Authentication
* Authorization
* Validation
* Database abstraction
* Caching
* Security middleware
* Testing foundation
* Containerization
* CI/CD foundation

However, production deployment still requires environment-specific configuration, security review, monitoring, real OAuth credentials, production secrets, and infrastructure configuration.

## 🔮 Future Improvements

Potential next steps include:

* Connect the frontend to all backend APIs
* Implement production OAuth credentials
* Integrate a real AI provider
* Implement semantic search
* Add portfolio analytics
* Add monitoring and observability
* Add automated deployment
* Expand automated tests
* Add comprehensive API documentation
* Add admin dashboard functionality
* Improve caching strategies
* Add production database backups
* Add advanced security monitoring

## 🎯 Project Goal

The goal of this project is to create a **scalable, maintainable, secure, and AI-ready personal portfolio platform** rather than a simple static portfolio website.

It provides a foundation for combining:

```text
Modern Web Development
        +
Backend Engineering
        +
Database Engineering
        +
Authentication & Security
        +
Cloud / DevOps
        +
AI Integration
```

## 👨‍💻 Author

**M D Yousuf**

Computer Science & Engineering student interested in:

* Artificial Intelligence
* Machine Learning
* AGI
* Software Engineering
* Biomedical AI
* Robotics
* Cybersecurity
* Future Technologies

---

⭐ If you find this project useful, consider giving the repository a star.
