# Apna Video Calling App 🎥📞

A real-time video calling application with chat functionality, built using Node.js, Express, Socket.IO, MongoDB, and WebRTC.

## ✨ Features

- 🔐 User Authentication (Register/Login)
- 📹 Real-time Video Calling
- 💬 In-call Chat Messaging
- 📊 Meeting History Tracking
- 🏠 Room-based Video Conferencing
- 🔒 Secure Token-based Authentication

## 🛠️ Tech Stack

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **Socket.IO** - Real-time communication
- **MongoDB** - Database
- **Mongoose** - ODM
- **bcrypt** - Password hashing

### Frontend
- **React.js** - UI library
- **Socket.IO Client** - Real-time client
- **WebRTC** - Peer-to-peer video/audio

## 📦 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- MongoDB Atlas account
- npm or yarn

### Backend Setup

1. Navigate to backend folder:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env` file in backend folder:
```env
PORT=8000
MONGO_URI=your_mongodb_connection_string
NODE_ENV=development
```

4. Start backend server:
```bash
npm run dev
```

Server will run on `http://localhost:8000`

### Frontend Setup

1. Navigate to frontend folder:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start frontend:
```bash
npm start
```

Frontend will run on `http://localhost:5173` (Vite) or `http://localhost:3000` (CRA)

## 🌐 API Endpoints

### Authentication
- `POST /api/v1/users/register` - Register new user
- `POST /api/v1/users/login` - Login user

### Meeting History
- `GET /api/v1/users/get_all_activity?token=USER_TOKEN` - Get user's meeting history
- `POST /api/v1/users/add_to_activity` - Add meeting to history



## 🔌 Socket.IO Events

### Client to Server
- `join-call` - Join a video call room
- `signal` - WebRTC signaling
- `chat-message` - Send chat message
- `leave-call` - Leave the call
- `disconnect` - User disconnected

### Server to Client
- `user-joined` - New user joined the room
- `user-left` - User left the room
- `chat-message` - Receive chat message
- `signal` - WebRTC signaling response

## 🚀 Deployment

### Backend (Render)
1. Push code to GitHub
2. Connect repository to hosting platform
3. Set environment variables
4. Deploy

### Frontend (Render)
1. Build frontend: `npm run build`
2. Deploy `dist` or `build` folder
3. Update API endpoints to production URL


## 🙏 Acknowledgments

- Socket.IO for real-time communication
- WebRTC for peer-to-peer video
- MongoDB Atlas for database hosting

---

⭐ If you like this project, please give it a star on GitHub!
