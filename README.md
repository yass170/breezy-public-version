# Breezy — Social Networking Platform

A social networking application for publishing short posts, following people and participating in conversations through a personalized feed.

Users can build a profile, share posts, react and reply, follow other accounts and keep up with their network. The project explores domain-oriented backend services alongside a responsive web interface, including privacy, messaging and moderation concerns.

## Users

| Role | Use |
|---|---|
| Member | Publish posts, follow accounts, interact with content and exchange messages. |
| Private-account owner | Control follow requests and account visibility. |
| Moderator | Review reports and manage inappropriate activity. |

## Main features

- **Accounts and profiles.** Manage sign-in, profile information and public or private account behavior.
- **Posts and conversations.** Publish short content, react, comment and reply.
- **Social graph and feed.** Follow accounts and browse content associated with the user’s network.
- **Media.** Attach and retrieve media through a dedicated component.
- **Messages and notifications.** Exchange private messages and follow unread social activity.
- **Moderation.** Report content and review moderation cases.

## Typical workflow

1. Create an account and complete a profile.
2. Follow other accounts or submit a request to a private account.
3. Publish a post and participate in feed conversations.
4. Review messages and notifications or report content when necessary.

## Project structure

```text
breezy-public-version/
├── .github/
│   └── workflows/
├── apps/
│   ├── auth-service/
│   │   ├── module-004/
│   │   ├── scripts/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── demo-seed/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── feed-service/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── frontend/
│   │   ├── e2e/
│   │   ├── messages/
│   │   ├── public/
│   │   ├── src/
│   │   │   ├── app/
│   │   │   └── components/
│   │   ├── tests/
│   │   └── package.json
│   ├── media-service/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── moderation-service/
│   │   ├── module-004/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── notification-service/
│   │   ├── module-004/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── post-service/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── social-service/
│   │   ├── module-004/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   └── user-service/
│       ├── module-004/
│       ├── src/
│       ├── tests/
│       ├── package.json
│       └── README.md
├── docs/
│   ├── decisions/
│   ├── design/
│   │   ├── decisions.md
│   │   ├── requirements.md
│   │   └── verification.md
│   └── module-010/
├── infra/
│   ├── docker/
│   ├── module-003/
│   │   └── module-001/
│   └── nginx/
│       ├── module-001/
│       └── README.md
├── packages/
│   ├── event-bus/
│   │   ├── src/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   └── event-contracts/
│       ├── src/
│       ├── tests/
│       ├── package.json
│       └── README.md
├── postman/
│   └── module-001/
├── scripts/
├── ARCHITECTURE.md
├── package.json
└── README.md
```

[Complete directory structure](docs/design/structure.md)

| Area | Responsibility |
|---|---|
| Web interface | Next.js, React and TypeScript screens for feed, profiles and interactions. |
| Domain services | Node.js/Express services for identity, users, posts, relationships, feed and notifications. |
| Media and moderation services | Dedicated responsibilities for uploaded media and report handling. |
| Domain persistence | PostgreSQL and MongoDB used by the corresponding application domains. |
| Event infrastructure | Shared contracts and RabbitMQ-backed communication for asynchronous effects. |
| Object storage | MinIO-backed media storage independent of service processes. |

## Technology

Next.js, React, TypeScript, Node.js, Express, PostgreSQL, MongoDB, RabbitMQ, MinIO, Docker, Jest and Playwright.

## Engineering

- [Architecture](ARCHITECTURE.md)
- [Product requirements](docs/design/requirements.md)
- [Design decisions](docs/design/decisions.md)
- [Verification strategy](docs/design/verification.md)

Privacy and moderation apply across several services; a visible interface control is not sufficient without the corresponding server-side check.

---

Source code, operational configuration and project-specific data are withheld for confidentiality.
