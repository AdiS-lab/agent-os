# Verification Rules

## Principle

The implementation is not the result.

The verified behavior is the result.

---

## Verification Hierarchy

Use the strongest applicable verification.

### Level 1 — Static

- type checking
- linting
- build

### Level 2 — Automated

- unit tests
- integration tests
- API tests

### Level 3 — Runtime

- start the application
- inspect logs
- exercise the feature

### Level 4 — End-to-End

Perform the actual user flow.

Example:

User action
→ application state
→ network/API interaction
→ external service
→ response
→ UI result

---

## External Integrations

For integrations with external services, successful initialization is NOT sufficient.

Verify the actual interaction.

For example:

Bad verification:

> "The ElevenLabs client initialized successfully."

Good verification:

> "Started the application, initiated a conversation, granted microphone access, spoke to the agent, confirmed agent audio, then terminated the session."

---

## Failure Handling

When verification fails:

Do not report success.

Record:

- observed failure
- likely cause
- attempted correction
- result after correction

Continue until the acceptance criterion passes or clearly document why it cannot be verified.