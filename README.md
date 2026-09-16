<h1 align="center">Swift Learn</h1>
 
<p align="center">
  <em>SwiftLearn
    An educational website that lets you learn and take quizzes without paid subscription.
</em>
</p>
<p align="center">
  <a href="https://github.com/USER/swift-learn/actions"><img src="https://img.shields.io/github/actions/workflow/status/USER/swift-learn/ci.yml" alt="Build"></a>
  <a href="LICENSE"><img src="https://img.shields.io/github/license/USER/swift-learn" alt="License"></a>
  <a href="https://swift-learn.example.com"><img src="https://img.shields.io/badge/demo-live-brightgreen" alt="Live demo"></a>
</p>
<p align="center">
  <img src="docs/demo.gif" alt="Swift Learn walkthrough" width="700">
</p>
---
 
## What it does
 
Swift Learn lets instructors publish structured courses and lets learners work
through them at their own pace — lessons, quizzes, and progress tracking in one
place, with no setup beyond a browser.
 
*(Replace this paragraph with your actual one-liner. Be concrete: who uses it,
what problem it removes.)*
 
**[Live demo →](https://swift-learn.example.com)** · **[Documentation →](https://docs.swift-learn.example.com)**
 
## Features
 
- SWIFT
- SCOPE
- CLYNX



## Tech stack
 
| Layer | Technology |
|-------|-----------|
| Frontend | React 18 + TypeScript, Vite |
| Styling | Tailwind CSS |
| Backend | Node.js + Express |
| Database | PostgreSQL + Prisma |
| Auth | JWT / OAuth |
 
## Getting started
 
**Requirements:** Node 18+, npm 9+, PostgreSQL 14+
 
```bash
git clone https://github.com/USER/swift-learn.git
cd swift-learn
npm install
cp .env.example .env
npm run db:migrate
npm run dev
```
 
Open http://localhost:5173 — a seeded demo course and test accounts are created
automatically.
 
| Role | Email | Password |
|------|-------|----------|
| Instructor | `teacher@demo.local` | `demo1234` |
| Learner | `student@demo.local` | `demo1234` |
 
## Configuration
 
Copy `.env.example` to `.env` and set:
 
| Variable | Required | Description |
|----------|----------|-------------|
| `DATABASE_URL` | yes | PostgreSQL connection string |
| `JWT_SECRET` | yes | Secret used to sign session tokens |
| `PORT` | no | API port (default `3000`) |
| `UPLOAD_DIR` | no | Where lesson media is stored (default `./uploads`) |
 
## Scripts
 
```bash
npm run dev        # start frontend + API in watch mode
npm run build      # production build
npm run test       # run the test suite
npm run lint       # eslint + type check
npm run db:seed    # reset and reseed demo data
```
 
## Project structure
 
```
swift-learn/
├── client/        # React frontend
│   ├── src/components/
│   ├── src/pages/
│   └── src/hooks/
├── server/        # Express API
│   ├── src/routes/
│   ├── src/services/
│   └── prisma/
└── docs/
```
 
## Roadmap
 
- [x] Course builder and lesson player
- [x] Quizzes with auto-grading
- [ ] Certificates on completion
- [ ] Offline mode
- [ ] Instructor analytics dashboard
See [open issues](https://github.com/USER/swift-learn/issues) for the full list.
 
## Contributing
 
Pull requests are welcome. For larger changes, open an issue first so we can
discuss the approach.
 
1. Fork the repo and create a branch: `git checkout -b feat/my-feature`
2. Make your changes and add tests
3. Run `npm run lint && npm run test`
4. Open a pull request describing what changed and why
## License
 
[MIT](LICENSE) © Your Name
