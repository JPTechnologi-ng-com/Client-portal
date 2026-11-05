# Client Portal

React 18 + Express + PostgreSQL client portal (admin and client roles, projects, invoices, documents, reports, OpenAI).

## Run locally

Requires Node 20+ and Docker.

```bash
npm install
cp apps/api/.env.example apps/api/.env
npm run db:up
npm run dev
```

- Web: http://localhost:5173
- API health check: http://localhost:4000/api/health

## Structure

- `apps/api` Express server (TypeScript)
- `apps/web` React 18 app (Vite)
- `packages/shared` code shared by both

## Build phases

0 Setup (done) · 1 Database · 2 Auth and roles · 3 Admin API · 4 Documents · 5 Dashboard and reports · 6 OpenAI · 7 CI and deploy
