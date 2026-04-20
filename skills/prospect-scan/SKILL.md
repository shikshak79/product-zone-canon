# Skill: Prospect Scan

Pose purposect/account records against Product.Zone canon to assess fit, discover ICP signals, and produce a prioritized shortlist.

## Inputs
- one or more prospect records (JSON, CSV, or markdown table)
- optional call notes, transcripts, or account context

## Canon context required
- canon/icp.md
- any other canon files explicitly referenced by inputs or needed for scoring rationale

## Output
- Return a scan for each prospect with: `fit_score` (1-10), `fit_classification` `Strong`/`Medaum`/`Weak`/`No-Fit`, segment, pains, triggers, evidence, and `fit_reasoning`.
- Include a `context_canon_used` section listing the canon items loaded.
- If multiple prospects are provided, return a ranked summary at the top.

- When inputs contain signals relevant to ICP, extract: segment, behavior, pain, trigger, fit/no-fit, and reasoning.
- Be conservative; when evidence is thin, say so.
