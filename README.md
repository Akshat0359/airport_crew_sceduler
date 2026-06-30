# Airport Crew Scheduler

<div align="center">
  <img src="https://img.shields.io/badge/React-19.0-blue?logo=react&logoColor=white" alt="React" />
  <img src="https://img.shields.io/badge/Node.js-Express-green?logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/PostgreSQL-Database-blue?logo=postgresql&logoColor=white" alt="Postgres" />
  <img src="https://img.shields.io/badge/Tailwind-CSS-06B6D4?logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
</div>

<br />

A comprehensive full-stack web application designed to streamline, automate, and optimize the scheduling and management of airline crew. Built with a modern tech stack, this application leverages linear programming and optimization algorithms to solve complex crew assignment logistical challenges.

## 🚀 Problem Statement

Efficiently assigning pilots, flight attendants, and ground crew to flights while respecting availability, labor regulations, and maximum work hours is a highly complex task. Manual scheduling often leads to operational bottlenecks, increased risk of human error, and employee fatigue. **Airport Crew Scheduler** aims to fully automate and optimize this process, ensuring optimal coverage, reducing costs, and improving overall operational efficiency.

## ✨ Key Features

- **Automated AI Scheduling:** Leverages linear programming (`glpk.js` and `javascript-lp-solver`) to auto-assign crew based on constraints and availability.
- **Role-Based Access Control (RBAC):** Distinct dashboards and permissions for Admins and Crew members.
- **Real-Time Dashboard:** Interactive analytics and visual overviews of daily flights, crew tasks, and schedules using Recharts.
- **Secure Authentication:** Robust login system powered by `Passport.js` (including Google OAuth2 and Local strategy), JWT, and `bcrypt`.
- **Flight & Task Management:** Create new flights, assign specific duties, and track work progress.
- **Modern & Responsive UI:** Clean, intuitive, and accessible user interface built with Tailwind CSS, Shadcn UI, and Material-UI.

## 🛠 Tech Stack

### Frontend
- **Framework:** React 19, React Router DOM
- **Styling:** Tailwind CSS, Shadcn UI, Material-UI (@mui)
- **Data Visualization:** Recharts
- **Icons:** Lucide React, MUI Icons

### Backend
- **Runtime:** Node.js, Express.js
- **Database:** PostgreSQL (via `pg`)
- **Authentication:** Passport.js, JSON Web Tokens (JWT), session management
- **Optimization Algorithms:** `javascript-lp-solver`, `glpk.js`

## 📂 Project Structure

```text
airport_crew_sceduler/
├── backend/                  # Node.js Express server
│   ├── aiml/                 # AI/ML helper scripts
│   ├── db/                   # Database configuration and queries
│   ├── ai_scheduling.js      # Linear programming assignment logic
│   ├── index.js              # Entry point for backend API
│   └── package.json          # Backend dependencies
├── public/                   # Static frontend assets
├── src/                      # React frontend source code
│   ├── components/           # Reusable UI components (Navbar, etc.)
│   ├── pages/                # Application views (Dashboard, Admin, Crew, etc.)
│   ├── App.js                # Main routing component
│   └── index.css             # Tailwind imports and global styles
├── package.json              # Frontend dependencies
└── tailwind.config.js        # Tailwind CSS configuration
```

## ⚙️ Setup and Installation

### Prerequisites
- [Node.js](https://nodejs.org/) (v16+)
- [PostgreSQL](https://www.postgresql.org/) installed and running locally

### 1. Clone the repository
```bash
git clone https://github.com/Akshat0359/airport_crew_sceduler.git
cd airport_crew_sceduler
```

### 2. Backend Setup
```bash
cd backend
npm install
```
- Create a `.env` file in the `backend` directory (copy from `.env.example`). Add your PostgreSQL credentials and JWT secret.
- Start the backend server:
```bash
node index.js
```

### 3. Frontend Setup
Open a new terminal window in the project root:
```bash
npm install
npm start
```
The application will be accessible at `http://localhost:3000`.

## 📖 Usage Guide

1. **Admin Login:** Log in with admin credentials to access the main management dashboard.
2. **Flight Creation:** Navigate to "New Flight" to add upcoming flight schedules.
3. **Crew Assignment:** Use the automated scheduling tool to optimally assign available crew members to flights based on defined constraints.
4. **Crew Portal:** Crew members can log in to view their assigned flights, schedules, and specific tasks via the dedicated crew dashboard.

## 🛡️ Security

If you discover any security vulnerabilities, please do not use the issue tracker. Refer to [SECURITY.md](SECURITY.md) for reporting guidelines.

## 🔮 Future Improvements

- **Mobile Application:** Develop a React Native mobile app for crew members to check schedules on the go.
- **Push Notifications:** Implement real-time alerts via SMS or Email for last-minute schedule changes.
- **External API Integrations:** Fetch real-time flight status and weather data from external aviation APIs.

## 👨‍💻 Author

**Akshat**
- GitHub: [@Akshat0359](https://github.com/Akshat0359)
- Email: [akshat.prabhakar5903@gmail.com](mailto:akshat.prabhakar5903@gmail.com)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
*If you find this project helpful, please consider giving it a ⭐ on GitHub!*
