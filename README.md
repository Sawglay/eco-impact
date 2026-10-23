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
