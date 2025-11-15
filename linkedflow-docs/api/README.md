# API Documentation

Complete API documentation for LinkedFlow AI backend.

## Endpoints

- [Authentication](./AUTH.md) - Login, registration, JWT tokens
- [Posts](./POSTS.md) - Post generation and management
- [Analytics](./ANALYTICS.md) - Analytics and metrics
- [CRM](./CRM.md) - Customer relationship management
- [Planner](./PLANNER.md) - Content planning and scheduling
- [Monitor](./MONITOR.md) - Social media monitoring

## Base URL

```
Development: http://localhost:3001
Production: https://api.linkedflow.ai
```

## Authentication

All protected endpoints require a JWT token in the Authorization header:

```
Authorization: Bearer <token>
```

