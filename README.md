# 🌱 EcoImpact

**Your actions. Our planet. Real impact.**

EcoImpact is a planned sustainability-focused web application that encourages people to adopt environmentally friendly habits, earn EcoPoints for verified actions, and participate in community challenges and partner-sponsored rewards.

> **Project status:** Planning / pre-development. Features described below are proposed and are not yet implemented.

## Overview

Small everyday actions can make a difference, but people often lack an engaging way to track their progress or participate in local sustainability initiatives. EcoImpact aims to make sustainable habits more accessible, measurable, and rewarding.

The initial product will be a responsive web application (with Progressive Web App capabilities considered) focused on individual users and small community pilots. Future versions may introduce business partnerships and verified social-impact programs.

## Mission

Encourage sustainable daily habits through accessible technology, transparent rewards, and community participation.

## Planned MVP Features

- **User accounts:** Registration, login, and profile management.
- **Eco-action catalog:** Browse activities such as recycling, using reusable bottles, or choosing public transportation.
- **Action submissions:** Record completed activities for review or verification.
- **EcoPoints wallet:** Earn points for approved actions and view a transaction history.
- **Daily challenges:** Participate in simple sustainability challenges.
- **Personal dashboard:** View activity history, points, and progress.
- **Demo rewards:** Explore simulated redemptions during development; no real-world donations are implied.
- **Admin tools:** Manage actions, review submissions, and configure challenges.
- 
### Example User Journey

1. Create an EcoImpact account.
2. Select an available eco-friendly action.
3. Submit evidence or complete a partner-verified activity.
4. Receive EcoPoints after approval.
5. Track progress and explore available challenges or rewards.

**Important:** EcoPoints are not money. Any future real-world reward, tree planting, or food donation will require verified partners, funding, and transparent fulfillment records. Self-reported actions will not automatically qualify for real-world impact claims.

## Proposed Tech Stack

| Layer | Technology |
| --- | --- |
| Frontend | Next.js, React, TypeScript |
| UI styling | Tailwind CSS |
| Backend API | Python, FastAPI |
| Database | PostgreSQL |
| Design | Figma |
| Development environment | Docker, Docker Compose |
| Version control | Git, GitHub |

The stack may change as the prototype evolves.

## High-Level Architecture

```text
Browser / Mobile Web (Next.js)
             |
             | HTTPS / REST
             v
       FastAPI Backend
       |      |      |
    Users  Actions  Rewards
       \      |      /
        PostgreSQL
```

### Proposed Data Models

- `users` — account and profile information
- `eco_actions` — available activities and point rules
- `action_submissions` — activity evidence and verification status
- `point_transactions` — auditable points earned and spent
- `rewards` — available or simulated reward options
- `redemptions` — redemption requests and outcomes

Points should be awarded server-side only after a submission is approved. The transaction history should prevent duplicate awards and support auditing.

## Getting Started

The application has **not yet been scaffolded**, so there are no working installation commands at this stage.

Once development begins, this section will document:

1. Prerequisites and required tool versions.
2. Repository setup and environment variables.
3. Database initialization and migrations.
4. Frontend and backend development commands.
5. Automated tests and local Docker setup.

Never commit secrets or real credentials to the repository. An `.env.example` file will be provided when configuration is implemented.

## Development Roadmap

- [ ] **Phase 1 — Discovery:** Validate target users, use cases, and pilot partners.
- [ ] **Phase 2 — Product design:** Finalize requirements, user flows, and Figma screens.
- [ ] **Phase 3 — Foundation:** Scaffold frontend/backend, database, and authentication.
- [ ] **Phase 4 — Core MVP:** Build actions, submissions, verification, points, and dashboard.
- [ ] **Phase 5 — Rewards:** Add demo redemptions and admin controls.
- [ ] **Phase 6 — Quality:** Add tests, access controls, abuse prevention, and responsive QA.
- [ ] **Phase 7 — Pilot:** Deploy a beta version and gather user feedback.
- [ ] **Phase 8 — Partnerships:** Explore verified rewards and business-sponsored challenges.


## Future Possibilities

These are **not part of the initial MVP**:

- Partner QR-code verification
- Community leaderboards and team challenges
- AI-assisted recycling guidance
- Food rescue and donation coordination
- Verified tree-planting or meal-sponsorship programs
- Business sustainability dashboards and reporting
- Dedicated iOS and Android applications

## Business Direction

EcoImpact may eventually offer sponsored sustainability challenges, local reward partnerships, and subscription-based tools for businesses or organizations. These are hypotheses to validate through pilot programs, not established revenue streams.

## Principles

- **Transparency:** Clearly distinguish estimated, simulated, and verified impact.
- **Trust:** Protect user information and prevent fraudulent point claims.
- **Accessibility:** Keep the experience simple and mobile-friendly.
- **Measurability:** Focus on useful participation and retention metrics.
- **Sustainability:** Avoid promising rewards or donations without funding and fulfillment partners.

## Contributing

The project is currently in its early planning stage. Contribution guidelines and issue templates will be added when the first development repository is ready.

## License

**License not yet selected.** Until a license is added, no open-source reuse permissions are granted by default. A suitable license will be chosen before inviting external contributions.

---

**EcoImpact** — *Your actions. Our planet. Real impact.*
