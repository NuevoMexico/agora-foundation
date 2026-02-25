# Architecture Principles (Agora)

## Security-first
- No production secrets on my Mac.
- No production data in dev environments.

## Execution boundary
- All agent execution happens inside an isolated VM (client-like runtime).
- Snapshot before installing or changing system dependencies.

## Network discipline
- Prefer deny-by-default egress for agent runtimes (enable only what is required).

## Auditability
- Every tool call and external interaction must be logged and attributable.
