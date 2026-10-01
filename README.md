# 🧾 BillBuddies

Split bills and track trip expenses with friends — no spreadsheets, no arguments.

## What is this?

BillBuddies is a lightweight web app for splitting bills with friends. It has two modes:

- **Single Bill** — one meal, one quick split. Just enter the amount and who's in.
- **Trip** — track expenses day by day across a multi-day trip, with multiple payers per expense, and get a final settlement showing who owes whom.

## Features

- Split a single bill instantly among selected people
- Multi-day trip tracking with auto-generated days
- Support for multiple people paying for one expense (split cash contributions)
- Shareable trip links — open the same trip from any device
- "Continue last trip" — pick up where you left off, no login required
- One-tap share of the final settlement via WhatsApp/Messenger
- Cloud-synced using Supabase (PostgreSQL + auto-generated API)
- Secured via Postgres RPC functions (no public bulk data access)

## Tech Stack

- **Frontend:** HTML, CSS, vanilla JavaScript (no frameworks)
- **Backend/Database:** [Supabase](https://supabase.com) (PostgreSQL)
- **Hosting:** Vercel

## Live Demo

🔗 https://billbuddies-cyan.vercel.app

## Setup (for running your own copy)

1. Create a free [Supabase](https://supabase.com) project
2. Run the SQL setup script (creates the `bills` table and the `get_bill` / `upsert_bill` RPC functions)
3. Open `index.html`, paste your Supabase Project URL and anon key into the `SUPABASE_URL` / `SUPABASE_ANON_KEY` constants
4. Open `index.html` in a browser — that's it, no build step needed

## Why this project

Built as a hands-on project to learn frontend development, backend/database integration, and deployment — a practical step toward DevOps and cloud engineering.
