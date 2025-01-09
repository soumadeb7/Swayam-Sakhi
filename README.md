# Swayam-Sakhi
 Empowering Rural Women Through AI

# Architecture Diagram

**System Components:**
1. **Frontend:**
   - Mobile App (React Native)
   - Web Portal (React.js)
2. **Backend:**
   - Node.js with Express.js
   - Database: MongoDB (user data, course progress, transactions)
3. **APIs:**
   - REST APIs for frontend-backend communication
   - Third-party APIs for payment gateway (Razorpay/PayPal), analytics, and microfinance integration
4. **Integration:**
   - Partner Financial Institutions (for loans and payments)
   - Training Content Management System (CMS)
   - Analytical Tools (Google Analytics or custom ML models)

**Data Flow:**
1. User interacts with the **frontend**, inputs registration, or course data.
2. Data is sent to the **backend** using secure REST APIs.
3. Backend communicates with:
   - Database for storage/retrieval.
   - Third-party APIs for payments and loans.
4. Data is processed and sent back to the frontend for visualization or feedback.

---

# Flow Chart

**Steps:**
1. User Registration
   - Input: Name, Contact, Area of Interest
   - Output: Profile Created
2. Course Selection
   - Input: Browse Categories, Select Course
   - Output: Start Training
3. Training Progress
   - Input: Access Modules (Video, Text, Quizzes)
   - Output: Completion Status Updated
4. Loan Application
   - Input: Fill Loan Form, Submit
   - Output: Loan Processed
5. Product Sales
   - Input: Upload Products for Sale
   - Output: Marketplace Listings
6. Progress Dashboard
   - Input: Analyze User Activity
   - Output: Show Achievements/Opportunities

---

# Interface Code (React.js)

**Login/Register Component:**
```jsx
import React, { useState } from 'react';

function LoginRegister() {
  const [isLogin, setIsLogin] = useState(true);

  const toggleMode = () => setIsLogin(!isLogin);

  return (
    <div className="auth-container">
      <h2>{isLogin ? 'Login' : 'Register'}</h2>
      <form>
        {!isLogin && <input type="text" placeholder="Name" required />}
        <input type="email" placeholder="Email" required />
        <input type="password" placeholder="Password" required />
        <button type="submit">{isLogin ? 'Login' : 'Register'}</button>
      </form>
      <p onClick={toggleMode} style={{ cursor: 'pointer', color: 'blue' }}>
        {isLogin ? 'Don\'t have an account? Register' : 'Already have an account? Login'}
      </p>
    </div>
  );
}

export default LoginRegister;
```

**Dashboard Component:**
```jsx
import React from 'react';

function Dashboard() {
  return (
    <div className="dashboard">
      <h1>Welcome to Swayam Sakhi</h1>
      <div className="cards">
        <div className="card">Active Courses</div>
        <div className="card">Upcoming Modules</div>
        <div className="card">Financial Tools</div>
      </div>
    </div>
  );
}

export default Dashboard;
```

**Training Module Component:**
```jsx
import React from 'react';

function TrainingModule() {
  return (
    <div className="training-module">
      <h2>Module Title</h2>
      <video controls src="/path/to/video.mp4">Your browser does not support the video tag.</video>
      <button>Download Resources</button>
      <button>Take Quiz</button>
    </div>
  );
}

export default TrainingModule;
```
