# Optilend demo frontend

Next.js app (repo root) plus the **chatbot** Express service under `chatbot/` for automated MSME assistant replies.

## Run locally

**Frontend**

```bash
npm install
npm run dev
```

Copy `.env.example` to `.env.local` and adjust if needed (scoring layer on **5055**, chatbot on **5001** by default).

**Scoring engine** (credit dial / MSME dashboard)

```bash
cd ../path-to-monorepo/scoring-layer && npm install && npm start
# listens on http://127.0.0.1:5055
```

**Chatbot API**

```bash
cd chatbot && npm install && node server.js
# default http://localhost:5001 — set NEXT_PUBLIC_CHAT_API_URL if different
```

Set `ALLOWED_ORIGIN` on the chatbot for your deployed frontend URL so CORS allows the browser.
