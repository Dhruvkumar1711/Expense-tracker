# Expense Tracker API

## Overview
A REST API for tracking personal expenses, with JWT-based auth.

## Tech Stack
Node, Express, PostgreSQL, pg , bcrypt, jsonwebtoken

## Data Model
### Users
- id, email, password_hash, created_at

### Expenses
- id, user_id (FK), amount, category, description, date, created_at

## API Endpoints
POST   /api/auth/signup
POST   /api/auth/login
GET    /api/expenses?range=week|month|3months&start=&end=
POST   /api/expenses
PUT    /api/expenses/:id
DELETE /api/expenses/:id

## Setup
1. clone repo
2. npm install
3. set up .env (DATABASE_URL, JWT_SECRET)
4. npm run dev