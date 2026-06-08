# 💬 EchoChat: Full-Stack Real-Time Messaging Architecture

A robust, full-stack web application designed to facilitate seamless, bidirectional real-time communication. Engineered with a strict focus on low-latency messaging, secure authentication, and a scalable UI architecture.

## 🚀 Technical Stack & Architecture

| Layer | Technologies Used |
| :--- | :--- |
| **Frontend UI** | React.js, Tailwind CSS, DaisyUI |
| **State Management** | Zustand (for optimized, re-render-free global state) |
| **Backend API** | Node.js, Express.js |
| **Database** | MongoDB, Mongoose |
| **Real-Time Engine** | Socket.io (WebSockets) |
| **Security & Auth** | JSON Web Tokens (JWT), Bcrypt |

## ✨ System Features

* **Secure Authentication Flow:** End-to-end user registration and login workflows protected by JWT-based authorization and strictly encrypted user credentials.
* **Real-Time Bi-Directional WebSockets:** Instant message delivery, typing indicators, and reception powered by optimized Socket.io events.
* **Live Presence Tracking:** Real-time online/offline status indicators for active users dynamically synced across all active client instances.
* **Optimized Global State:** Centralized frontend state management utilizing Zustand to prevent unnecessary component re-renders and manage message caching.
* **Centralized Error Handling:** Comprehensive server-side middleware and client-side error catching to ensure a crash-free user experience.
* **Responsive UI/UX:** Fully responsive, accessible, and modern interface built entirely with utility-first Tailwind CSS.

## 🛠️ Local Development Setup

Follow these instructions to configure and run the application locally.

### 1. Environment Configuration

Create a `.env` file in the root directory and configure the following environment variables:

```env
# Server Configuration
PORT=5001
NODE_ENV=development

# Database Connection
MONGODB_URI=<your_mongodb_connection_string>

# Security Secrets
JWT_SECRET=<your_secure_jwt_secret>

# Media Storage (Cloudinary)
CLOUDINARY_CLOUD_NAME=<your_cloud_name>
CLOUDINARY_API_KEY=<your_api_key>
CLOUDINARY_API_SECRET=<your_api_secret>
```

### 2. Installation & Execution

Install the necessary dependencies and boot up both the client and server environments:

```bash
# Install dependencies for both frontend and backend
npm install

# Build the application for production optimization
npm run build

# Boot up the server
npm start