# TASK 3 — Project Management Tool (Full Details)

## Project Name

**CodeAlpha_ProjectManagementTool**

---

## Project Overview

Build a full-stack collaborative project management application similar to:

- **Trello**
- **Asana**
- **Jira**

Users can:

- Create projects
- Create task boards
- Assign tasks
- Add comments
- Track project progress
- Receive notifications
- Get real-time updates

---

## Tech Stack

### Frontend

- React.js
- HTML
- CSS
- JavaScript
- React Router
- axios
- socket.io-client

### Backend

- Node.js
- Express.js
- MongoDB (Mongoose)
- Socket.io (real-time)
- JWT Authentication
- bcryptjs
- multer (uploads)

---

## ✅ Main Features (1–7)

### 1) User Authentication

- Register
- Login
- Logout
- JWT Authentication
- Protected Routes

### 2) Dashboard

Dashboard shows:

- Total Projects
- Pending Tasks
- Completed Tasks
- Notifications

### 3) Project Management

Users can:

- Create Projects
- Edit Projects
- Delete Projects
- Add Team Members

Example:

- Project Name: **Website Redesign**
- Description: **Build new company website**

### 4) Task Management

Users can:

- Create Tasks
- Assign Tasks
- Set Deadlines
- Change Task Status

Task Status:

- **To Do**
- **In Progress**
- **Completed**

### 5) Comments System

Inside each task:

- Add comments
- Team communication
- Discussion thread

Example:

- “Frontend design completed.”

### 6) Notifications

Notifications for:

- Task assigned
- Task completed
- New comments
- Project updates

### 7) Real-Time Updates (Socket.io)

- Instant task updates
- Live comments
- Live notifications

---

## 🗂️ Database Collections (Sample Schemas)

### users

```json
{
  "name": "Siva",
  "email": "siva@gmail.com",
  "password": "hashedPassword"
}
```

### projects

```json
{
  "title": "Project Management Tool",
  "description": "Full stack project",
  "members": ["userId"]
}
```

### tasks

```json
{
  "title": "Build Login Page",
  "status": "In Progress",
  "assignedTo": "userId",
  "deadline": "2026-05-30"
}
```

### comments

```json
{
  "taskId": "123",
  "userId": "456",
  "message": "Task completed"
}
```

### notifications

```json
{
  "userId": "456",
  "type": "TASK_ASSIGNED",
  "message": "You were assigned a new task",
  "read": false
}
```

---

## 📂 Important Pages

| Page      | Purpose           |
| --------- | ----------------- |
| Home      | Landing page      |
| Login     | User login        |
| Register  | User registration |
| Dashboard | Main overview     |
| Projects  | Manage projects   |
| Tasks     | Manage tasks      |
| Team      | Team members      |
| Profile   | User profile      |

---

## 📂 Important Components

| Component      | Purpose          |
| -------------- | ---------------- |
| Navbar         | Navigation       |
| Sidebar        | Dashboard menu   |
| Board          | Task board       |
| TaskCard       | Display tasks    |
| ProjectCard    | Display projects |
| CommentSection | Task comments    |
| Notification   | Alerts           |
| Loader         | Loading UI       |
| Modal          | Popups           |

---

## 🔌 API Routes

### Authentication

- `/api/auth/register`
- `/api/auth/login`

### Projects

- `/api/projects/create`
- `/api/projects/update/:id`
- `/api/projects/delete/:id`

### Tasks

- `/api/tasks/create`
- `/api/tasks/update/:id`
- `/api/tasks/delete/:id`

### Comments

- `/api/comments/add`

---

## 📦 Required Packages

### Frontend

- `npm install axios react-router-dom react-icons socket.io-client`

### Backend

- `npm install express mongoose cors dotenv bcryptjs jsonwebtoken socket.io multer`

---

## ▶️ Run Project

### Frontend

```bash
cd client
npm install
npm run dev
```

### Backend

```bash
cd server
npm install
node server.js
```

---

## 🌟 Bonus Features (Optional)

- Drag & Drop Tasks
- File Uploads
- Team Chat
- Dark Mode
- Email Notifications
- Activity Logs
- Search & Filters

---

## 📌 GitHub Repository Structure

- `client/` (React)
- `server/` (Express)

---

## 📹 Explain (What to Demo)

- Login/Register
- Create Project
- Create Tasks
- Assign Tasks
- Real-Time Updates
- Database Working
- Backend APIs

---

## ✅ Internship Criteria Covered

- ✅ Frontend Development
- ✅ Backend Development
- ✅ Authentication
- ✅ REST APIs
- ✅ MongoDB Integration
- ✅ Real-Time Features
- ✅ Full Stack Architecture
- ✅ GitHub Repository
- ✅ Deployment Ready
