# Verification Strategy

## Critical behaviors

- Private-profile and follow-request behavior respect account visibility.
- Post interactions are reflected coherently in feed and notifications.
- Private messages remain limited to the appropriate participants.
- Moderation actions are restricted to the corresponding role.

## Test layers

| Layer | Focus |
|---|---|
| Unit | Domain rules, validation and state changes without live external dependencies. |
| Integration | Consistency across application services and their storage or external-service adapters. |
| User journey | A complete path from a user action to its visible outcome, including failure states. |

## Environment checks

Privacy and moderation apply across several services; a visible interface control is not sufficient without the corresponding server-side check.
