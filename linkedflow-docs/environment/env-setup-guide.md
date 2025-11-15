# Environment Setup Guide

## Prerequisites

- Node.js 18+ 
- PostgreSQL 14+
- npm or yarn

## Frontend Setup

1. Navigate to `linkedflow-frontend`
2. Copy `.env.example` to `.env.local`
3. Install dependencies: `npm install`
4. Run development server: `npm run dev`

## Backend Setup

1. Navigate to `linkedflow-backend`
2. Copy `.env.example` to `.env`
3. Configure database connection in `.env`
4. Install dependencies: `npm install`
5. Generate Prisma client: `npx prisma generate`
6. Run migrations: `npx prisma migrate dev`
7. Start development server: `npm run start:dev`

## Required Environment Variables

### Frontend (.env.local)
- `NEXT_PUBLIC_API_URL` - Backend API URL
- `NEXT_PUBLIC_APP_URL` - Frontend URL

### Backend (.env)
- `DATABASE_URL` - PostgreSQL connection string
- `JWT_SECRET` - JWT signing secret
- `OPENAI_API_KEY` - OpenAI API key
- `ANTHROPIC_API_KEY` - Anthropic (Claude) API key
- `PORT` - Server port (default: 3001)

## Database Setup

1. Create PostgreSQL database: `createdb linkedflow`
2. Update `DATABASE_URL` in backend `.env`
3. Run Prisma migrations: `npx prisma migrate dev`

