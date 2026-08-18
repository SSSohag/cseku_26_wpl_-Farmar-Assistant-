# Smart Farmer Assistance Platform

A crop-lifecycle-centered farmer assistance platform — a mobile app (with a supporting admin web panel) that guides a farmer through the complete journey of a selected crop, from cultivation planning to harvest.

> Unlike a generic agricultural information app, this platform tracks a farmer's actual crop stage-by-stage and tells them **what to do now, what's coming next, what's already been done, what problems have occurred, and how much they've spent.**

## Project Info

| | |
|---|---|
| **Course** | Web Programming & Mobile App Development Project Lab |
| **Program** | 4th Year BSc Honours in CSE |
| **Team Size** | 2 Members |
| **Duration** | ~2.5 Months |
| **Development Approach** | AI-in-the-Loop Engineering (AI-assisted, human-reviewed at every stage) |

## Core Features

- Farmer authentication & profile
- Farm management (location, soil type, land size, irrigation)
- Crop registration with auto-generated cultivation plan
- Crop lifecycle & stage tracking (Land Prep → Planting → Growth → Flowering → Fruiting → Harvest)
- Today's & upcoming activity scheduling
- Notifications & reminders
- Stage-based farming guidance/recommendations
- Weather integration & weather-driven alerts
- Farming diary (activity logs)
- Complete crop history
- Crop problem reporting (text/image) with possible-issue assistance
- Expense tracking & cultivation cost calculation
- Farmer dashboard
- Admin panel (manage crops, stages, activities, knowledge base)

**Optional (post-core):** image-based disease detection, revenue/profit calculation, advanced AI chatbot, analytics, voice assistant, IoT integration.

## Tech Stack

| Layer | Technology |
|---|---|
| Mobile App | Flutter / React Native |
| Admin Web | React.js |
| Backend API | Node.js + Express.js |
| Database | PostgreSQL |
| Auth | JWT |
| Weather | OpenWeatherMap API |
| Notifications | Firebase Cloud Messaging |
| Image Storage | Firebase Storage / Cloudinary |

## Project Structure

```
├── mobile-app/        # Flutter/React Native farmer app
├── admin-web/         # React admin panel
├── backend/           # REST API (Node.js/Express)
├── docs/              # SRS, diagrams, and other documentation
└── README.md
```

## System Architecture

3-tier architecture: **Farmer App + Admin Web** (presentation) → **Backend REST API** (business logic — plan generation, stage advancement, guidance, reminders) → **Database + Weather API** (data).

## Development Approach: AI-in-the-Loop Engineering

AI agents assist across the SDLC, with mandatory human review at each step:

```
Human Requirement → AI Requirement Agent → Human Review
→ Architecture Agent → Human Decision
→ Coding Agent → Human Review
→ Testing Agent → Human Validation
→ Final Integration
```

## Documentation

Full requirement details (functional/non-functional requirements, use cases, database schema, API list, screen list, and timeline) are in [`docs/SRS.docx`](./docs/SRS.docx).

## Timeline

| Week | Focus |
|---|---|
| 1 | Initiation & SRS ✅ |
| 2 | Architecture & DB design, wireframes |
| 3 | Backend core (auth, farm) + mobile skeleton |
| 4 | Crop planning & lifecycle tracking |
| 5 | Activity scheduling |
| 6 | Notifications, guidance, weather |
| 7 | Diary, history, expenses |
| 8 | Crop problem module |
| 9 | Admin panel |
| 10–11 | Dashboard, integration, testing, docs, demo |

## Contribution Guidelines

- Branch naming: `feature/`, `bugfix/`, `docs/`
- Commit format: [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, `docs:`)
- Open a PR with a description + checklist; at least 1 reviewer approval required to merge

## Team

| Role | Member |
|---|---|
| Backend & Admin Panel | [Name] |
| Mobile App & Frontend | [Name] |

## License

MIT
