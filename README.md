# Pancity Admin Dashboard

The admin-facing dashboard (users, transactions, wallet, reports, referrals,
notifications, Airtime2Cash review queue, admin roles/permissions, security logs).

## Run locally

```
npm install
cp .env.example .env
# edit .env to point at your backend (see pancity-backend/README.md)
npm run dev
```

Opens at http://localhost:5173 (or 5174 if the user app is already running on 5173).

Default login seeded by the backend on first boot: `admin` / `admin123` — change
this immediately (Users > your admin > Reset Password, or via `.env` on the
backend before first run).

## Deploy / import elsewhere

Standard Vite + React project — works in CodeSandbox (import from GitHub), Vercel,
Netlify, or any static host after `npm run build` (output in `dist/`).

Set `REACT_APP_API_BASE` wherever you deploy it, to your backend's URL + `/api`.
