# 🎓 SmartGroup AI
### Automatic Student Group Creator System

---

## 📌 Overview

SmartGroup AI is an intelligent automation system designed to automatically create balanced and optimized student project groups in colleges and universities.

Instead of manually dividing students into teams — which often leads to imbalance, bias, and inefficiency — SmartGroup AI uses algorithms to generate fair, skill-balanced, and constraint-aware groups in seconds.

---

## 🚨 Problem Statement

Faculty members currently:

- Manually divide students into groups
- Try to balance CGPA and skill levels
- Avoid friendship bias
- Prevent repeating the same team combinations
- Adjust groups when students drop out

This process is:
- Time-consuming
- Error-prone
- Subjective
- Difficult to manage for large classes

---

## 🎯 Solution

SmartGroup AI automates the entire group formation process using:

- CGPA-based balancing
- Skill-based distribution
- Diversity constraints
- Conflict avoidance rules
- Previous grouping history tracking

Faculty only need to:

1. Upload student data
2. Select group size
3. Define constraints
4. Click "Generate Groups"

The system automatically produces optimized teams.

---

## ⚙️ Core Features

### 1️⃣ Balanced Academic Distribution
Ensures each group has a mix of high, medium, and low CGPA students.

---

### 2️⃣ Skill-Based Team Formation
Distributes skills evenly across groups (e.g., coding, documentation, presentation, AI/ML).

---

### 3️⃣ Constraint Management
Faculty can define:

- Do-not-pair students
- Gender balance requirement
- Avoid previous team repetition
- Custom rules

---

### 4️⃣ Automatic Role Assignment
System assigns roles inside each group:

- Team Leader
- Developer
- Documentation Lead
- Presenter

---

### 5️⃣ Dynamic Reallocation
If a student drops or is absent, the system automatically rebalances affected groups.

---

### 6️⃣ Group Quality Score
Each generated group receives:

- Balance Score
- Skill Coverage Percentage
- Diversity Score

---

## 🧠 Algorithm Approach

### Basic Version (Hackathon Ready)
- Sort students by CGPA
- Distribute in round-robin pattern
- Apply skill balancing
- Enforce constraints

### Advanced Version
- Genetic Algorithm Optimization
- Fitness function minimizes:
  - CGPA variance
  - Skill imbalance
  - Conflict violations
  - Repeated grouping

---

## 🏗️ Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Chart.js (for analytics)

### Backend
- Python (FastAPI / Django)
- REST API architecture

### Database
- PostgreSQL / MySQL

### Optional Enhancements
- Machine Learning for compatibility prediction
- Personality-based matching

---

## 📊 System Architecture

User Interface → Backend API → Group Formation Engine → Database → Output Generator

---

## 📂 Database Schema (Simplified)

### Students
- student_id
- name
- cgpa
- skills
- gender
- previous_groups

### Groups
- group_id
- semester
- project_title

### GroupMembers
- group_id
- student_id

### Constraints
- avoid_pair_student1
- avoid_pair_student2

---

## 🔐 Fairness & Transparency

- Eliminates favoritism
- Prevents biased grouping
- Provides explainable group allocation
- Maintains audit logs

---

## 🚀 Future Enhancements

- AI Compatibility Scoring
- Personality-based grouping
- Real-time collaboration insights
- Integration with LMS systems
- Performance tracking per group

---

## 🎓 Use Cases

- Mini Projects
- Final Year Projects
- Lab Grouping
- Hackathon Team Formation
- Classroom Activities

---

## 💡 Impact

- Saves faculty time
- Ensures fair team distribution
- Improves project performance
- Reduces complaints
- Scales for large institutions

---

## 🏆 Why This Project Matters

Team formation directly affects:

- Student learning
- Project success
- Team collaboration
- Academic fairness

SmartGroup AI transforms a manual academic process into an intelligent automated system.

---

## 📜 License

This project is developed for academic and research purposes.