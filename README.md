<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Banking%20Application&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Secure%20%C2%B7%20Scalable%20%C2%B7%20Production-Grade&descAlignY=58&descSize=16&descColor=93c5fd" width="100%"/>

<br/>

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=Apache%20Maven&logoColor=white)

<br/>

> **A full-stack digital banking platform** built with Spring Boot, React, and JWT-based authentication —
> engineered to mirror real-world banking infrastructure with security-first design and clean layered architecture.

<br/>

[![GitHub stars](https://img.shields.io/github/stars/sujxth0304/springboot-banking-app?style=social)](https://github.com/sujxth0304/springboot-banking-app)&nbsp;&nbsp;
[![GitHub forks](https://img.shields.io/github/forks/sujxth0304/springboot-banking-app?style=social)](https://github.com/sujxth0304/springboot-banking-app/fork)

</div>

<br/>

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Tech Stack](#️-tech-stack)
- [Architecture](#-architecture)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Testing](#-testing)
- [Roadmap](#-roadmap)
- [Author](#-author)

---

## 🧭 Overview

This isn't just another CRUD app. It's a **security-aware, layered, and scalable banking system** designed to reflect how real banking backends are structured — the kind of project that demonstrates genuine engineering depth.

| Area | What was built |
|------|---------------|
| 🔐 Security | JWT auth, BCrypt encryption, role-based access control |
| 💳 Banking | Deposits, withdrawals, transfers, transaction history |
| 🧩 Backend | Layered Spring Boot architecture with DTO pattern |
| 🌐 Frontend | React SPA with full API integration |

---

## ✨ Key Features

<details>
<summary><b>🔐 Authentication & Security</b></summary>

<br/>

- Stateless **JWT-based authentication**
- Secure login & registration flow
- **Role-based access control** — `USER` / `ADMIN`
- **BCrypt** password hashing
- Protected REST endpoints via Spring Security filter chain

</details>

<details>
<summary><b>💳 Banking Operations</b></summary>

<br/>

- Account creation & management
- Real-time balance inquiry
- Deposits & withdrawals
- **Peer-to-peer fund transfers**
- Full transaction history tracking

</details>

<details>
<summary><b>🧩 Backend Architecture</b></summary>

<br/>

- RESTful APIs with Spring Boot
- **Controller → Service → Repository** layered design
- DTO-based request/response handling
- Global exception handling with meaningful error responses
- Clean separation of business logic from persistence

</details>

<details>
<summary><b>🌐 React Frontend</b></summary>

<br/>

- Component-based architecture
- Axios-powered API integration
- Responsive and user-friendly design
- Protected routes based on auth state

</details>

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology |
|-------|-----------|
| **Language** | Java |
| **Framework** | Spring Boot |
| **Security** | Spring Security + JWT |
| **ORM** | Hibernate / JPA |
| **Database** | MySQL |
| **Build Tool** | Maven |
| **Frontend** | React, JavaScript (ES6+) |
| **HTTP Client** | Axios |
| **API Testing** | Postman |
| **Version Control** | Git & GitHub |

</div>

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────┐
│           CLIENT (React SPA)            │
│     Component UI  ·  Axios  ·  ES6+     │
└──────────────────┬──────────────────────┘
                   │  HTTP / REST
┌──────────────────▼──────────────────────┐
│        REST API LAYER (Spring Boot)     │
│   Controllers  ·  DTOs  ·  JWT Filter   │
└──────────────────┬──────────────────────┘
                   │
┌──────────────────▼──────────────────────┐
│         SERVICE LAYER                   │
│   Business Logic  ·  Transaction Mgmt   │
└──────────────────┬──────────────────────┘
                   │
┌──────────────────▼──────────────────────┐
│         REPOSITORY LAYER                │
│        JPA / Hibernate  ·  DAO          │
└──────────────────┬──────────────────────┘
                   │
┌──────────────────▼──────────────────────┐
│           MySQL DATABASE                │
│     Relational Schema  ·  ACID          │
└─────────────────────────────────────────┘
```

---

## 📂 Project Structure

```bash
springboot-banking-app/
│
├── 📁 backend/
│   ├── 📁 controller/        # REST endpoints
│   ├── 📁 service/           # Business logic
│   ├── 📁 repository/        # Data access layer
│   ├── 📁 model/             # JPA entities
│   ├── 📁 dto/               # Request/Response objects
│   ├── 📁 security/          # JWT filter, config
│   └── 📁 exception/         # Global exception handling
│
├── 📁 frontend/
│   ├── 📁 components/        # Reusable UI components
│   ├── 📁 pages/             # Route-level pages
│   ├── 📁 services/          # API service calls
│   └── 📁 utils/             # Helper functions
│
└── 📄 README.md
```

---

## 🚀 Getting Started

### Prerequisites

- Java 17+
- Node.js 18+
- MySQL 8+
- Maven 3.8+

### Backend Setup

```bash
# Clone the repository
git clone https://github.com/sujxth0304/springboot-banking-app.git

# Navigate to backend
cd springboot-banking-app/backend

# Build the project
mvn clean install

# Run the application
mvn spring-boot:run
```

> API will be available at `http://localhost:8080`

### Frontend Setup

```bash
# Navigate to frontend
cd ../frontend

# Install dependencies
npm install

# Start the dev server
npm start
```

> App will be available at `http://localhost:3000`

---

## 🔑 Environment Variables

Create `src/main/resources/application.properties`:

```properties
# ── Database ────────────────────────────────────────────
spring.datasource.url=jdbc:mysql://localhost:3306/banking_app
spring.datasource.username=your_username
spring.datasource.password=your_password

# ── JWT ─────────────────────────────────────────────────
jwt.secret=your_secret_key_here
jwt.expiration=86400000

# ── JPA / Hibernate ─────────────────────────────────────
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

---

## 🧪 Testing

- ✅ API testing via **Postman**
- ✅ Authentication & authorization edge cases covered
- ✅ Manual testing of all transaction workflows
- ✅ Role-based access scenarios validated

---

## 🗺️ Roadmap

- [x] JWT Authentication
- [x] Core banking operations
- [x] Role-based access control
- [x] Transaction history
- [ ] Transaction rollback support
- [ ] Scheduled & recurring payments
- [ ] Admin analytics dashboard
- [ ] Two-factor authentication (2FA)
- [ ] Docker + CI/CD pipeline
- [ ] Audit logs for compliance

---

## 👨‍💻 Author

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f2027,100:2c5364&height=2&section=header" width="100%"/>

<br/>

**Sujith Santhosh**

*Backend & Systems Enthusiast · Aspiring Software Engineer*

[![GitHub](https://img.shields.io/badge/GitHub-@sujxth0304-181717?style=for-the-badge&logo=github)](https://github.com/sujxth0304)

<br/>

*If this project helped you or impressed you — drop a ⭐ on the repo. It means a lot!*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer" width="100%"/>

</div>
