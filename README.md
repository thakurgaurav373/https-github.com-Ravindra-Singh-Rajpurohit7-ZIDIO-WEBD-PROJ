# IntellMeet — AI-Powered Meeting & Collaboration Platform

> A full-stack, real-time meeting and collaboration platform designed for modern remote and hybrid teams.




\

## 🚀 Overview

**IntellMeet** is a full-stack AI-powered meeting and collaboration platform built for remote and hybrid teams.

The platform combines **real-time video communication, messaging, screen sharing, AI-powered meeting assistance, team workspaces, authentication, and collaborative features** into a single application.

The project was developed to demonstrate practical full-stack engineering skills, including:

* Modern React frontend development
* REST API development
* Real-time WebSocket communication
* WebRTC-based video communication
* JWT authentication
* MongoDB database integration
* OpenAI API integration
* Responsive UI development
* Full-stack deployment

---

## ✨ Key Features

### 🔐 Authentication & User Management

* User registration and login
* JWT-based authentication
* Protected routes
* User profile management
* Secure session handling

### 🎥 Real-Time Video Meetings

* Create and join meetings
* Browser-based video conferencing
* Audio/video controls
* Participant management
* Screen sharing
* Leave/end meeting functionality
* WebRTC-powered communication

### 💬 Real-Time Chat

* Meeting-based chat
* Real-time message delivery
* Typing indicators
* Message timestamps
* Socket.IO-powered communication

### 🤖 AI Meeting Assistant

The AI assistant helps transform meetings into structured information.

Features include:

* Meeting summarization
* Action-item extraction
* AI-generated meeting insights
* Transcript-based processing
* OpenAI API integration
* Saving generated meeting information

### 👥 Team Workspace

* Create teams/workspaces
* Add and manage team members
* Shared notes
* Collaborative workspace functionality

### 📊 Meeting Management

* Create meetings
* Join using Meeting ID
* Upcoming meetings
* Meeting history
* Meeting information management

### 📱 Responsive Design

The interface is designed to work across:

* Desktop
* Laptop
* Tablet
* Mobile devices

---

# 🛠️ Tech Stack

## Frontend

| Technology       | Purpose                       |
| ---------------- | ----------------------------- |
| React            | UI development                |
| Vite             | Frontend build tool           |
| Tailwind CSS     | Styling and responsive design |
| JavaScript       | Application logic             |
| WebRTC           | Real-time audio/video         |
| Socket.IO Client | Real-time communication       |

## Backend

| Technology | Purpose                 |
| ---------- | ----------------------- |
| Node.js    | Runtime                 |
| Express.js | REST API                |
| Socket.IO  | Real-time communication |
| JWT        | Authentication          |
| MongoDB    | Database                |
| Mongoose   | MongoDB ODM             |
| OpenAI API | AI meeting assistance   |

## Deployment

| Service       | Purpose             |
| ------------- | ------------------- |
| Vercel        | Frontend deployment |
| Render        | Backend deployment  |
| MongoDB Atlas | Cloud database      |

---

# 🏗️ System Architecture

```text
                         ┌─────────────────────┐
                         │       User          │
                         │ Browser / Mobile    │
                         └──────────┬──────────┘
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │   React + Vite      │
                         │   Frontend          │
                         └──────────┬──────────┘
                                    │
                     ┌──────────────┼──────────────┐
                     │              │              │
                     ▼              ▼              ▼
                  REST API      Socket.IO        WebRTC
                     │              │              │
                     ▼              ▼              ▼
             ┌────────────────────────────────────────┐
             │          Node.js + Express              │
             │              Backend                    │
             └──────────────────┬─────────────────────┘
                                │
                     ┌──────────┴──────────┐
                     │                     │
                     ▼                     ▼
              MongoDB Atlas           OpenAI API
              Database                AI Assistant
```

---

# 📂 Project Structure

```text
ZIDIO-WEBD-PROJ/
│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── sockets/
│   │   └── ...
│   │
│   ├── package.json
│   ├── package-lock.json
│   └── .env.example
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── ...
│   │
│   ├── public/
│   ├── package.json
│   └── ...
│
├── .gitignore
├── README.md
└── LICENSE
```

> The exact folder structure may vary depending on the current project version.

---

# ⚙️ Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/ZIDIO-WEBD-PROJ.git

cd ZIDIO-WEBD-PROJ
```

---

# 🔧 Backend Setup

Navigate to the backend:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file:

```env
PORT=5000

MONGO_URI=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret

OPENAI_API_KEY=your_openai_api_key

CLIENT_URL=http://localhost:5173
```

Start the backend:

```bash
npm run dev
```

Backend will run on:

```text
http://localhost:5000
```

---

# 💻 Frontend Setup

Open another terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Create the required environment variables:

```env
VITE_API_URL=http://localhost:5000
```

Start the development server:

```bash
npm run dev
```

Open:

```text
http://localhost:5173
```

---

# 🔑 Environment Variables

Never commit your real environment variables to GitHub.

Use:

```text
.env
```

for local development and:

```text
.env.example 
```

for documenting required variables.

Example:

```env
MONGO_URI=
JWT_SECRET=
OPENAI_API_KEY= 
CLIENT_URL=
VITE_API_URL=
```

---

# 🔒 Security

The project follows basic security practices including:

* JWT-based authentication
* Protected API routes
* Environment variables for secrets
* Password hashing
* CORS configuration
* Separation of frontend and backend
* No API keys committed to source control

> Production deployments should use platform-managed environment variables and HTTPS.

---

# 🌐 Live Demo

### 🚀 IntellMeet

**Live Application:**

https://intellmeet-full-stack-project.vercel.app

> The live demo may require configured backend services and environment variables.

---

# 📸 Screenshots

Add screenshots of the following sections to make the repository more attractive to recruiters:

```text
screenshots/
├── landing-page.png
├── login.png
├── dashboard.png
├── meeting-room.png
├── video-call.png
├── chat.png
├── ai-assistant.png
└── team-workspace.png
```

Then display them in the README:

```markdown
## 📸 Screenshots

### Dashboard

![Dashboard](screenshots/dashboard.png)

### Video Meeting

![Video Meeting](screenshots/video-call.png)

### AI Meeting Assistant

![AI Assistant](screenshots/ai-assistant.png)

### Team Workspace

![Team Workspace](screenshots/team-workspace.png)
```

---

# 🧠 What I Learned

Building IntellMeet helped me develop practical experience in:

* Designing full-stack applications
* Building REST APIs with Node.js and Express
* Implementing JWT authentication
* Working with MongoDB and Mongoose
* Building real-time applications with Socket.IO
* Understanding WebRTC communication
* Integrating AI APIs into production-style applications
* Managing asynchronous operations
* Designing responsive React applications
* Connecting frontend and backend services
* Debugging deployment and environment issues
* Working with cloud-hosted databases
* Deploying full-stack applications

---

# 🚧 Challenges Solved

Some of the major engineering challenges included:

### Real-Time Communication

Managing real-time communication between multiple users required WebSocket-based event handling and synchronization.

### WebRTC

Implementing browser-based audio/video communication required understanding:

* Media streams
* Peer connections
* ICE candidates
* Offer/answer negotiation
* Connection lifecycle

### AI Integration

The meeting assistant required connecting application data with an external AI service and converting meeting information into useful structured outputs.

### Authentication

JWT authentication was implemented to protect user-specific resources and application routes.

### Deployment

The application required coordinating:

```text
Frontend → Vercel
Backend → Render
Database → MongoDB Atlas
AI → OpenAI API
```

while maintaining correct environment configuration.

---

# 🎯 Future Improvements

Planned improvements include:

* Advanced meeting transcription
* Speaker identification
* Better AI meeting analytics
* Calendar integration
* Meeting recording
* Advanced notification system
* Improved team permissions
* File sharing
* Email notifications
* Meeting analytics dashboard
* Improved WebRTC scalability
* Automated testing
* CI/CD pipeline

---

# 📈 Project Highlights

```text
✔ Full-Stack MERN Application
✔ Real-Time Communication
✔ WebRTC Video Conferencing
✔ Socket.IO Messaging
✔ JWT Authentication
✔ MongoDB Database
✔ OpenAI Integration
✔ Team Collaboration
✔ Responsive UI
✔ Cloud Deployment
```

---

# 👨‍💻 Developer

## Gaurav Singh

**B.Tech — Information Technology**

Interested in:

* Full-Stack Development
* Software Engineering
* Data Analytics
* AI Engineering
* Backend Development

### Connect With Me

* **Portfolio:** https://gauravwebcv.netlify.app/
* **LinkedIn:** https://www.linkedin.com/in/gaurav-singh-28b217388
* **GitHub:** https://github.com/YOUR-USERNAME

---

# ⭐ Support

If you find this project useful or interesting, consider giving the repository a ⭐.

---

## 📄 License

This project is available under the MIT License.

See the `LICENSE` file for details.
