# Deployment Guide

## Production Deployment

Deployment is handled directly through Render and Vercel, no Docker setup required. Both platforms handle containerization automatically.

### Frontend Deployment (Vercel)

1. Connect GitHub repository to Vercel
2. Configure environment variables in Vercel dashboard:
   - `NEXT_PUBLIC_API_URL` - Backend API URL
   - `NEXT_PUBLIC_APP_URL` - Frontend URL
3. Deploy automatically on push to main branch
4. Vercel will automatically build and deploy your Next.js application

### Backend Deployment (Render)

1. Connect GitHub repository to Render
2. Create a new Web Service
3. Configure build settings:
   - **Build Command**: `npm install && npx prisma generate && npm run build`
   - **Start Command**: `npm run start:prod`
4. Configure environment variables in Render dashboard:
   - `DATABASE_URL` - PostgreSQL connection string
   - `JWT_SECRET` - JWT signing secret
   - `OPENAI_API_KEY` - OpenAI API key
   - `ANTHROPIC_API_KEY` - Anthropic (Claude) API key
   - `PORT` - Server port (Render will set this automatically)
   - `FRONTEND_URL` - Frontend URL for CORS
   - `NODE_ENV` - Set to `production`
5. Render will automatically build and deploy your NestJS application

### Database Deployment

- Use Render PostgreSQL service or any managed PostgreSQL service
- Update `DATABASE_URL` in production environment
- Run migrations: `npx prisma migrate deploy` (can be done via Render shell or CI/CD)

## Environment Variables

Ensure all production environment variables are set:
- Database connection string
- JWT secret (use strong random string)
- API keys for OpenAI and Anthropic
- Frontend URL for CORS configuration

## Monitoring

- Set up error tracking (Sentry, etc.)
- Configure logging (Winston, Pino)
- Set up health check endpoints
- Monitor API rate limits

