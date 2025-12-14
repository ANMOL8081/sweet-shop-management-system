
🧁 Sweet Shop Management System

A full-stack Sweet Shop Management System built using React (Frontend) and Node.js with Express (Backend).
The project demonstrates RESTful API design, JWT-based authentication, database integration, and a modern single-page application (SPA) frontend.

This project was developed using GitHub Codespaces following clean coding practices and version control workflows.

📌 Features
👤 Authentication

User Registration

User Login

Token-based authentication using JWT

Role-based access (User / Admin)

🍬 Sweet Management

Add new sweets (Admin only)

View all available sweets

Search sweets by name/category/price

Update sweet details (Admin only)

Delete sweets (Admin only)

📦 Inventory Management

Purchase sweets (quantity decreases)

Restock sweets (Admin only)

Purchase button disabled when stock is zero

🖥 Frontend

Single Page Application (SPA)

Login & Register pages

Responsive UI

API integration using Axios

🛠 Tech Stack
Frontend

React

React Router

Axios

HTML, CSS, JavaScript

Backend

Node.js

Express.js

JWT Authentication

SQLite Database

Tools & Platforms

GitHub Codespaces

Git & GitHub

npm

📂 Project Structure
sweet-shop-management-system/
│sweet-shop-management-system/
│
├── backend/
│   ├── index.js
│   ├── database.js
│   ├── sweetshop.db
│   ├── src/
│   │   ├── routes/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   └── tests/
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── services/
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
│
└── README.md


⚙️ Setup & Run Instructions
🔹 Prerequisites

Node.js (v16+ recommended)

npm

GitHub account

🔹 Backend Setup
cd backend
npm install
npm start


Backend will run on:

http://localhost:5000

🔹 Frontend Setup
cd frontend
npm install
npm start


Frontend will run on:

http://localhost:3000

🔐 API Endpoints
Authentication

POST /api/auth/register

POST /api/auth/login

Sweets (Protected)

POST /api/sweets

GET /api/sweets

GET /api/sweets/search

PUT /api/sweets/:id

DELETE /api/sweets/:id (Admin)

Inventory

POST /api/sweets/:id/purchase

POST /api/sweets/:id/restock (Admin)

🧪 Testing

Backend testing is done using Jest and Supertest following Test-Driven Development (TDD) principles.

npm test
