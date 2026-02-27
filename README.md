# bitbug
Hackathon Project

# 🤖 AI Academic Risk Prediction System

An AI-powered full-stack web application that predicts whether a student is at **Low Risk**, **Medium Risk**, or **High Risk** of academic failure based on performance indicators.

This system helps institutions identify struggling students early and take preventive action.

---

## 🚀 Project Overview

This project is built using:

- ⚛ React (Frontend)
- 🟢 Node.js + Express (Backend API)
- 🐍 Python Flask (Machine Learning API)
- 📊 Scikit-learn (Logistic Regression Model)
- 🗄 MySQL (Optional for data storage)

The system analyzes:

- Attendance percentage
- Internal marks percentage
- Assignment completion percentage

And returns:

- Risk Level
- AI-based academic suggestion

---

## 🏗 Project Structure

```
ai-academic-risk-system/
│
├── frontend/        # React frontend
├── backend/         # Node.js API server
└── ml-model/        # Python ML model + Flask API
```

---

## 🧠 How It Works

1. User enters student academic data in React UI.
2. React sends data to Node.js backend.
3. Backend forwards data to Python Flask ML API.
4. Logistic Regression model predicts risk level.
5. Risk result is returned to frontend.
6. Result is displayed with color indicator and suggestion.

---

## 🎯 Features

✅ AI-based risk prediction  
✅ Simple and clean dashboard UI  
✅ Risk classification (Low / Medium / High)  
✅ Academic improvement suggestion  
✅ History tracking (last analyses)  
✅ Optional MySQL database storage  

---

## 🛠 Installation Guide

### 1️⃣ Clone the Repository

```bash
git clone <your-repo-url>
cd ai-academic-risk-system
```

---

# 🐍 Setup ML Model (Python)

### Go to ML folder

```bash
cd ml-model
```

### Create virtual environment (recommended)

```bash
python -m venv venv
venv\Scripts\activate   # Windows
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Train the model (only first time)

```bash
python train_model.py
```

This generates:
```
risk_model.pkl
```

### Start Flask ML API

```bash
python app.py
```

Runs on:
```
http://localhost:5000
```

---

# 🟢 Setup Backend (Node.js)

### Go to backend folder

```bash
cd backend
```

### Install dependencies

```bash
npm install
```

### Start backend server

```bash
node server.js
```

Runs on:
```
http://localhost:4000
```

---

# ⚛ Setup Frontend (React)

### Go to frontend folder

```bash
cd frontend
```

### Install dependencies

```bash
npm install
```

### Start React app

```bash
npm start
```

Runs on:
```
http://localhost:3000
```

---

## 🔄 Application Flow

```
React (3000)
    ↓
Node Backend (4000)
    ↓
Flask ML API (5000)
    ↓
Machine Learning Model
```

---

## 📊 Risk Classification Logic

| Risk Level   | Meaning |
|-------------|----------|
| 🟢 Low Risk | Student performance is stable |
| 🟠 Medium Risk | Needs monitoring and improvement |
| 🔴 High Risk | Immediate academic intervention recommended |

---

## 🧪 Example Input

```
Attendance: 45
Marks: 38
Assignments: 40
```

Output:
```
High Risk
Suggestion: Immediate academic counseling recommended.
```

---

## 🗄 Optional MySQL Database

If enabled, the system can store:

- Attendance
- Marks
- Assignments
- Risk level
- Timestamp

Table structure:

```sql
CREATE TABLE students_analysis (
    id INT AUTO_INCREMENT PRIMARY KEY,
    attendance INT,
    marks INT,
    assignments INT,
    risk VARCHAR(50),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

---

## 🔒 Future Improvements

- Add student login authentication
- Add faculty dashboard
- Add graphical analytics (charts)
- Connect real academic data
- Deploy to cloud (Render / Railway / AWS)
- Improve ML accuracy with larger dataset

---

## 🧠 Why This Project is Valuable

✔ Beginner-friendly AI integration  
✔ Full-stack architecture  
✔ Real-world academic application  
✔ Hackathon-ready concept  
✔ Expandable into SaaS product  

---

## 📌 Tech Stack Summary

| Layer | Technology |
|--------|------------|
| Frontend | React |
| Backend | Node.js + Express |
| ML API | Python Flask |
| ML Model | Logistic Regression |
| Database | MySQL (Optional) |

---

## 👨‍💻 Author

Your Name  
AI Academic Risk Prediction System  

---

## 📄 License

This project is for educational and demonstration purposes.
