# Directory Structure

```text
breezy-public-version/
├── .github/
│   └── workflows/
├── apps/
│   ├── auth-service/
│   │   ├── module-004/
│   │   │   └── migrations/
│   │   │       ├── module-001/
│   │   │       └── module-002/
│   │   ├── scripts/
│   │   ├── src/
│   │   │   ├── config/
│   │   │   ├── db/
│   │   │   ├── health/
│   │   │   ├── module-005/
│   │   │   ├── module-008/
│   │   │   ├── modules/
│   │   │   │   └── auth/
│   │   │   ├── types/
│   │   │   └── utils/
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
│   │   │   ├── config/
│   │   │   ├── events/
│   │   │   ├── health/
│   │   │   ├── module-005/
│   │   │   ├── modules/
│   │   │   │   └── module-001/
│   │   │   ├── types/
│   │   │   └── utils/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── frontend/
│   │   ├── e2e/
│   │   │   └── support/
│   │   ├── messages/
│   │   ├── public/
│   │   │   └── branding/
│   │   │       └── module-001/
│   │   │           └── README.md
│   │   ├── src/
│   │   │   ├── app/
│   │   │   │   └── [locale]/
│   │   │   │       ├── admin/
│   │   │   │       │   └── module-001/
│   │   │   │       ├── messages/
│   │   │   │       ├── module-003/
│   │   │   │       ├── module-005/
│   │   │   │       │   └── module-002/
│   │   │   │       │       └── module-001/
│   │   │   │       ├── module-007/
│   │   │   │       ├── module-009/
│   │   │   │       │   └── module-001/
│   │   │   │       ├── module-010/
│   │   │   │       │   └── module-001/
│   │   │   │       ├── module-011/
│   │   │   │       ├── module-013/
│   │   │   │       │   └── module-001/
│   │   │   │       ├── notifications/
│   │   │   │       └── search/
│   │   │   ├── components/
│   │   │   │   ├── module-011/
│   │   │   │   ├── module-022/
│   │   │   │   └── ui/
│   │   │   ├── context/
│   │   │   ├── hooks/
│   │   │   ├── i18n/
│   │   │   └── lib/
│   │   ├── tests/
│   │   └── package.json
│   ├── media-service/
│   │   ├── src/
│   │   │   ├── config/
│   │   │   ├── health/
│   │   │   ├── module-004/
│   │   │   ├── modules/
│   │   │   │   └── module-001/
│   │   │   ├── types/
│   │   │   └── utils/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── moderation-service/
│   │   ├── module-004/
│   │   │   └── migrations/
│   │   │       ├── module-001/
│   │   │       └── module-002/
│   │   ├── src/
│   │   │   ├── config/
│   │   │   ├── db/
│   │   │   ├── events/
│   │   │   ├── health/
│   │   │   ├── module-006/
│   │   │   ├── modules/
│   │   │   │   ├── module-001/
│   │   │   │   └── module-002/
│   │   │   ├── types/
│   │   │   └── utils/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── notification-service/
│   │   ├── module-004/
│   │   │   └── migrations/
│   │   │       ├── module-001/
│   │   │       ├── module-002/
│   │   │       └── module-003/
│   │   ├── src/
│   │   │   ├── config/
│   │   │   ├── db/
│   │   │   ├── events/
│   │   │   ├── health/
│   │   │   ├── module-006/
│   │   │   ├── modules/
│   │   │   │   └── notifications/
│   │   │   ├── types/
│   │   │   └── utils/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── post-service/
│   │   ├── src/
│   │   │   ├── config/
│   │   │   ├── db/
│   │   │   ├── events/
│   │   │   ├── health/
│   │   │   ├── module-006/
│   │   │   ├── modules/
│   │   │   │   ├── module-001/
│   │   │   │   └── module-002/
│   │   │   ├── types/
│   │   │   └── utils/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── social-service/
│   │   ├── module-004/
│   │   │   └── migrations/
│   │   │       ├── module-001/
│   │   │       └── module-002/
│   │   ├── src/
│   │   │   ├── config/
│   │   │   ├── db/
│   │   │   ├── events/
│   │   │   ├── health/
│   │   │   ├── module-006/
│   │   │   ├── modules/
│   │   │   │   └── module-001/
│   │   │   ├── types/
│   │   │   └── utils/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   └── user-service/
│       ├── module-004/
│       │   └── migrations/
│       │       ├── module-001/
│       │       ├── module-002/
│       │       ├── module-003/
│       │       └── module-004/
│       ├── src/
│       │   ├── config/
│       │   ├── db/
│       │   ├── health/
│       │   ├── module-005/
│       │   ├── modules/
│       │   │   ├── messages/
│       │   │   └── users/
│       │   ├── types/
│       │   └── utils/
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
