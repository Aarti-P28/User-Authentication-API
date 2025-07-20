# 🛡️ User Authentication API

A simple Flask-based backend API for user registration and login with secure password hashing and JWT-based authentication. Ideal for learning or as a base for production-grade backend applications.

---

## 🚀 Features

- User Registration
- User Login with JWT Token Generation
- Secure Password Hashing (`pbkdf2:sha256`)
- Token-based Authentication Middleware
- SQLite Database Integration (via SQLAlchemy)

---

## 🛠️ Tech Stack

- Python 3.x
- Flask
- SQLAlchemy
- Werkzeug Security
- PyJWT
- SQLite

---

## ⚙️ Setup Instructions

 1. 🔃 Clone the Repository

    git clone https://github.com/your-username/User_auth_API.git
    cd User_auth_API

 2. 📦 Install Dependencies

    pip install -r requirements.txt

 3. ▶️ Run the Flask Serve

    python app.py
    
Server runs at: http://127.0.0.1:5000

---

## 🧪 API Testing (Using Postman)

🔐 Register a New User
Endpoint: POST /register
Body (JSON):
{
  "username": "admin",
  "password": "admin123"
}

🔑 Login
Endpoint: POST /login
Body (JSON):
{
  "username": "admin",
  "password": "admin123"
}
Returns: JWT Token

🔒 Protected Route Example (Requires Token)
Endpoint: GET /protected
Headers: 
        Authorization: Bearer <your_token_here>

---

## 🛡️ Security Notes

Make sure to change SECRET_KEY in app.py before production.

Do not upload users.db if using real user data.

Use HTTPS in real-world deployments.



---

## ✅ Requirements

Python 3.8+

Flask

SQLAlchemy

PyJWT

Werkzeug

Install all with: pip install -r requirements.txt

Or using: pip install flask sqlalchemy pyjwt werkzeug

---
