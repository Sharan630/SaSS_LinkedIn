# System Architecture

## Overview

LinkedFlow AI follows a microservices-oriented architecture with clear separation between frontend, backend, and AI services.

## Architecture Diagram

```
┌─────────────────┐
│   Next.js 14    │
│   Frontend      │
└────────┬────────┘
         │
         │ HTTP/REST
         │
┌────────▼────────┐
│   NestJS API    │
│   Backend       │
└────────┬────────┘
         │
    ┌────┴────┐
    │         │
┌───▼───┐ ┌──▼────┐
│Prisma │ │  AI   │
│  ORM  │ │Engine │
└───┬───┘ └───┬───┘
    │         │
┌───▼─────────▼───┐
│   PostgreSQL    │
│   Database      │
└─────────────────┘
```

## Components

- **Frontend**: Next.js 14 with App Router
- **Backend**: NestJS REST API
- **Database**: PostgreSQL with Prisma ORM
- **AI Engine**: OpenAI + Claude integration with LangChain

