# Talent-Acquisition-System - AI-powered Recruitment Platform

Talent-Acquisition-System is an advanced AI-driven recruitment platform designed to optimize and automate the complete hiring lifecycle. It empowers HR teams and organizations to post job openings, manage applicants, evaluate candidate responses, schedule interviews, and monitor performance through insightful analytics.
The platform integrates secure authentication, smart workflows, and AI-powered tools that generate job descriptions, interview questions, and candidate assessments—making hiring faster, smarter, and more efficient.

Key Features
**Job Posting & Management**
Create, update, and organize job openings with role-specific criteria and structured details.
**Candidate Tracking Pipeline**
Seamlessly track applicants through multiple hiring stages (Applied → Screening → Shortlisted → Interview → Hired).
**Custom Application Builder**
Add tailored screening questions to filter applicants based on role-specific requirements.
**Interview Coordination**
Schedule, manage, and update interviews, with reminders and stage-based tracking.
**Analytics & Reporting Dashboard**
View hiring statistics, applicant flow, time-to-hire, and performance metrics.
**Secure User Access & Authentication**
Includes encrypted login, registration, and role-based permissions.
**AI-Generated Job Descriptions**
Automatically generate detailed job descriptions and role expectations using AI.
**AI-Generated Interview Questions**
Produce customized interview questions tailored to the job title and skill set.


## Tech Stack

### Frontend
- React with TypeScript
- Vite for build tooling
- shadcn-ui components
- Tailwind CSS for styling
- React Router for navigation
- Axios for API calls

### Backend
- Node.js with Express
- MySQL database with Sequelize ORM
- JWT authentication
- Express-validator for input validation

## Project Structure

```
hirer-mind/
├── src/                 # Frontend React application
│   ├── components/      # React components
│   ├── pages/          # Page components
│   ├── services/       # API services
│   ├── hooks/          # Custom React hooks
│   └── lib/            # Utility functions
├── backend/            # Node.js API server
│   ├── config/         # Configuration files
│   ├── middleware/     # Express middleware
│   ├── models/         # Sequelize models
│   └── routes/         # API routes
└── public/             # Static assets
```

## Getting Started

### Prerequisites
- Node.js (v14+)
- MySQL (v8+)
- npm

### Installation

1. Clone the repository
```bash
git clone <repository-url>
cd hirer-mind
```

2. Install dependencies
```bash
# Install frontend dependencies
npm install

# Install backend dependencies
cd backend
npm install
cd ..
```

3. Set up the database
```bash
# Create database and tables
mysql -u root -p < backend/database.sql
```

4. Configure environment variables
- Copy `backend/.env.example` to `backend/.env`
- Update database credentials and JWT secret
- Set `VITE_API_URL` in root `.env` file

5. Start the application
```bash
# Start both frontend and backend
npm run dev:all

# Or start separately
npm run dev      # Frontend (port 8080)
npm run backend  # Backend (port 5000)
```

## API Endpoints

- `/api/auth` - Authentication (login, register, password reset)
- `/api/jobs` - Job management
- `/api/candidates` - Candidate operations
- `/api/applications` - Application handling
- `/api/interviews` - Interview scheduling
- `/api/dashboard` - Analytics data

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License
