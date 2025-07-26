FREELANCEFINDER : DISCOVERING OPPORTUNITIES, UNLOCKING POTENTIAL

Full-stack FreelanceFinder with React frontend and Node.js backend.

Features

Freelancer: Create profile, browse job listings, submit proposals
Client: Post projects, review proposals, manage hires
Admin: Manage users, moderate content, analyze usage

Tech Stack

Frontend: React.js, CSS3, Axios
Backend: Node.js, Express.js, MongoDB, JWT

📹 Demo Video

Click here to watch the demo video (https://drive.google.com/file/d/1Mzt-tccZ-QYNE1Klxv8ge3LpP9HMOPAf/view?usp=drivesdk)

Installation
1. Clone & Install

git clone <repository-url>
cd freelance-finder
# Backend
cd backend && npm install
# Frontend  
cd frontend && npm install

2. Environment Setup
   
Backend .env:
MONGO_URI=mongodb://127.0.0.1:27017/freelance_finder
PORT=5000
JWT_SECRET=YOUR_JWT_SECRET
Frontend .env:
REACT_APP_API_URL=http://localhost:5000/api

3. Run Application
   
# Start MongoDB
mongod
# Terminal 1 - Backend
cd backend && nodemon index.js
# Terminal 2 - Frontend
cd frontend && npm start

Access URLs
Frontend: http://localhost:3000
Backend API: http://localhost:5000/api
Admin Panel: http://localhost:3000/admin
Client Dashboard: http://localhost:3000/client
Freelancer Dashboard: http://localhost:3000/freelancer

API Endpoints
POST   /api/auth/register       - Register user  
POST   /api/auth/login          - Login user  
GET    /api/jobs                - Get all job listings  
POST   /api/jobs/post           - Post a new job (client)  
POST   /api/proposals/submit    - Submit proposal (freelancer)  
GET    /api/dashboard           - Dashboard data  
PUT    /api/profile/update/:id  - Update profile

Project Structure

├── backend/
│   ├── models/         # Database schemas
│   ├── routes/         # API routes
│   ├── controllers/    # Business logic
│   └── server.js       # Main server file
├── frontend/
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── pages/       # Page components
│   │   └── App.js       # Main app
│   └── public/
└── README.md

Common Commands
Development:

# Backend dev mode
nodemon index.js
# Frontend dev mode
npm start
# Install dependencies
npm install

Contributing
 1.Fork repository
 2.Create feature branch
 3.Commit changes
 4.Push to branch
 5.Create Pull Request

License
MIT License
