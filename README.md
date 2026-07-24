<div align="center">

# 🛍️ PrestigeWear Backend

### Production-Ready E-Commerce REST API

Built with **Python**, **FastAPI**, **PostgreSQL**, and **JWT Authentication**

A scalable backend API powering a modern e-commerce platform with secure authentication, product management, shopping cart, order processing, and role-based administration.

<p>

<img src="https://img.shields.io/badge/Python-3.12+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>

<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>

<img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white"/>

<img src="https://img.shields.io/badge/SQLAlchemy-red?style=for-the-badge"/>

<img src="https://img.shields.io/badge/JWT-Authentication-success?style=for-the-badge"/>

<img src="https://img.shields.io/badge/Alembic-Migrations-orange?style=for-the-badge"/>

</p>

</div>

---

# 🚀 Overview

PrestigeWear Backend is a production-style e-commerce REST API built using FastAPI and PostgreSQL.

The backend provides secure authentication, role-based authorization, product and category management, shopping cart functionality, inventory control, and complete order processing through a clean, scalable architecture.

The project follows backend engineering best practices including layered architecture, JWT security, database migrations, and automatic API documentation.

---

# ✨ Key Features

## 🔐 Authentication & Security

- JWT Authentication
- Secure Password Hashing (bcrypt)
- Access Token Authorization
- Role-Based Access Control
- Protected API Routes

---

## 👥 User Management

- User Registration
- Login
- Profile Management
- Customer & Admin Roles

---

## 🗂 Category Management

- Create Categories
- Update Categories
- Delete Categories
- Browse Categories

---

## 👕 Product Management

- Product CRUD
- Product Images
- Product Search
- Inventory Management
- Category Assignment

---

## 🛒 Shopping Cart

- Persistent User Cart
- Quantity Management
- Automatic Price Calculation
- Cart Management

---

## 📦 Order Management

- Place Orders
- Order History
- Automatic Stock Deduction
- Order Status Tracking

Order lifecycle:

```text
Pending
   │
Processing
   │
Shipped
   │
Delivered

or

Cancelled
```

---

# 🏗 System Architecture

```text
             Client Application
                     │
                     ▼
             FastAPI REST API
                     │
      ┌──────────────┼──────────────┐
      │              │              │
 Authentication   Business Logic   Validation
      │              │              │
      └──────────────┼──────────────┘
                     │
                     ▼
               SQLAlchemy ORM
                     │
                     ▼
                PostgreSQL
```

---

# 🛠 Technology Stack

| Category | Technologies |
|-----------|--------------|
| Language | Python 3.12 |
| Framework | FastAPI |
| Database | PostgreSQL |
| ORM | SQLAlchemy |
| Validation | Pydantic |
| Authentication | JWT |
| Password Security | bcrypt |
| Database Migration | Alembic |
| API Documentation | Swagger / ReDoc |

---

# 📂 Project Structure

```bash
backend/
│
├── app/
│   ├── core/
│   ├── database/
│   ├── models/
│   ├── schemas/
│   ├── routers/
│   ├── services/
│   ├── utils/
│   └── main.py
│
├── uploads/
├── alembic/
├── requirements.txt
├── .env.example
└── README.md
```

---

# ⚡ Quick Start

## Clone Repository

```bash
git clone https://github.com/abizaid24/prestigewear-backend.git

cd prestigewear-backend
```

---

## Create Virtual Environment

### Windows

```powershell
python -m venv .venv

.\.venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv .venv

source .venv/bin/activate
```

---

## Install Dependencies

```bash
pip install --upgrade pip

pip install -r requirements.txt
```

---

## Configure Environment

Create a `.env` file.

```env
DATABASE_URL=postgresql://username:password@localhost/prestigewear

SECRET_KEY=your_secret_key

ALGORITHM=HS256

ACCESS_TOKEN_EXPIRE_MINUTES=60
```

---

## Run Database Migrations

```bash
alembic upgrade head
```

---

## Start Development Server

```bash
uvicorn app.main:app --reload
```

Swagger UI

```
http://localhost:8000/docs
```

ReDoc

```
http://localhost:8000/redoc
```

---

# 📡 API Modules

| Module | Endpoint |
|----------|----------------|
| Authentication | /auth |
| Users | /users |
| Categories | /categories |
| Products | /products |
| Shopping Cart | /cart |
| Orders | /orders |

---

# 🔐 Authentication Flow

```text
Register
     │
     ▼
Login
     │
     ▼
Generate JWT Token
     │
     ▼
Access Protected APIs
     │
     ▼
Authorized Request
```

---

# 📸 Screenshots

Add screenshots here:

- Swagger Documentation
- Product API
- Shopping Cart
- Order API
- PostgreSQL Database
- Project Structure

---

# 🚀 Roadmap

### ✅ Implemented

- JWT Authentication
- RBAC
- Product CRUD
- Category CRUD
- Shopping Cart
- Order Processing
- Inventory Management
- Swagger Documentation

### 🔜 Planned

- Refresh Tokens
- Stripe Payments
- Docker Support
- CI/CD Pipeline
- Product Reviews
- Wishlist
- Email Notifications
- Redis Caching

---

# 🌟 Why This Project?

PrestigeWear Backend demonstrates production-ready backend engineering using FastAPI.

The project showcases REST API development, secure authentication, relational database design, layered architecture, inventory management, and scalable business logic suitable for real-world e-commerce applications.

---

# 📄 License

Licensed under the MIT License.

---

# 👨‍💻 Author

## Hafiz Abi Zaid

**Python Backend Developer • FastAPI • Agentic AI**

📧 **hafizabizaid@gmail.com**

🌐 **https://github.com/abizaid24**

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a Star!

Building scalable backend systems with Python & FastAPI.

</div>
