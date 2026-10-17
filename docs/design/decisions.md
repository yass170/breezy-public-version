# Design Decisions

## 1. Separate services by social-network responsibility

**Benefit.** Identity, posts, relationships and moderation can evolve within clear boundaries.

**Trade-off.** Cross-domain behavior requires explicit communication and integration tests.

## 2. Use events for secondary effects

**Benefit.** Social actions can trigger feed or notification updates without combining every concern in one request.

**Trade-off.** Users and services must account for asynchronous completion.

## 3. Keep media outside service-local filesystems

**Benefit.** Uploaded content survives replacement of an application process.

**Trade-off.** Media access and failure handling require a dedicated storage boundary.
