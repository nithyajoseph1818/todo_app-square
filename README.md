# MERN To-Do App

A simple **To-Do app** built using the **MERN** stack with **Vite** for the frontend.

## 🛠 Tech Stack
- **Frontend:** Vite + React.js
- **Backend:** Node.js + Express.js
- **Database:** MongoDB (Atlas or Local)
- **State Management:** useState, useEffect (React Hooks)
- **HTTP Requests:** Axios

## 🚀 Features
- Create, Read, Update, and Delete (CRUD) tasks
- Mark tasks as completed
- Organize tasks into lists
- Responsive and minimalist UI

---

## 📂 Project Structure
```
mern-todo-app/
├── backend/       # Node.js + Express Server
│   ├── models/    # Mongoose Models
│   ├── routes/    # API Routes
│   ├── server.js  # Main Server File
│   ├── .env       # Environment Variables
├── frontend/      # Vite + React
│   ├── src/       # React Components & Pages
│   ├── App.jsx    # Main App Component
│   ├── main.jsx   # React Entry Point
│   ├── index.css  # Global Styles
├── package.json   # Dependencies & Scripts
```

---

## 🛠 Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/nithyajoseph1818/todo_app-square.git
cd mern-todo-app
```

### 2️⃣ Backend Setup (Node.js + MongoDB)
```bash
cd backend
npm install
```

#### Configure Environment Variables
Create a `.env` file in the `backend/` folder and add:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

#### Run the Backend Server
```bash
nodemon server.js
# or
node server.js
```
Server will start at `http://localhost:5000`

### 3️⃣ Frontend Setup (Vite + React)
```bash
cd frontend
npm install
npm run dev
```
Frontend will be running at `http://localhost:5173`

---

## 🛠 API Endpoints
### 📌 Tasks CRUD Operations
| Method | Endpoint         | Description           |
|--------|-----------------|-----------------------|
| GET    | /todos          | Fetch all tasks      |
| POST   | /todos          | Add a new task       |
| PUT    | /todos/:id      | Update a task        |
| DELETE | /todos/:id      | Delete a task        |

---

## ⚠️ Troubleshooting

### 1️⃣ MongoDB Connection Error
- Ensure your **MongoDB Atlas connection string** is correctly set in `.env`
- If using **local MongoDB**, make sure it's running (`mongod`)

### 2️⃣ CORS Issues (Frontend not connecting to Backend)
- Add CORS middleware in `server.js`:
  ```js
  const cors = require('cors');
  app.use(cors());
  ```

### 3️⃣ Vite Issues (Frontend Not Loading)
- Try clearing cache and reinstalling dependencies:
  ```bash
  rm -rf node_modules package-lock.json
  npm install
  ```

---

## 🌟 Future Enhancements
- Add authentication (JWT)
- Implement drag-and-drop for task reordering
- Improve UI with TailwindCSS

## 📜 License
This project is **open-source** and free to use under the MIT License.

---

💡 **Happy Coding!** 🚀

