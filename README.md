# Impactpure admin

Vite + React admin panel for the Impactpure store (products and orders). Talks to the Impactpure API.

## Deployment
- Production: Vercel project "impactpure-admin", branch main, root ./, Node 22.x, Vite preset (build: vite build, output: dist).
- Staging: Vercel project "impactpure-admin-staging", branch staging.
- Every push to main is a production deploy.

## Local development
Copy .env.example to .env and point VITE_BACKEND_URL at a staging API, never production, when testing writes.
    npm install
    npm run dev

## Environment variables (names only)
App: admin. Environments: Production and Staging only.

| Variable | Visibility | Environments | Service |
|---|---|---|---|
| VITE_BACKEND_URL | public (build time) | Production, Staging | Impactpure API |
