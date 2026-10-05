# Outreach Agent (backend + frontend)

## 1. Backend  (`backend/`)
1. `npm install`
2. `cp .env.example .env` and set at least:
   `MONGODB_URI`, `JWT_SECRET`, `ENCRYPTION_KEY` (new, keep it stable), `ADMIN_EMAIL`, `ADMIN_PASSWORD`, `OLLAMA_URL`, `OLLAMA_MODEL`
3. `ollama pull qwen2.5:7b`
4. `npm run dev`  -> http://localhost:4000

## 2. Frontend  (`frontend/`)
1. `npm install`
2. `npm run dev`  -> http://localhost:5173  (proxies /api to the backend)

## First use
1. Log in with ADMIN_EMAIL / ADMIN_PASSWORD.
2. Settings: save your email + app password once, press "Test connection".
3. Templates: write your base email. Leads: upload a CSV, tick leads, "Draft emails".
4. Review & send: check each draft, edit, "Approve & send" one by one.
5. New people use "Request access"; approve them in the Users page.
