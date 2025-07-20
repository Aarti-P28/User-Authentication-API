# User Authentication API (Flask + SQLite + JWT)

### Features:
- User Registration
- User Login
- JWT-based Authentication
- Protected Route (`/profile`)

### Setup Instructions:
```bash
pip install -r requirements.txt
python app.py
```

### API Endpoints:
- `POST /register`: `{ "username": "user1", "password": "pass123" }`
- `POST /login`: `{ "username": "user1", "password": "pass123" }` → returns JWT token
- `GET /profile`: Header `x-access-token: <JWT>` → returns user info