# DineFlow

A modern restaurant reservation and waitlist platform built with Next.js, Express, TypeScript, and MongoDB.

DineFlow helps guests book tables, manage waitlists, and navigate restaurant availability with a polished frontend experience and a secure backend API.

## Features

- Reservation flow for guests
- Waitlist management
- Table overview and booking status
- Admin-friendly dashboard interface
- JWT-based authentication
- MongoDB persistence
- Monorepo setup using npm workspaces

## Tech Stack

- Frontend: Next.js, React, TypeScript, Tailwind CSS
- Backend: Express.js, TypeScript, MongoDB, Mongoose
- Auth: JWT + bcryptjs
- Dev tooling: npm workspaces, concurrently, nodemon

## Project Structure

- `frontend/` – Next.js app
- `backend/` – Express API and MongoDB integration
- `package.json` – root workspace scripts

## Getting Started

### Prerequisites

- Node.js 18+
- npm
- MongoDB instance or MongoDB Atlas connection string

### 1. Clone the repository

```bash
git clone https://github.com/Aryan3356/summer-term.git
cd summer-term
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Copy the example environment file and update the values:

```bash
copy .env.example .env
```

Then edit `.env` with your MongoDB URI and secret values:

```env
PORT=5001
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_EXPIRE=7d
NODE_ENV=development
CLIENT_ORIGIN=http://localhost:3000
```

### 4. Run the app

```bash
npm run dev
```

This will start:

- Frontend at `http://localhost:3000`
- Backend at `http://localhost:5001`

## Available Scripts

From the root workspace:

```bash
npm run dev
npm run frontend
npm run backend
npm run build
```

## Notes

- The backend loads environment variables from the root `.env` file.
- The project uses npm workspaces to manage both frontend and backend in one repository.

## License

ISC
