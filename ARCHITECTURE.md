# Breezy — Social Networking Platform — Architecture

Users can build a profile, share posts, react and reply, follow other accounts and keep up with their network. The project explores domain-oriented backend services alongside a responsive web interface, including privacy, messaging and moderation concerns.

## Components

| Component | Responsibility |
|---|---|
| Web interface | Next.js, React and TypeScript screens for feed, profiles and interactions. |
| Domain services | Node.js/Express services for identity, users, posts, relationships, feed and notifications. |
| Media and moderation services | Dedicated responsibilities for uploaded media and report handling. |
| Domain persistence | PostgreSQL and MongoDB used by the corresponding application domains. |
| Event infrastructure | Shared contracts and RabbitMQ-backed communication for asynchronous effects. |
| Object storage | MinIO-backed media storage independent of service processes. |

## Main interactions

```mermaid
flowchart TD
    N0["Member"]
    N1["Web interface"]
    N2["Domain services"]
    N3["Domain-owned persistence"]
    N4["Application events"]
    N5["Feed and notifications"]
    N6["Media storage"]
    N7["Moderator"]
    N8["Moderation interface"]
    N0 --> N1
    N1 --> N2
    N2 --> N3
    N2 --> N4
    N4 --> N5
    N2 --> N6
    N7 --> N8
```

## Responsibility boundaries

- Separate services by social-network responsibility. Identity, posts, relationships and moderation can evolve within clear boundaries.
- Use events for secondary effects. Social actions can trigger feed or notification updates without combining every concern in one request.
- Keep media outside service-local filesystems. Uploaded content survives replacement of an application process.

## Constraints

Privacy and moderation apply across several services; a visible interface control is not sufficient without the corresponding server-side check.

## Technology

Next.js, React, TypeScript, Node.js, Express, PostgreSQL, MongoDB, RabbitMQ, MinIO, Docker, Jest and Playwright.
