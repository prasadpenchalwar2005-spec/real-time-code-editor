# 🚀 Real-Time Collaborative Code Editor

A real-time collaborative code editor where changes made in one browser window are instantly synchronized with another browser window.

## 🌐 Live Demo

**Live URL:**
http://dock-aws-learn-CS-125539470.ap-northeast-1.elb.amazonaws.com

> Open the application in two browser windows and start typing in one window. The changes will be reflected in the other window in real time.

## ✨ Features

* ⚡ Real-time code synchronization
* 🖥️ Monaco Editor integration
* 🔄 Multiple browser windows can collaborate
* 🔌 Real-time communication using Socket.IO
* 🎨 Responsive UI with Tailwind CSS
* 🐳 Dockerized application
* ☁️ Deployed on AWS

## 🛠️ Tech Stack

### Frontend

* React.js
* Monaco Editor
* Tailwind CSS
* Vite

### Backend

* Node.js
* Express.js
* Socket.IO

### Deployment & DevOps

* Docker
* AWS ECS
* AWS Load Balancer

## 📁 Project Structure

```text
DOCK-AWS/
│
├── Backend/
│   ├── public/
│   ├── server.js
│   ├── package.json
│   └── package-lock.json
│
├── Frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── package-lock.json
│
├── .dockerignore
├── .gitignore
├── dockerfile
└── README.md
```

## ⚙️ How to Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/prasadpenchalwar2005-spec/real-time-code-editor.git
```

### 2. Go into the project directory

```bash
cd real-time-code-editor
```

### 3. Install backend dependencies

```bash
cd Backend
npm install
```

### 4. Start the backend

```bash
npm run dev
```

### 5. Install frontend dependencies

Open another terminal:

```bash
cd Frontend
npm install
```

### 6. Start the frontend

```bash
npm run dev
```

Then open the local URL shown by Vite in your browser.

## 🐳 Docker

The application is containerized using Docker.

Build the Docker image:

```bash
docker build -t real-time-code-editor .
```

Run the container:

```bash
docker run -p 3000:3000 real-time-code-editor
```

The application can then be accessed at:

```text
http://localhost:3000
```

## ☁️ AWS Deployment

The application was deployed using Docker and AWS.

Deployment setup includes:

* Docker container
* AWS ECS
* ECS Task Definition
* ECS Service
* Application Load Balancer
* Target Group
* Health Checks

The deployed application is accessible through the AWS Load Balancer URL provided above.

## 🔄 How Real-Time Collaboration Works

The application uses **Socket.IO** for real-time communication.

```text
Browser 1
   │
   │ Code Change
   ▼
Socket.IO Server
   │
   │ Broadcast
   ▼
Browser 2
   │
   ▼
Updated Code
```

When code is changed in one browser, the change is sent to the server through Socket.IO and synchronized with the other connected browser.

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience with:

* Building real-time applications
* Socket.IO communication
* React and Node.js integration
* Monaco Editor
* Docker containerization
* AWS deployment
* ECS and Load Balancer setup
* Deploying a full-stack application to the cloud

## 👨‍💻 Author

**Prasad Penchalwar**

GitHub:
https://github.com/prasadpenchalwar2005-spec

---

⭐ If you found this project interesting, feel free to check out the repository!
