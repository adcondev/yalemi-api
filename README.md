# Yalemi API

![Project Logo](https://via.placeholder.com/150)

> **Y**et **A**nother **L**earning **E**xperience **M**ade **I**n **P**ython.

A robust Social Media REST API built with FastAPI, SQLModel, and PostgreSQL. This project demonstrates a scalable backend architecture featuring user authentication, content management, and interaction systems.

![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-0.109.0-009688.svg)
![License](https://img.shields.io/badge/license-MIT-green)
![Build Status](https://img.shields.io/badge/build-passing-brightgreen)

## 🏗️ Architecture

```mermaid
graph TD
    Client[Client Application] -->|HTTP / JSON| API[FastAPI Gateway]
    
    subgraph "Application Layer"
        API --> Auth[Auth Router]
        API --> User[User Router]
        API --> May["May (Post) Router"]
        API --> Vote[Vote Router]
    end
    
    subgraph "Data Layer"
        Auth --> ORM[SQLModel ORM]
        User --> ORM
        May --> ORM
        Vote --> ORM
        ORM --> DB[(PostgreSQL Database)]
    end
```

## 🚀 Features

- **User Management**: Registration, profile updates, and secure password handling.
- **Authentication**: JWT-based OAuth2 authentication flow.
- **Content System**: Create, read, and manage "Mays" (posts).
- **Voting System**: Upvote/downvote functionality with duplicate prevention.
- **Documentation**: Auto-generated Swagger UI and ReDoc.

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/adcondev/yalemi-api.git
   cd yalemi-api
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Environment Configuration**
   Copy `.env.example` to `.env` and update the values:
   ```bash
   cp .env.example .env
   ```
   *Make sure you have a PostgreSQL instance running and accessible.*

## 🏃 Usage

Start the development server:

```bash
uvicorn app.main:app --reload
```

The API will be available at `http://localhost:8000`.
- **Interactive Docs (Swagger UI):** `http://localhost:8000/docs`
- **Alternative Docs (ReDoc):** `http://localhost:8000/redoc`

## 🤝 Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.MD) for details on our code of conduct, and the process for submitting pull requests to us.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
