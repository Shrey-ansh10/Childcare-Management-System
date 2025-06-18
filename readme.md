# EduEase: Childcare & School Management Platform

## Overview
EduEase is a comprehensive full-stack web application designed to streamline and manage the operations of childcare facilities and schools. It provides features for staff, parents, and administrators to handle daily activities such as child enrollment, attendance tracking, staff management, accounting, and reporting.

## Project Structure

- **Backend/**: Node.js/Express server handling authentication, business logic, and API endpoints.
  - `App.js`: Main server entry point.
  - `globalFunctions.js`, `loginFunctions.js`: Utility and authentication logic.
  - `package.json`: Backend dependencies and scripts.
  - `azure-pipelines.yml`: Azure DevOps pipeline configuration.

- **Frontend/**: React application built with Vite for a fast development experience.
  - `index.html`: Main HTML file.
  - `vite.config.js`: Vite configuration.
  - `package.json`: Frontend dependencies and scripts.
  - `src/`: Main source code directory.
    - `App.jsx`, `main.jsx`: App entry points.
    - `Pages/`: Contains feature-specific React components:
      - **AccountingLedger**: Ledger and accounting management.
      - **Admin**: Admin dashboard and login.
      - **Attendance**: Staff attendance tracking.
      - **Dashboard**: Main dashboard for users.
      - **EnrollChild**: Child enrollment forms and logic.
      - **GlobalComponents**: Reusable UI components (e.g., text fields, login modal).
      - **Homepage**: Landing, login, and account creation pages.
      - **ManageClassroom**: Classroom management.
      - **ManageStaff**: Staff management.
      - **PersonalInformation**: Facility and parent information.
      - **Report**: Reporting and ledger reports.
      - **StudentAttendance**: Student attendance tracking.
    - `redux/`: State management using Redux.

## Features
- User authentication (admin, staff, parent)
- Child enrollment and personal information management
- Staff and student attendance tracking
- Classroom and staff management
- Accounting ledger and financial reporting
- Admin dashboard and reporting tools

## Getting Started

### Prerequisites
- Node.js (v16+ recommended)
- npm or yarn

### Backend Setup
1. Navigate to the `Backend` directory:
   ```bash
   cd Backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the `Frontend` directory:
   ```bash
   cd Frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the frontend development server:
   ```bash
   npm run dev
   ```
4. Open your browser and go to `http://localhost:5173` (default Vite port).

## Deployment
- Project was originally deployed on GCP.
- The project includes an `azure-pipelines.yml` for CI/CD with Azure DevOps. 
- For production builds, use `npm run build` in the `Frontend` directory.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Acknowledgements
- [React](https://react.dev/)
- [Vite](https://vitejs.dev/)
- [Node.js](https://nodejs.org/)
- [Express.js](https://expressjs.com/)
- [Redux](https://redux.js.org/)
- Google Cloud Platform (GCP)
