# LEARNING.md

This document summarizes the key learnings and achievements from the Social Media API project, intended to provide context for a CV or professional portfolio.

## 🚀 Project Overview

Developed a full-stack social media backend API inspired by Twitter, using a modern Python technology stack. The project involved designing and implementing a RESTful API with a PostgreSQL database, focusing on performance, scalability, and security. The API supports user authentication, CRUD operations for users and posts, and a voting system for user engagement.

## 🛠️ Skills & Technologies

### Backend Development

- **Python:** Proficient in modern Python 3.8+ features.
- **FastAPI:** Built a high-performance, asynchronous API with FastAPI, including routing, request/response handling, and dependency injection.
- **SQLModel & SQLAlchemy:** Utilized SQLModel for type-safe database operations and SQLAlchemy for ORM capabilities.
- **Pydantic:** Implemented robust data validation and serialization using Pydantic models.
- **Uvicorn:** Deployed the application using the Uvicorn ASGI server.

### Database Management

- **PostgreSQL:** Designed and managed a PostgreSQL database schema, including tables, relationships, and constraints.
- **Database Migrations:** (Implicit) Experience with managing database schema changes.

### Authentication & Security

- **OAuth2 & JWT:** Implemented a secure authentication system using OAuth2 and JSON Web Tokens (JWT) for stateless authentication.
- **Password Hashing:** Secured user passwords using bcrypt (via Passlib) for hashing and verification.

### DevOps & Tools

- **CI/CD:** Configured GitHub Actions workflows for automated release management and changelog generation.
- **Git:** Utilized Git for version control and collaborative development.

### API Design & Development

- **RESTful API Design:** Designed and implemented a RESTful API with clear and consistent endpoints.
- **API Documentation:** Automatically generated interactive API documentation using Swagger UI.
- **Manual API Testing:** Verified API endpoints and logic using tools like Postman.

## 🏆 Major Achievements

- **Implemented a Secure Authentication System:** Designed and implemented a robust authentication and authorization system using OAuth2 with JWT, ensuring secure access to the API. This included token generation, validation, and password hashing.
- **Developed Complex Voting Logic:** Implemented a flexible voting system allowing users to upvote, downvote, or remove votes (neutral), with automatic handling of vote switching (e.g., changing from upvote to downvote).
- **Developed a Full-Featured RESTful API:** Built a comprehensive set of RESTful endpoints for user management, post creation, and voting, with full CRUD functionality.
- **Designed a Relational Database Schema:** Created a well-structured and normalized database schema in PostgreSQL, with clear relationships between users, posts, and votes.
- **Ensured Data Integrity with Pydantic:** Leveraged Pydantic for strict data validation and serialization, preventing common data-related errors and improving the API's reliability.
- **Built for Performance with FastAPI:** Utilized FastAPI's asynchronous capabilities to build a high-performance API capable of handling concurrent requests efficiently.
