# MERN‑Blog Project

> A full-stack blog application built with the MERN stack (MongoDB, Express.js, React, and Node.js), featuring user authentication, image uploads, draft/published statuses, and a clean user interface.

---

## 🚀 Features

- 🔐 JWT-based user authentication
- 📝 Create, Read, Update, and Delete blog posts
- ✍️ Draft and published status support
- 🖼 Image uploads for posts
- 🔒 Protected routes for editing/deleting by author only
- 📱 Responsive React UI with Hooks and Router
- 🔧 Clean backend using Express, MongoDB, and Mongoose

---

## 📁 Project Structure
mern-project/
├── backend/ # Express API server
│ ├── models/ # Mongoose schemas (e.g. Post, User)
│ ├── routes/ # API route handlers
│ └── server.js # App entry point
└── frontend/ # React client application
├── src/
│ ├── components/ # Reusable UI components
│ └── pages/ # Pages (e.g. Home, PostDetail, Create/Edit)
└── public/



---

## 🛠 Getting Started

### Prerequisites

- Node.js (v14+)
- MongoDB (local or Atlas)
- NPM or Yarn

### Backend Setup

```bash
cd backend
npm install


Create a .env file inside /backend with:

PORT=5001
MONGO_URI=mongodb://localhost:27017/mern-blog
JWT_SECRET=your_jwt_secret_here

Then run the backend:
npx nodemon server.js
Backend should run on: http://localhost:5001




Frontend Setup
bash
Copy code
cd frontend
npm install
npm start
Frontend should run on: http://localhost:3000

It proxies API requests to the backend.



🧪 Usage
Register a user and login (token is saved in localStorage)

Create new posts with title, content, category, image, and status

View all your posts in the dashboard (including drafts)

Edit and delete your own posts

Public users can see only published posts

📎 API Endpoints
Public
GET /api/posts — View posts

GET /api/posts/:id — View a single post

Protected (Requires JWT in headers)
POST /api/posts — Create a new post

PUT /api/posts/:id — Edit a post (author only)

DELETE /api/posts/:id — Delete a post (author only)

✅ Key Learnings
Authentication & authorization using JWT

File/image upload handling with Express

React Hooks & routing for navigation and state

Protected API routes in Express

Modular and scalable codebase separation

🔮 Future Enhancements
Markdown or rich text editing

Comments on blog posts

Like/share functionality

Pagination or infinite scrolling

Admin role for managing all posts

Deployment on Render / Vercel / Railway

🎓 Author
0007-web
🔗 GitHub: https://github.com/0007-web

📝 License
This project is open source under the MIT License.
Feel free to use it for your own learning or commercial projects.




---

Let me know if you'd like a deployment section added (e.g., for Render, Vercel, or Railway), or badges like build status, license, or live demo links.
