# Context Rules

## Principle

More context is not necessarily better.

Load the minimum information required to make the current decision correctly.

---

## Priority

Use context in this order:

1. Current task
2. Relevant source files
3. Relevant project architecture
4. Relevant decisions
5. Relevant documentation
6. Historical context

Do not load unrelated project history.

---

## Source Selection

Before reading large files or directories:

1. identify likely relevant files
2. inspect targeted sections
3. expand context only when necessary

Avoid dumping entire repositories into context.

---

## Tool Output

Prefer concise, relevant output.

When command output is large:

- identify the relevant error
- inspect surrounding context
- avoid repeatedly injecting irrelevant output

---

## Historical Context

Historical decisions are useful only when they affect the current implementation.

Do not treat old decisions as immutable requirements.

Current task requirements take precedence.