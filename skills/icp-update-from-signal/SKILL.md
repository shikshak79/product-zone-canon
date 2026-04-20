# Skill: ICP Update From Signal

Analyze a batch of signal artifacts and propose a specific update to the ICP canon item.

## Inputs
- Batch of artifacts from `inbox/`
- Current `canon/icp.md`

## Extract
- segment
- behavior
- pain
- trigger
- fit/no-fit reasoning
- evidence references back to artifact files and quotes

## Output
Return a structured `Proposed Canon Update` with:
- canon_item: ICP
- specific_delta: what the current canon says vs what new evidence suggests
- evidence_base: artifact references
- rationale
- suggested_rewrite

## Rules
- The update is a proposal, not an auto-edit.
- Be specific and cite evidence.