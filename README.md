# Watch Store Project

This repository contains a full-stack "watch" e-commerce application built with:

- **Frontend**: React + Vite (in `/frontend`)
- **Admin panel**: React + Vite (in `/admin`)
- **Backend**: Node.js + Express with MongoDB (in `/backend`)

Each subfolder is its own package with its own `package.json` and development
scripts. You can run them independently during development.

---

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/watch-store.git
   cd watch-store
   ```

2. **Create environment file**
   Copy the example and fill in your values:
   ```bash
   cp .env.example backend/.env
   # edit backend/.env and provide your Mongo URI, Stripe key, JWT secret, etc.
   ```

3. **Install dependencies**
   ```bash
   cd backend && npm install && cd ../frontend && npm install && cd ../admin && npm install
   ```

4. **Run the services**
   - Start the backend server:
     ```bash
     cd backend && npm run dev
     ```
   - Start the frontend app:
     ```bash
     cd frontend && npm run dev
     ```
   - Start the admin panel:
     ```bash
     cd admin && npm run dev
     ```

5. **Build for production**
   Run `npm run build` in each of the three subfolders (`backend`, `frontend`, and
   `admin`). Output will appear in `dist/` directories which are ignored by git.

---

## GitHub Ready Checklist ✅

The following items have been added to make the repository ready for GitHub:

- A root-level `.gitignore` that excludes `node_modules/`, environment files
  (`.env`), local MongoDB data, build artifacts, and common OS/editor files.
- A `.env.example` showing required environment variables without secrets.
- A `LICENSE` (MIT) for open source distribution.
- A top-level `README.md` with overview and setup instructions.

Feel free to adapt the text above before pushing to your GitHub remote.

---

## Subproject READMEs

Both `/frontend` and `/admin` currently contain the default Vite template
README; they can be updated as needed to document their individual features.

---

Enjoy working on the watch store! 🕒
