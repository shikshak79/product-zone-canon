# Hurozo Demo Notes

- Agent 1: Canonical Hygiene watches `canon/` and runs `daily` sweeps.
- Agent 2: Skill Execution reads `skills/` in real time and loads canon context before running.
- Agent 3: Signal Ingest watches `inbox/` and writes proposals to `hurozo/proposals/`.
- Founder: can edit canon and accept/reject proposals.
- Reader: can view canon and outputs, but should not be given repo write permissions.
