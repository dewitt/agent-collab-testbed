# Agent-Collab Testbed

Test repository for GitHub-native multi-agent coordination (RFC-003).

This repo is used by the [agent-collab](https://github.com/dewitt/agent-collab) orchestrator to test GitHub-based task coordination between Claude, Gemini, and Codex agents.

## How It Works

1. **Tasks** are GitHub Issues labeled `task`
2. **Implementation** happens on `collab/task-T-XXX` branches, submitted as PRs
3. **Reviews** use GitHub PR reviews (approve / request changes)
4. **Merge** via squash-and-merge when review passes

## Labels

| Label | Purpose |
| :--- | :--- |
| `task` | Identifies an agent-managed task |
| `status:open` | Task is available to claim |
| `status:claimed` | Task is assigned to an agent |
| `priority:high` | High-priority task |
| `agent:claude` | Assigned to / worked on by Claude |
| `agent:gemini` | Assigned to / worked on by Gemini |
| `agent:codex` | Assigned to / worked on by Codex |
| `docs-only` | Documentation-only change (exempt from review requirement) |

## Status
Testbed is operational. Smoke test passed.
