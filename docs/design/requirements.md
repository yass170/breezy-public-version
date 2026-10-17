# Product Requirements

A social networking application for publishing short posts, following people and participating in conversations through a personalized feed.

## Users

| Role | Expected outcome |
|---|---|
| Member | Publish posts, follow accounts, interact with content and exchange messages. |
| Private-account owner | Control follow requests and account visibility. |
| Moderator | Review reports and manage inappropriate activity. |

## Functional scope

| Capability | User outcome |
|---|---|
| Accounts and profiles | Manage sign-in, profile information and public or private account behavior. |
| Posts and conversations | Publish short content, react, comment and reply. |
| Social graph and feed | Follow accounts and browse content associated with the user’s network. |
| Media | Attach and retrieve media through a dedicated component. |
| Messages and notifications | Exchange private messages and follow unread social activity. |
| Moderation | Report content and review moderation cases. |

## Main user journey

1. Create an account and complete a profile.
2. Follow other accounts or submit a request to a private account.
3. Publish a post and participate in feed conversations.
4. Review messages and notifications or report content when necessary.

## Acceptance priorities

- Private-profile and follow-request behavior respect account visibility.
- Post interactions are reflected coherently in feed and notifications.
- Private messages remain limited to the appropriate participants.
- Moderation actions are restricted to the corresponding role.

## Product constraint

Privacy and moderation apply across several services; a visible interface control is not sufficient without the corresponding server-side check.
