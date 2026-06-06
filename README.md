# 📋 Attendance Management System

> A web application to record and query student attendance by course and subject.

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)

---

## 📁 Project Structure

```
tp/
├── server.js
├── bd.sql
└── public/
    ├── index.html
    ├── style.css
    └── main.js
```

---

## ✨ Features

- 👤 **Create students** and assign them to a course
- ✅ **Record attendance** by student, subject, and type
- 🔍 **Query attendance** filtering by course, subject, and date
- ✏️ **Edit** existing records
- 🗑️ **Delete** records with confirmation prompt

---

## 🗄️ Database

**Tables:** `courses` · `students` · `subjects` · `records`

**Attendance types:**

| Code | Meaning |
|------|---------|
| `P` | Present |
| `A` | Absent |
| `T` | Late |
| `RA` | Early departure |
| `AP` | Excused absence |

---

## 🌐 API Endpoints

| Method | Route | Description |
|--------|-------|-------------|
| `GET` | `/cursos` | List all courses |
| `GET` | `/materias/:cursoId` | Get subjects for a course |
| `GET` | `/alumnos/:cursoId` | Get students in a course |
| `POST` | `/alumnos` | Create a new student |
| `POST` | `/asistencias` | Record attendance |
| `GET` | `/asistencias` | Query attendance records |
| `PUT` | `/asistencias/:id` | Update an attendance record |
| `DELETE` | `/asistencias/:id` | Delete an attendance record |

---

## 🚀 Getting Started

**1. Import the database**
```bash
mysql -u root -p < bd.sql
```

**2. Install dependencies**
```bash
npm install
```

**3. Start the server**
```bash
node server.js
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🛠️ Tech Stack

- **Backend:** Node.js + Express
- **Database:** MySQL
- **Frontend:** Vanilla JavaScript, HTML5, CSS3

---

