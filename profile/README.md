# 🚀 Noyra Labs

> Building scalable Discord operations infrastructure with modern cloud architecture

## About

Noyra Labs develops microservice-based solutions for Discord community management, focusing on ticket systems, role management, and service monitoring. Our infrastructure leverages containerized Discord bots with serverless AWS backends to deliver reliable, scalable operations tools.

---

## 🏗️ Architecture Overview

Our ecosystem consists of two primary microservices working in tandem:

```
┌─────────────────────┐         ┌──────────────────────┐
│   NoyraDocket Bot   │────────▶│   Tickets AWS API    │
│   (Discord Bot)     │         │   (Lambda Backend)   │
│                     │         │                      │
│  • TypeScript       │         │  • Node.js Lambdas   │
│  • SapphireJS       │         │  • S3 Storage        │
│  • Discord.js       │         │  • API Gateway       │
│  • Prisma ORM       │         │                      │
│  • MariaDB          │         │                      │
│  • Docker           │         │                      │
└─────────────────────┘         └──────────────────────┘
```

---

## 📦 Microservices

### NoyraDocket — Discord Operations Bot

A comprehensive Discord bot built on the Sapphire Framework for managing private-thread ticket workflows, role enrollment, and service alerts.

**Key Features:**
- 🎫 **Ticket Lifecycle Management** — Private-thread tickets with type selection, role-based access, status tracking, and automated closure workflows
- ⚙️ **Per-Guild Configuration** — Customizable ticket types, numbering formats, and notification channels
- 👥 **Role Self-Enrollment** — Interactive announcement panels with toggle buttons for role management
- 📊 **Service Monitoring** — Integration capabilities for external service status tracking
- 📝 **Transcript Generation** — Automatic transcript creation and cloud storage integration

**Tech Stack:**
- TypeScript with SapphireJS framework
- Discord.js for Discord API integration
- Prisma ORM with MariaDB
- Docker containerization
- Modular command and interaction handling architecture

---

### Tickets-AWS — Serverless Transcript Backend

A serverless AWS Lambda backend providing secure transcript storage and retrieval for Discord support tickets.

**Capabilities:**
- 📤 **Secure Upload** — Authenticated API for transcript ingestion
- 💾 **Cloud Storage** — Scalable S3-based storage with lifecycle management
- 🌐 **Web Access** — Rendered HTML transcript pages and raw JSON retrieval
- 🔒 **Security** — API authentication and input validation

**Tech Stack:**
- Node.js Lambda functions
- AWS Lambda, S3, and API Gateway
- Serverless architecture with automatic scaling
- RESTful API design

---

## 🔄 System Integration

The two microservices work together to provide a complete ticket management solution:

1. **Ticket Creation** — Users create support tickets through Discord interactions
2. **Lifecycle Management** — Comprehensive status tracking and user management
3. **Transcript Generation** — Automatic capture of ticket conversations
4. **Cloud Storage** — Secure, persistent transcript archival
5. **Web Access** — Shareable transcript links for reference and auditing

---

## 🛠️ Development Philosophy

- **Microservice Architecture** — Loosely coupled services with clear boundaries
- **Cloud-Native Design** — Leveraging managed services for scalability and reliability
- **Infrastructure as Code** — Reproducible deployments via Docker and serverless configurations
- **Security First** — API authentication, input validation, and secure credential management
- **Developer Experience** — Comprehensive documentation, type safety, and modern tooling

---

## 📊 Tech Stack Summary

| Category | Technologies |
|----------|--------------|
| **Languages** | TypeScript, Node.js |
| **Frameworks** | SapphireJS, Discord.js |
| **Databases** | MariaDB, Prisma ORM |
| **Cloud Services** | AWS Lambda, S3, API Gateway |
| **Infrastructure** | Docker, Serverless |
| **Development Tools** | Just, ESLint, Prettier |

---

<div align="center">

**Built with ❤️ by Noyra Labs**

*Scalable Discord operations infrastructure for modern communities*

</div>

