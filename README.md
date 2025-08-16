# 🧠 Real-Time User Monitoring & Admin Control System

A powerful, production-grade user tracking system that monitors user login activity, session duration, and allows admins to control user accounts in real time.

---

## 🔧 Features

✅ Real-time login/logout tracking  
✅ Session duration calculation  
✅ Admin dashboard to view all user sessions  
✅ Account deactivation/reactivation by admin  
✅ Access control for deactivated users  
✅ Backend-agnostic SQL schema (can integrate with Node.js, Flask, Django, etc.)

---

## 🧱 Database Schema

### 📁 `users` Table

```sql
CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    email VARCHAR(255) UNIQUE NOT NULL,
    name VARCHAR(255),
    password_hash TEXT,
    is_active BOOLEAN DEFAULT TRUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

## Follow the steps below to set up and run the project on your local machine:

1️⃣ Clone the Repository

If you haven’t already, clone the repo from GitHub:

git clone https://github.com/YOUR_USERNAME/Complaint-Management-System.git


Then navigate into the project folder:

cd Complaint-Management-System

2️⃣ Install Dependencies

Install all required packages:

npm install

3️⃣ Start the Development Server

Run the project in development mode:

npm run dev

4️⃣ Open in Browser

After starting, the project will automatically open in your default browser.
If not, you can manually open:

http://localhost:8080/
