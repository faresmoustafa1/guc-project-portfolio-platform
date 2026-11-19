# GUC Project Portfolio Platform

A web platform for GUC students, instructors and employers. Students show their academic projects as portfolios, instructors supervise and endorse that work, and employers find talent and post internships. An admin panel handles moderation and verification.

Built by **Syntax Squad** for the Software Engineering course (Spring 2026).

### 🔗 [Live Demo](https://faresmoustafa1.github.io/guc-project-portfolio-platform/)

No setup needed: open the link and log in with one of the [demo accounts](#demo-accounts).

## Features

- **Authentication**: login, password reset, change password, employer sign-up with a verification step
- **Role-based access** for four roles: Student, Instructor, Employer and Admin
- **Profiles**: student, instructor and company profiles, plus an instructor search
- **Projects**: create and manage projects, view project details, team invitations
- **Discovery**: browse projects and student portfolios, save favourites
- **Internships**: employers post internships, students browse and apply
- **Messaging and notifications** between users
- **Admin panel**: dashboard, user and employer verification, courses, projects, appeals, link requests, flagged content and internships

## Tech Stack

- [React 19](https://react.dev/)
- [React Router 7](https://reactrouter.com/)
- [Vite](https://vite.dev/)
- ESLint

> **Note:** There is no backend yet. All data comes from a mock data store (`src/data/DummyDataStore.js`) and is saved in the browser's `localStorage`.

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) 20.19 or newer
- npm (comes with Node.js)

### Installation

```bash
git clone https://github.com/faresmoustafa1/guc-project-portfolio-platform.git
cd guc-project-portfolio-platform
npm install
```

### Run locally

```bash
npm run dev
```

Then open [http://localhost:5173](http://localhost:5173) in your browser.

### Available scripts

| Command           | Description                           |
| ----------------- | ------------------------------------- |
| `npm run dev`     | Start the development server          |
| `npm run build`   | Build the app for production (`dist/`) |
| `npm run preview` | Preview the production build          |
| `npm run lint`    | Run ESLint                            |

## Demo Accounts

You can log in with any of these mock accounts:

| Role       | Email / Username                  | Password   |
| ---------- | --------------------------------- | ---------- |
| Student    | `ahmed.hassan@student.guc.edu.eg` | `password` |
| Instructor | `dr.kamel@guc.edu.eg`             | `password` |
| Employer   | `hr@techcorp.com`                 | `password` |
| Admin      | `admin`                           | `admin123` |

To reset the demo data, clear the site's `localStorage` in your browser's developer tools.

## Project Structure

```
src/
├── components/      # Shared UI components (e.g. Navbar)
├── context/         # React context (authentication)
├── data/            # Mock data store
├── pages/
│   ├── admin/       # Admin panel pages
│   ├── auth/        # Login, sign-up, password pages
│   ├── courses/
│   ├── favorites/
│   ├── internships/
│   ├── invitations/
│   ├── messages/
│   ├── notifications/
│   ├── portfolios/
│   ├── profile/
│   └── projects/
├── App.jsx          # Routes and route guards
└── main.jsx         # App entry point
```

## License

This project was made for educational purposes as part of a university course.
