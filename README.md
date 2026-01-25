# MERN Todo List Application

A simple, elegant todo list application built with MongoDB, Express, React, and Node.js.

## Features

- ✅ Create new tasks
- 📋 View all tasks
- 🗑️ Delete tasks
- 🎨 Modern, responsive UI

## Project Structure

```
mern-todo/
├── client/                 # React frontend
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── App.js
│   │   ├── App.css
│   │   └── index.js
│   ├── .gitignore          # Git ignore file for client
│   └── package.json
├── server/                 # Node.js/Express backend
│   ├── models/
│   │   └── Task.js
│   ├── .env                # Environment variables (create this)
│   ├── .env.example        # Example environment file
│   ├── .gitignore          # Git ignore file for server
│   ├── server.js
│   └── package.json
├── .gitignore              # Root git ignore file
└── README.md
```

## Prerequisites

- Node.js (v14 or higher)
- MongoDB Atlas account or local MongoDB instance

## Installation

### 1. Clone or create the project structure

### 2. Setup Server

```bash
cd server
npm install
```

**Configure Environment Variables:**

1. Create a `.env` file in the `server` directory
2. Copy the contents from `.env.example`
3. Replace the MongoDB URL with your actual connection string:

```env
MONGODB_URL=mongodb+srv://your-username:your-password@your-cluster.mongodb.net/todoapp?retryWrites=true&w=majority
```

**Note:** The `.env` file is gitignored to keep your credentials safe.

### 3. Setup Client

```bash
cd ../client
npm install
```

## Running the Application

### Start the Server (from server directory)

```bash
npm start
```

Server runs on `http://localhost:5000`

### Start the Client (from client directory)

```bash
npm start
```

Client runs on `http://localhost:3000`

## API Endpoints

- `GET /api/tasks` - Get all tasks
- `POST /api/tasks` - Create a new task
- `DELETE /api/tasks/:id` - Delete a task

## Technologies Used

- **MongoDB** - Database
- **Express.js** - Backend framework
- **React** - Frontend library
- **Node.js** - Runtime environment
- **Mongoose** - MongoDB ODM
- **Axios** - HTTP client
- **CORS** - Cross-origin resource sharing
- **dotenv** - Environment variable management

## License

MIT