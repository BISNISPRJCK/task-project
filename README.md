# 📌 Task Management Project

A simple **Task Management Application** built with **Node.js (Express, PostgreSQL, Sequelize)** for the backend and **React.js** for the frontend.  
This project is part of a take-home assessment for Backend Developer role.

---

## 🚀 Getting Started

### 1. Clone Repository

```bash
git clone https://github.com/BISNISPRJCK/task-project
cd task-project
2. Setup Backend
bash

cd backend
npm install
🗄️ Configure Database
Create PostgreSQL database:

sql

CREATE DATABASE taskdb;
Update database config in backend/config/db.js with your PostgreSQL username and password:

js

import { Sequelize } from "sequelize";

const sequelize = new Sequelize("taskdb", "postgres", "Rakkha-17", {
  host: "localhost",
  dialect: "postgres",
  logging: false,
});

export default sequelize;
▶️ Run Backend
bash
nodemon server.js
# or
node server.js
Backend will run at:
👉 http://localhost:5000

3. Setup Frontend
bash
cd ../frontend
npm install
npm start
⚠️ Requires Node.js v22

Frontend will run at:
👉 http://localhost:3000

📌 API Endpoints
Create Task
POST /tasks

json
{
  "title": "Finish assignment",
  "description": "Complete the backend task",
  "status": "pending",
  "due_date": "2025-08-30"
}
Get All Tasks
GET /tasks

Get Task by ID
GET /tasks/:id

Update Task
PUT /tasks/:id

Delete Task
DELETE /tasks/:id

🖥️ Frontend Features
Show list of tasks in a table

Add new task

Edit task

Delete task

View task details

📖 Assumptions & Design Decisions
Task must have title and due_date

status can only be pending or completed

Simple UI with focus on CRUD functionality

✅ Evaluation Ready
Clear folder structure for backend and frontend

API documentation included

Database configuration with Sequelize

CRUD operations tested and working
```
