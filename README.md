# 🚀 CIVITAS  
### Smart City Complaint Management and Analytics System

CIVITAS is a full-stack web application designed to streamline civic complaint management in smart cities. It enables citizens to report issues while allowing administrators and staff to manage, track, and resolve complaints efficiently through a centralized platform.

---

## 📌 Features

- 👤 User Authentication (JWT-based)
- 🧑‍💼 Role-Based Access (Citizen, Staff, Admin)
- 📝 Complaint Submission with Location
- ⚡ Automated Priority Calculation
- 📊 Real-Time Analytics Dashboard
- ⏱ SLA Monitoring & Breach Detection
- 💬 Comment & Status Tracking System
- 📈 Department Performance Insights

---

## 🛠 Tech Stack

### Frontend
- React.js  
- Tailwind CSS  
- Axios  

### Backend
- Node.js  
- Express.js  

### Database
- MongoDB Atlas  

### Security
- JWT Authentication  
- bcrypt Password Hashing  

---

## 🏗 Architecture

The application follows a three-tier architecture:

- **Presentation Layer** → React.js  
- **Application Layer** → Node.js + Express.js  
- **Data Layer** → MongoDB Atlas  

---

## ⚙️ Installation and Setup

Follow these steps to run the project locally on your system.

---

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/civitas.git
cd civitascd server
npm install
cd client
npm install
npm run dev
