# 🎓 Virtual Classroom - Smart Learning Platform

A full-featured virtual classroom platform built with Flask, SocketIO, and modern web technologies.

## 📌 Project Overview

Virtual Classroom is a full-stack web application that provides a digital learning environment for students and teachers. It allows teachers to create classrooms, manage assignments, conduct quizzes, communicate with students, and monitor learning progress.

Students can join classrooms, submit assignments, participate in discussions, attend live sessions, and use productivity tools.

The platform also integrates an AI-powered teaching assistant to support learning and educational activities.

## ✨ Features

- **Real-time Chat & Video** — Live classroom sessions with WebRTC
- **Assignments & Grading** — Create, submit, and grade assignments with file uploads
- **Live Quizzes** — Interactive quizzes with leaderboards
- **Discussion Threads** — Forum-style class discussions
- **AI Teaching Assistant** — Powered by Google Gemini
- **Gamification** — XP, levels, streaks, badges, and daily challenges
- **Scheduling** — Class schedules with notifications
- **Whiteboard** — Collaborative real-time whiteboard
- **Todo & Bookmarks** — Personal productivity tools
👨‍🏫 User Management
- Student and teacher registration
- Secure login and logout
- JWT-based authentication
- Role-based access control
- User profile management

### 🏫 Classroom Management
- Create and manage classrooms
- Join classrooms using unique codes
- Student enrollment management
- Classroom announcements
- Member management

### 📝 Assignment Management
- Create and distribute assignments
- Upload assignment files
- Submit assignments
- Teacher grading and feedback
- Assignment notifications

### 💬 Communication
- Real-time classroom chat
- Private messaging
- Message reactions
- Pinned messages
- Typing indicators

### 🎥 Live Classroom
- Video communication using WebRTC
- Microphone and camera controls
- Screen sharing
- Participant management
- Raise-hand functionality
- In-class chat and quizzes

### 🧠 AI Teaching Assistant
- AI-powered learning assistance
- Ask educational questions
- Generate learning notes
- Save and manage AI notes
- Google Gemini API integration

### 📝 Collaborative Whiteboard
- Real-time drawing
- Pen and eraser tools
- Shapes and colors
- Sticky notes
- Undo and clear options
- Download whiteboard as an image

### 🏆 Gamification
- Experience points (XP)
- Student levels
- Achievement badges
- Learning streaks
- Daily challenges
- Leaderboard

### 📊 Productivity and Analytics
- Student learning analytics
- Dashboard overview
- Personal to-do list
- Bookmark management
- Class scheduling
- Notifications

## 🚀 Quick Start (Local)

```bash
pip install -r requirements.txt
python app.py
```

Visit `http://localhost:5000`

**Demo Accounts:**
- Teacher: `teacher@demo.com` / `password123`
- Student: `student@demo.com` / `password123`

## 🌐 Deploy on Railway

1. Push this repo to GitHub
2. Go to [railway.app](https://railway.app) → **New Project** → **Deploy from GitHub Repo**
3. Add a **PostgreSQL** plugin from the dashboard
4. Set environment variables (see below)
5. Deploy!

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `DATABASE_URL` | Auto-set by Railway PostgreSQL plugin | ✅ Auto |
| `SECRET_KEY` | Flask secret key | ✅ Set manually |
| `GEMINI_API_KEY` | Google Gemini API key for AI assistant | Optional |
| `PORT` | Server port | ✅ Auto |

## 🛠 Technology Stack

| Category | Technologies |
|---|---|
| Frontend | HTML5, CSS3, JavaScript |
| Backend | Python, Flask |
| Database | SQLite, PostgreSQL |
| ORM | Flask-SQLAlchemy |
| Authentication | JWT, Werkzeug |
| Real-time Communication | Flask-SocketIO |
| Video Communication | WebRTC |
| AI Integration | Google Gemini API |
| Data Visualization | Chart.js |
| Icons | Lucide |
| Deployment | Gunicorn, Eventlet |

## 📂 Project Structure

```text
Virtual-Classroom/
│
├── app.py
├── models.py
├── auth_routes.py
├── api_routes.py
├── utils.py
│
├── templates/
│   └── index.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   │
│   └── js/
│       ├── app.js
│       ├── auth.js
│       ├── ai.js
│       ├── chat.js
│       ├── classroom.js
│       ├── dashboard.js
│       ├── gamification.js
│       ├── productivity.js
│       ├── video.js
│       └── whiteboard.js
│
├── requirements.txt
├── Procfile
├── runtime.txt
├── nixpacks.toml
├── .gitignore
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Virtual-Classroom.git
```

### 2. Navigate to the Project Directory

```bash
cd Virtual-Classroom
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

**Windows:**

```bash
venv\Scripts\activate
```

**Linux / macOS:**

```bash
source venv/bin/activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Configure Environment Variables

Create a `.env` file in the root directory.

```env
SECRET_KEY=your-secure-secret-key
GEMINI_API_KEY=your-google-gemini-api-key
DATABASE_URL=sqlite:///virtual_classroom.db
```

The Gemini API key is optional if you do not need AI features.

For production, configure PostgreSQL using the appropriate database URL.

### 7. Run the Application

```bash
python app.py
```

### 8. Open in Browser

```text
http://localhost:5000
```

## 🗄️ Database

The application uses Flask-SQLAlchemy for database management.

- SQLite is used as the default local database.
- PostgreSQL can be configured for production deployment.
- Database models manage users, classrooms, assignments, submissions, messages, quizzes, notifications, and other application data.

## 🔐 Security

The project includes:

- Password hashing using Werkzeug
- JWT-based authentication
- Role-based authorization
- Protected API endpoints
- File extension validation
- Environment-based configuration for API credentials

**Important:** Configure a strong SECRET_KEY before deployment. Never publish API keys, passwords, or production credentials.

## 🚀 Deployment

The project includes deployment configuration files:

- `Procfile`
- `runtime.txt`
- `nixpacks.toml`

It can be prepared for deployment on compatible Python hosting platforms, with PostgreSQL and the required environment variables configured.

## 🎯 Project Objectives

- Make online learning more interactive.
- Improve communication between students and teachers.
- Simplify assignment management and grading.
- Support collaborative learning.
- Provide AI-assisted educational support.
- Encourage student engagement through gamification.

## 👨‍💻 Author

**Your Name**

GitHub: https://github.com/sadapahmed007-arch

## 📄 License

No license has been specified yet. All rights reserved unless a license is added to this repository.

