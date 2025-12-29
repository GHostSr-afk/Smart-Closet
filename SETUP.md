# SmartCloset Setup Guide

## Quick Start

1. **Install Dependencies**
   ```bash
   npm run install:all
   ```

2. **Start Development Servers**
   ```bash
   npm run dev
   ```

   This will start:
   - Backend server on http://localhost:3001
   - Frontend development server on http://localhost:3000

3. **Access the Application**
   - Open your browser to http://localhost:3000
   - Register a new account or login

## Manual Setup (Alternative)

### Backend Setup
```bash
cd backend
npm install
npm run dev
```

### Frontend Setup (in a new terminal)
```bash
cd frontend
npm install
npm run dev
```

## Notes

- The database (SQLite) will be created automatically in `backend/smartcloset.db`
- Uploaded images will be stored in `backend/uploads/` directory
- If you encounter issues with `better-sqlite3`, you may need to install build tools:
  - Windows: Install Visual Studio Build Tools or use `npm install --build-from-source`
  - macOS: Xcode Command Line Tools
  - Linux: `build-essential` package

## Production Build

### Backend
```bash
cd backend
npm run build
npm start
```

### Frontend
```bash
cd frontend
npm run build
# Serve the dist/ folder with your preferred web server
```

