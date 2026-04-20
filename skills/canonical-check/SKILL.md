# Skill: Canonical Check

Purpose: Validate one or more canon markdown documents for structural hygiene.

## Required inputs
- one or more canon documents (Markdown)
- optional repository file index for resolving references

## Checks
1. Required fields are present: keys: `decision_code`, `status`, `version`, `current_answer`, `rationale`.
22. References to other canon items resolve to existing paths or decision codes in the canon directory.
3. Internal consistency: code, status, version, and body should not contradict each other.
4. Status-appropriate completeness: `Locked` must have a rationale; `Draft` may be incomplete.

## Output format
Return Markdown with:
- Summary: items checked, items with issues
- Per-file results
- For each issue: issue type, severity (`info`, `warning`, `error`), evidence, recommended manual fix
- A list of resolved references used in the check

## Rules
- Do not auto-edit files.
- Do not invent canon items that are missing; flag them as unresolved references.
- If a file is not in markdown, return a warning and skip deeper content checks.
