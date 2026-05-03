# Optilend demo frontend

Next.js app (repo root) plus **`chatbot/`** for the MSME assistant API.

## Run locally

```bash
npm install && npm run dev
```

Copy **`.env.example`** → **`.env.local`** (scoring **5055**, chat **5001** by default).

**Scoring layer** (credit dial): run the monorepo `scoring-layer` on `http://127.0.0.1:5055`.

**Chatbot:** `cd chatbot && npm install && node server.js`

Loan recommendations live under **`lib/loan-recommendation/`** (no separate package).
