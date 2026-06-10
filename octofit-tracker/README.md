# OctoFit Tracker - Modern Multi-Tier Application

A modern fitness tracking application built with React 19, Vite, Node.js, Express, and MongoDB.

## Project Structure

```
octofit-tracker/
├── frontend/     # React 19 + Vite frontend application
├── backend/      # Node.js + Express + TypeScript API server
```

## Port Configuration

- **Frontend**: `5173` (Vite dev server)
- **Backend**: `8000` (Express API server)
- **MongoDB**: `27017` (MongoDB database)

## Prerequisites

- Node.js (v18+)
- npm (v9+)
- MongoDB running on port 27017

## Getting Started

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend will be available at: `http://localhost:5173`

### Backend Setup

```bash
cd backend
npm install
npm run dev
```

Backend will be available at: `http://localhost:8000`

### Environment Configuration

1. **Backend** - Create `.env` file in `backend/` directory:
   ```
   MONGODB_URI=mongodb://localhost:27017/octofit-tracker
   PORT=8000
   NODE_ENV=development
   ```

2. **Frontend** - Create `.env.local` file in `frontend/` directory:
   ```
   VITE_API_URL=http://localhost:8000
   ```

See `.env.example` files in each directory for reference.

## Dependencies

### Frontend
- React 19
- Vite 8
- ESLint

### Backend
- Express 5
- TypeScript
- Mongoose (MongoDB ODM)
- ts-node (TypeScript execution)
- nodemon (Auto-reload)
- @types/node, @types/express (Type definitions)

## Development

### Frontend Development
```bash
cd frontend
npm run dev          # Start dev server
npm run build        # Build for production
npm run preview      # Preview production build
```

### Backend Development
```bash
cd backend
npm run dev          # Start with auto-reload
npm run build        # Compile TypeScript
npm start            # Run compiled code
```

## Health Check

Backend health check endpoint: `http://localhost:8000/health`

## MongoDB Connection

The backend automatically connects to MongoDB at startup. Ensure MongoDB is running before starting the backend server.

Connection string: `mongodb://localhost:27017/octofit-tracker`

## License

ISC
