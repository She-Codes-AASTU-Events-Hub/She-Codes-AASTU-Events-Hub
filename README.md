# AASTU Event Hub — Frontend

## Run locally

1. Start the **backend** first (`cd ../Backend && npm run dev`).
2. Copy env: `cp .env.example .env.local` (already created if missing).
3. Start frontend:

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

API calls are proxied through Next.js (`/api/v1/*` → backend) so auth cookies work on signup/login.

## Admin login

| Email | Password |
|-------|----------|
| `admin@aastu.edu` | `Admin@1234` |

Use **Admin** button on Explore / Organize / Sign up, or go to `/auth/admin`.

Admin dashboard: `/admin` — approve organizer applications and promotion requests by submission date.

Seed admin (in Backend): `npm run seed`
