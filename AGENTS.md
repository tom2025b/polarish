## About

Polarish is an open-source SDK for building AI workflows where users bring their own AI subscriptions.

- It has two parts that work in tandem:
- `@polarish/ai` — an AI SDK that helps you build AI workflows.
- `@polarish/cli` — the CLI that helps users connect their AI subscriptions and bridges those complex workflows.

## Rules

- Always run the typecheck and lint commands on every file that you edit.
- Always add JSDoc comments to any new function, type, or schema that you create. Keep the language simple, like "this function does this" and "this is the shape of the request that we are expecting".
- Always use bun, not npm or pnpm.
- When planning to edit or change a file, first read that file so you actually know its current state and can plan better, instead of assuming things.

## Core Priorities

1. Performance first.
2. Reliability first.
3. Keep behavior predictable under load and during failures (session restarts, reconnects, partial streams).

If a tradeoff is required, choose correctness and robustness over short-term convenience.

## Maintainability

Long-term maintainability is a core priority. If you add new functionality, first check if there is shared logic that can be extracted to a separate module. Duplicate logic across multiple files is a code smell and should be avoided. Don't be afraid to change existing code. Don't take shortcuts by just adding local logic to solve a problem.
