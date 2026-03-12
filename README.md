# library-management

![React](https://img.shields.io/badge/React-19-black?style=flat-square&logo=react&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5.7-black?style=flat-square&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-6-black?style=flat-square&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-4-black?style=flat-square&logo=tailwindcss&logoColor=white)

A full-featured library management system with a React + TypeScript frontend, supporting three distinct user roles: **Admin**, **Manager**, and **Client (Member)**.

## Overview

This project is the frontend for the SE104 (Introduction to Software Engineering) course assignment. It provides a web-based interface for managing a library's books, users, borrowing operations, and more.

## Project Structure

```
library-management/
└── se104-fe/          # React + TypeScript frontend (Vite)
    ├── src/
    │   ├── pages/
    │   │   ├── admin/         # Admin: user list, user profiles
    │   │   ├── manager/       # Manager: borrow/receive, reports, book list, chat, rules
    │   │   └── client/        # Client: homepage, book detail, favorites, borrow history, profile, chat
    │   ├── components/        # Shared UI components (admin, client, auth, layout)
    │   ├── services/          # Axios API service layer
    │   ├── styles/            # Global and scoped styles (SCSS)
    │   └── types/             # TypeScript type definitions
    ├── public/
    ├── index.html
    └── vite.config.ts
```

## Features

### Client (Member)
- Browse and search books; view book details and author information
- Favorite books and view reading history
- Submit borrow requests and track active borrowings
- In-app chat with library staff
- Account registration, login, email verification, and password reset

### Manager
- Process borrow and return (receive) requests
- Manage the full book catalog and add new books
- View and generate borrowing reports
- Configure library rules and parameters
- Chat with members

### Admin
- Full user account management (view list, manage profiles)
- Access to all manager capabilities

## Tech Stack

| Category | Technology |
|---|---|
| Framework | React 19 |
| Language | TypeScript 5.7 |
| Build Tool | Vite 6 |
| Styling | Tailwind CSS 4, SCSS (Sass) |
| UI Components | Ant Design (v5) |
| Routing | React Router DOM v7 |
| HTTP Client | Axios |
| Charts | Recharts |
| Icons | React Icons |

## Getting Started

### Prerequisites

- Node.js >= 18
- npm or a compatible package manager

### Installation

```bash
cd se104-fe
npm install
```

### Development

```bash
npm run dev
```

The development server starts at `http://localhost:5173` by default.

### Build

```bash
npm run build
```

### Lint

```bash
npm run lint
```

## Environment Variables

The frontend expects a `.env.development` file inside `se104-fe/`. Create one based on the template and set the backend API base URL:

```env
VITE_API_URL=http://localhost:8080
```
