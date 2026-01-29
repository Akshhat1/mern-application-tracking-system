MERN Application Tracking System (ATS)
A full-stack Application Tracking System (ATS) built using the MERN stack that helps organizations manage job postings and track candidate applications efficiently.

📌 Overview
This project digitizes the hiring process by allowing employers to post jobs, candidates to apply, and recruiters to track applications through different stages.
It supports role-based access to ensure secure and organized workflows.

Features
Role-based authentication (Candidate, Recruiter, Employer, Coordinator)
Job posting and job management
Candidate job application tracking
Recruiter dashboard to review and update application status
Secure authentication using JWT
Responsive UI
🛠️ Tech Stack
Frontend

React
Redux
Tailwind CSS
Backend

Node.js
Express.js
Database

MongoDB (Mongoose)
Authentication

JSON Web Tokens (JWT)
⚙️ How It Works
Employers post job openings
Candidates register and apply for jobs
Recruiters review applications
Application status is updated (Applied → Shortlisted → Selected / Rejected)
Data is stored and managed securely in MongoDB
Installation
Clone the repository:

git clone https://github.com/Akshhat1/mern-application-tracking-system.git
cd mern-application-tracking-system
Install server dependencies:

cd server
npm install
Install client dependencies:

cd client
npm install
Create a .env file in the server directory and add the following:

MONGODB_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
Start the development server:

cd server
npm run dev
Start the client:

cd client
npm start
Usage/Examples
Navigate to http://localhost:3000 in your web browser.
Create a user account for each role (Candidate, Coordinator, Recruiter, Employer).
Use the application according to the role functionalities outlined in the SRS summary.
SRS Summary
Problem Statement
The task is to design an Applicant Tracking System (ATS) that manages job postings, receives applications, and creates a hiring workflow.

Users
Candidate: A job seeker who applies for jobs.
Coordinator: Manages job postings and recruitment workflows.
Recruiters: Screens candidates' resumes.
Employers: Creates job postings.
Job Posting Flow
Employer creates a job post, including a job description and an R1 check form.
Coordinator approves the job post, assigns recruiters, and adds an R2 check form.
Coordinator posts the job, making it live for candidates to apply.
Application Flow
Candidate creates an account, views job postings, and applies by uploading a resume and completing the R1 check form.
Recruiter reviews applications, completes the R2 check form, and shortlists candidates for the final stage.
Shortlisted applications appear in both employers' and coordinators' dashboards.
Additional Requirements
User account management with role-based access.
Basic security practices.
