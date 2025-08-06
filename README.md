# 🔐 Secure Encryption Portal

A secure, end-to-end encrypted chat and encryption tool built with Flask and Socket.IO. This project provides strong encryption mechanisms (AES-CTR, RSA, SHA-1) along with secure user authentication and real-time messaging.

---

## 🚀 Features

- 🔑 User registration & login with secure password hashing
- 🔐 End-to-end encrypted chat using AES-CTR and RSA
- 🧾 Digital signature generation and verification
- 🧪 SHA-1 hash generator
- 📡 Real-time chat using Flask-SocketIO
- 🌗 Light / Dark theme toggle
- 🌐 Language support: English & Arabic
- ⚙️ User settings: theme, language, notifications

---

## 🧠 Technologies Used

- Python 3
- Flask
- Flask-Login
- Flask-SocketIO
- SQLAlchemy (SQLite DB)
- PyCryptodome (AES)
- RSA (encryption/signatures)
- HTML / CSS / JavaScript (Vanilla)
- Bootstrap 5
- Font Awesome

---

## 🖥️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/secure-encryption-portal.git
cd secure-encryption-portal
```

### 2. Create a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` is missing, manually install:
```bash
pip install flask flask-socketio flask-sqlalchemy flask-login pycryptodome rsa
```

### 4. Run the application

```bash
python app.py
```

Then open your browser and visit:

```
http://localhost:5000
```

---

## 📂 Project Structure

```
.
├── app.py
├── routes.py
├── models.py
├── crypto_utils.py
├── cryptography.py
├── templates/
│   ├── auth_standalone.html
│   ├── dashboard.html
│   ├── chat.html
│   ├── encryption.html
│   ├── profile.html
│   ├── settings.html
│   └── about.html
├── static/
│   ├── css/
│   │   ├── auth_standalone.css
│   │   ├── dark-theme.css
│   │   └── style.css
│   └── js/
│       ├── main.js
│       └── auth_standalone.js
└── secure_chat.db  (auto-created)
```

---

## 🧪 Sample Accounts

You can register manually through the `/auth` route.

---

## 🛡️ Security Notes

- Passwords are hashed using `werkzeug.security`.
- Messages are encrypted with AES-256 (CTR mode).
- Each message is signed with RSA for integrity.
- SHA-1 is used for hash comparisons (demo purposes only).

---

## 📃 License

MIT License
