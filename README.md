# Falcons Employee Management System: Frontend

A web app for managing employees, projects, tasks, timesheets and leave, with separate **Admin** and **Employee** views.
This repo is the **React frontend**. The backend is **[falcons-employee-management-web-api](https://github.com/NadeeshPerera/falcons-employee-management-web-api)** (ASP.NET Core Web API).

![React](https://img.shields.io/badge/React_18-20232A?logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)
![MUI](https://img.shields.io/badge/MUI-007FFF?logo=mui&logoColor=white)
![DevExtreme](https://img.shields.io/badge/DevExtreme-FF7200)
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?logo=netlify&logoColor=white)

**UI demo:** https://loquacious-cucurucho-cb7e57.netlify.app/
> The cloud backend (Azure App Service + AWS RDS) was decommissioned after the project ended, so the hosted UI loads but data calls won't work. Run the API locally to try the full app.

## Features

**Admin**
- Employee management: add and update employee records, roles and status
- Project and task management: create projects and assign tasks to employees
- Leave management: view and manage employee leave requests
- Timesheet logs: view hours logged across the team

**Employee**
- My tasks: see assigned tasks and update their status
- Timesheet: log hours against tasks
- Leave requests: apply for leave and track approval
- Event calendar and team contacts

## Tech stack

| Area | Tools |
|---|---|
| UI | React 18, React Router 6, Material UI 5, DevExtreme |
| Data | Axios → REST API (ASP.NET Core) |
| Build | Vite |
| Hosting | Netlify (frontend), Azure App Service (API), AWS RDS SQL Server (DB) |

## Project structure

```
src/
├── Components/
│   ├── Admin/        # Employee, project, task, leave, timesheet management
│   ├── Employee/     # My tasks, timesheet, leave request
│   ├── Dashboard/    # Tile view
│   └── pages/        # Calendar, contacts
├── Admin.jsx · Dashboard.jsx · Login.jsx · Users.jsx
└── variables.jsx     # API base URL
```

## Run locally

```bash
npm install
npm run dev
```

Set `API_URL` in `src/variables.jsx` to your local API (for example `https://localhost:44325/api/`).

## Team Falcon

University group project (SLTC Research University, 2022). Team members:
K.S. Winodahewa · E.M.M.S. Ekanayaka · G.S.K. Abeywickrama · Nayani Nawarathne · R.M.J.N. Kumari Rajapaksha · Aqeel Ahamadh · S.A.S.A. Dissanayake · Tharushi Umayanga · M.M.R.Y.M.B. Amarathunga · **S.P.N.M. Perera (Nadeesh Perera)**
