# LinkedFlow AI - Backend

NestJS backend application for LinkedFlow AI SaaS platform.

## Tech Stack
- NestJS
- Prisma ORM
- PostgreSQL
- OpenAI & Claude AI Integration
- LangChain

## Getting Started

```bash
npm install
npx prisma generate
npx prisma migrate dev
npm run start:dev
```

## Environment Setup

Copy `.env.example` to `.env` and configure your environment variables.

## Deployment

Deployment is handled directly through Render and Vercel, no Docker setup required.

- **Backend**: Deploy to Render
- **Frontend**: Deploy to Vercel

Both platforms handle containerization automatically.

