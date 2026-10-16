# Eymir — MUST Campus Connections

An independent, mobile-first student social app for Meru University. **Early development MVP, not production-ready.**

## Features implemented
- 18+ registration and password login with HttpOnly signed session cookies
- Plans and RSVPs
- Student discovery and mutual likes
- Match-gated message submission (history UI pending)
- Blocking and reporting submissions

## Local setup
1. `npm install`
2. Create a Neon PostgreSQL database and run `db/schema.sql` in its SQL editor.
3. Copy `.env.example` to `.env.local` and set `DATABASE_URL` and a random `SESSION_SECRET` of at least 32 characters.
4. `npm run dev` and open http://localhost:3000.

## Required before real student launch
**Do not invite real students yet.** Email ownership / campus verification is absent; account recovery, login throttling, CSRF/origin review, moderation dashboard, user consent and deletion workflows, message inbox/history, event moderation, and privacy/legal review remain outstanding. Age is self-declared only. Plan dates and attendance are beta-only. No institutional endorsement is implied.

## Deploy
Import this repository into Vercel, set environment variables, configure Neon and run the SQL migration first. Test with dummy data before opening registration.
