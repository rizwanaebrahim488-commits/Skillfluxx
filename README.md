# Skillflux

🌟 SkillFlux
Peer-to-Peer Skill Exchange Platform
📌 Project Overview
SkillFlux is a peer-to-peer skill exchange platform that enables users to teach and learn skills using a credit-based system.
Instead of paying money, users earn credits by teaching and spend credits to learn. The platform supports multi-session learning, credit transfers, and both online and offline skill exchanges.
SkillFlux is designed especially to empower local and rural communities where access to structured learning platforms is limited.
🚀 Problem Statement
Many people have valuable skills but lack visibility or opportunities to share them.
At the same time:
Learners struggle to find trusted skill providers.
Existing platforms focus mostly on urban users.
Most systems support only one-time exchanges.
There is no proper incentive or structured tracking system.
💡 Solution
SkillFlux solves this by providing:
✅ Peer-to-peer skill exchange
✅ Credit-based earning & spending model
✅ Multi-session learning support
✅ Online (Google Meet/Zoom) & offline session support
✅ Session tracking system
✅ Credit transfer between users
✅ Transparent and scalable structure
🎯 Key Features
1️⃣ User Authentication
Email & Password registration
Secure login using Firebase Authentication
2️⃣ Credit System
Users start with 2 default credits
Earn credits by teaching
Spend credits when learning
Transfer credits to friends/family
3️⃣ Skill Management
Add skills you can teach
Request skills you want to learn
Match with providers
4️⃣ Multi-Session Learning
Each session includes:
Date & Time
Meeting Link (Google Meet / Zoom)
Status (Pending / Completed)
Credit updates per session
5️⃣ Dashboard
View total credits
View skills
Track requests
Monitor session progress
🏗️ Tech Stack
Layer
Technology
Frontend
HTML, CSS, JavaScript
Backend
Firebase Authentication
Database
Firebase Firestore
Hosting
Firebase Hosting / GitHub Pages
Online Sessions
Google Meet / Zoom links
📂 Project Structure
Copy code

skillflux/
├── index.html          # Login Page
├── register.html       # Registration Page
├── dashboard.html      # User Dashboard
├── css/
│     └── style.css
└── js/
      ├── firebase-config.js
      ├── auth.js
      └── dashboard.js
🗄️ Firestore Database Structure
Users Collection
Copy code

users (collection)
 └── userId (document)
       ├── name
       ├── email
       ├── skills (array)
       ├── credits (number)
       └── createdAt (timestamp)
Requests Collection
Copy code

requests (collection)
 └── requestId (document)
       ├── skill
       ├── learnerId
       ├── providerId
       ├── status (pending/completed)
       ├── sessionLink
       └── createdAt
Transfers Collection (Optional)
Copy code

transfers (collection)
 └── transferId
       ├── fromUserId
       ├── toUserId
       ├── credits
       └── createdAt
⚙️ Setup Instructions (Without VS Code)
Step 1: Create Firebase Project
Go to Firebase Console
Create project → Name: SkillFlux
Click Web Icon (</>) → Register app
Copy Firebase config
Step 2: Add Firebase SDK
Include in all HTML files:
Html
Copy code
<script src="https://www.gstatic.com/firebasejs/9.22.0/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/9.22.0/firebase-auth-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/9.22.0/firebase-firestore-compat.js"></script>
<script src="js/firebase-config.js"></script>
Step 3: Configure Firebase
In firebase-config.js:
Javascript
Copy code
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};

firebase.initializeApp(firebaseConfig);
const auth = firebase.auth();
const db = firebase.firestore();
Step 4: Deploy
Option 1: Firebase Hosting
Hosting → Manual Upload
Upload entire folder
Get live URL
Option 2: GitHub Pages
Upload project to GitHub
Enable Pages from Settings
Site goes live
🔄 Application Flow
User registers
User adds skills
User requests skill
Provider accepts
Session conducted
Credits updated
Progress tracked
🌍 Target Audience
Students
Freelancers
Hobbyists
Rural communities
Skill trainers
🌟 Unique Differentiators
Structured credit system
Multi-session tracking
Rural & offline support
Transparent peer-to-peer system
Lightweight & serverless
🔮 Future Improvements
AI-based skill matching
Leaderboard system
WebRTC built-in video calls
Mobile app version
Rating & review analytics
🏆 One-Line Pitch
SkillFlux is a peer-to-peer credit-based skill exchange platform that enables communities to teach, learn, and grow together through structured multi-session learning and transparent credit tracking.
