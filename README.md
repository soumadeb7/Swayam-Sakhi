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
