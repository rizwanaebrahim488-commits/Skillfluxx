# Skillflux
# 🌟 SkillFlux  
## Peer-to-Peer Credit-Based Skill Exchange Platform

---

## 📌 Overview

SkillFlux is a peer-to-peer skill exchange platform that enables users to teach and learn skills using a structured credit-based system.

Users earn credits by teaching skills and spend credits to learn new ones. The platform supports multi-session learning, credit transfers, and both online and offline exchanges.

SkillFlux is designed to empower students, freelancers, and especially local and rural communities where access to structured learning platforms is limited.

---

## 🚀 Problem Statement

Many people have valuable skills but lack visibility or opportunities to share them.

At the same time:

- Learners struggle to find trusted skill providers  
- Most platforms focus only on urban users  
- Skill exchanges are usually one-time only  
- There is no structured incentive system  

---

## 💡 Solution

SkillFlux provides:

- Peer-to-peer skill exchange  
- Credit-based earning & spending system  
- Multi-session learning support  
- Online (Google Meet/Zoom) & offline session support  
- Credit transfer between users  
- Transparent session tracking  

---

## 🎯 Key Features

### 1️⃣ Authentication
- Email & password login  
- Firebase Authentication integration  

### 2️⃣ Credit System
- Users start with 2 default credits  
- Earn credits by teaching  
- Spend credits by learning  
- Transfer credits to other users  

### 3️⃣ Skill Management
- Add skills you can teach  
- Request skills to learn  
- Match with providers  

### 4️⃣ Multi-Session Support
Each session includes:
- Date & time  
- Meeting link (Google Meet / Zoom)  
- Status (Pending / Completed)  
- Automatic credit update per session  

### 5️⃣ Dashboard
- View available credits  
- Track sessions  
- Monitor requests  
- View skill progress  

---

## 🏗️ Tech Stack

Frontend: HTML, CSS, JavaScript  
Backend: Firebase Authentication  
Database: Firebase Firestore  
Hosting: Firebase Hosting / GitHub Pages  
Sessions: Google Meet / Zoom links  

---

## 📂 Project Structure

skillflux/
│
├── index.html
├── register.html
├── dashboard.html
│
├── css/
│   └── style.css
│
└── js/
    ├── firebase-config.js
    ├── auth.js
    └── dashboard.js

---

## 🗄️ Firestore Database Structure

### Users
