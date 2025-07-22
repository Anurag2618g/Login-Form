# 🔐 Modern Login App

A modern login application with:

- 💻 Frontend: **React.js**
- 🚀 Backend: **Express.js**
- 🛢️ Database: **MongoDB Atlas**
- ✅ Validation: **Joi**

## 🧰 Tech Stack

| Frontend | Backend | Database | Validation |
|----------|---------|----------|------------|
| React.js | Express | MongoDB Atlas | Joi |

---

## 📦 Features

- 🔐 User registration & login
- 🧾 Form validation using Joi
- 📦 API with Express Router
- 🌍 MongoDB Atlas integration
- 📬 JSON response structure
- 🛠 MVC Architecture

---

## 🚀 Getting Started

### Prerequisites

- Node.js & npm
- MongoDB Atlas account

### 📁 Folder Structure (MVC)

```
project-root/
├── models/
│ └── schemas.js
│ └── validations.js
├── routes/
│ └── user.js
├── constants/
│ └── response.js
├── server.js
├── .env
├── client/
│ └── App.jsx
└── README.md

```

### 🛠 Install

# Install backend deps
npm install

# Run backend
node server.js

# OR use nodemon
npx nodemon server.js


# 📮 API Endpoints
Method	Route	Description
GET	/api	Fetch all users
GET	/api/:id	Fetch user by ID
POST	/api/register	Register new user
POST	/api/login	Login existing user

# 🧪 Validation with Joi

const Joi = require('joi');

export const Register_Validation = Joi.object({
  name: Joi.string().required(),
  email: Joi.string().email().required(),
  password: Joi.string().min(6).required()
});

# 📚 Environment Variables

MONGO_URI = mongodb+srv://<your-cluster>
