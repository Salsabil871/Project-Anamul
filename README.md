# Todo Master ✅

Todo Master is a simple yet practical task management web app with user authentication, task tracking, and a clean dashboard interface. It uses **Firebase Authentication** for login and registration, and a **Node.js + Express + MySQL** backend to store and manage tasks.

## ✨ Features

- Email and password registration/login
- Google Sign-In with Firebase
- User profile display after login
- Add new tasks with an optional due date
- View task stats:
  - Total Tasks
  - Completed
  - Pending
- Filter tasks by:
  - All
  - Pending
  - Completed
- Mark tasks as completed/uncompleted
- Delete tasks
- Logout support
- Responsive frontend UI

## 🛠️ Tech Stack

**Frontend**
- HTML
- CSS
- JavaScript
- Firebase Authentication

**Backend**
- Node.js
- Express.js
- MySQL
- mysql2
- cors
- dotenv

## 📁 Project Structure

```bash
Todo-Master/
├── backend/
│   ├── src/
│   │   ├── db.js
│   │   ├── server.js
│   │   └── routes/
│   ├── package.json
│   └── .env
├── frontend/
│   ├── index.html
│   ├── dashboard.html
│   ├── auth.js
│   ├── dashboard.js
│   ├── firebase.js
│   ├── style.css
│   └── ...
└── database/
```

## 🚀 How It Works

1. A user creates an account or signs in using Firebase Authentication.
2. After login, the app redirects to the dashboard.
3. The dashboard loads that user’s tasks from the backend API.
4. Tasks can be added, filtered, completed, or deleted.
5. Task data is stored in MySQL through the Express backend.

## ⚙️ Backend API

The frontend communicates with the backend using these API routes:

- `POST /api/register-user`
- `POST /api/add-task`
- `GET /api/tasks/:uid`
- `PUT /api/task/:id`
- `DELETE /api/task/:id`

## 🔧 Setup Instructions

### 1) Clone the repository
```bash
git clone https://github.com/Amit-Bhowmik/Todo-Master.git
cd Todo-Master
```

### 2) Set up the backend
Go to the `backend` folder and install dependencies:

```bash
cd backend
npm install
```

Create a `.env` file inside `backend/` and add your MySQL details:

```env
PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=todo_db
```

Then start the backend:

```bash
npm start
```

### 3) Set up Firebase
Open `frontend/firebase.js` and replace the Firebase config with your own project credentials.

### 4) Run the frontend
Open `frontend/index.html` in your browser, or use a local server such as VS Code Live Server.

## ✅ Learning Outcome

- Firebase authentication workflow
- Frontend and backend integration
- MySQL database connection
- CRUD operations for todo management
- Building a clean task dashboard with vanilla JavaScript

## 🔮 Future Improvements

- Add edit task functionality
- Add task priority labels
- Add reminders and notifications
- Support search and sort
- Add better mobile animations
- Add dark mode

## 👨‍💻 Author

**Amit Bhowmik**

---
Built with care for staying organized and getting things done.
