# High-Level Design Document

## 1. Introduction
This document provides a high-level design overview of the Budget Minder application. The goal is to outline the main components, their interactions, and the technologies used.

## 2. System Overview
Budget Minder is a web-based budget management application that allows users to forecast monthly budgets, manage income and expenses, set savings goals, and track progress.

## 3. Main Components
- **Frontend (GUI)**: Built with React.js to provide an interactive user interface.
- **Backend (Server)**: Implemented using Node.js with Express.js to handle API requests and business logic.
- **Database**: MongoDB is used for data persistence.
- **Security**: bcrypt for password hashing and JSON Web Token (JWT) for authentication.

## 4. Architecture Diagram
```mermaid
graph TD;
    A[User] -->|HTTP Requests| B[React.js Frontend]
    B -->|API Calls| C[Express.js Backend]
    C -->|CRUD Operations| D[MongoDB Database]
    C -->|Authentication| E[JWT & bcrypt]
