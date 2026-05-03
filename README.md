# Optilend demo frontend

Next.js app (root) plus the **chatbot** Express service for automated MSME assistant replies.

## Run locally

**Frontend**

```bash
npm install
npm run dev
```

**Chatbot API** (optional; set `NEXT_PUBLIC_CHAT_API_URL` if not using default `http://localhost:5000`)

```bash
cd chatbot && npm install && node server.js
```

Set `ALLOWED_ORIGIN` for your dev or deployed frontend URL so CORS allows the browser. Use `NEXT_PUBLIC_CHAT_API_URL` on the Next app to point at the chatbot URL.
