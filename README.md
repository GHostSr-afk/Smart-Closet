# SmartCloset

A minimalist wardrobe management web application with AI-powered outfit suggestions.

## Features

- **User Authentication**: Secure login and registration system
- **Clothing Upload**: Upload photos and tag items with category, season, and last worn date
- **View Closet**: Browse your wardrobe with search and category filters
- **Outfit Planner**: Get AI-powered outfit suggestions based on your closet

## Tech Stack

- **Frontend**: React + TypeScript + Vite
- **Backend**: Node.js + Express + TypeScript
- **Database**: SQLite
- **Authentication**: JWT

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Install all dependencies:
```bash
npm run install:all
```

2. Start the development servers (both backend and frontend):
```bash
npm run dev
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend API: http://localhost:3001

### Manual Setup

If you prefer to run backend and frontend separately:

**Backend:**
```bash
cd backend
npm install
npm run dev
```

**Frontend:**
```bash
cd frontend
npm install
npm run dev
```

## Project Structure

```
smartcloset/
├── backend/
│   ├── src/
│   │   ├── database/    # Database setup and schema
│   │   ├── middleware/  # Authentication middleware
│   │   ├── routes/      # API routes
│   │   └── index.ts     # Server entry point
│   └── uploads/         # Uploaded images (created automatically)
├── frontend/
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── pages/       # Page components
│   │   ├── utils/       # API utilities
│   │   └── types.ts     # TypeScript types
│   └── public/
└── package.json         # Root package.json for convenience scripts
```

## API Endpoints

- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `GET /api/clothes` - Get all clothes (authenticated)
- `POST /api/clothes` - Upload new clothing item (authenticated)
- `POST /api/outfit/suggest` - Get outfit suggestion (authenticated)
- `POST /api/outfit/save` - Save outfit (authenticated)

## Design

The app features a "Quiet Luxury" aesthetic with:
- Neutral color palette (White, Beige, Soft Grey)
- Rounded corners and clean typography
- Minimalist interface
- Mobile-responsive design

## License

MIT

