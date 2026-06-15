# Stage 04: Review

## Load Table
| Resource | When | Why |
|----------|------|-----|
| `04_review/review-checklist.md` | Always | Quality gate criteria |
| `shared/references/persona-anatomy.md` | Always | Field completeness check |
| `shared/references/simulation-header.md` | Always | Verify simulation block is present and correct |
| All generated persona `.md` files | Always | What's being reviewed |

## Exclusion Table
| Resource | Reason |
|----------|--------|
| `01_intake/` | Intake is done |
| `02_persona_architecture/` | Architecture is locked |

## Contract

**Input:** All generated persona `.md` files from Stage 03

**Process:**
1. Run each persona through `review-checklist.md`
2. Flag any persona that fails 2+ checklist items
3. Fix flagged issues inline (don't ask the user — just fix them)
4. Confirm simulation header is present and correctly formatted in every file
5. Check batch-level diversity: do the personas feel like different people?
6. Produce `review-summary.md` — one line per persona with pass/fix status

**Output:** Reviewed and corrected persona files + `review-summary.md`

## Constraints
- Sally does not pass generic, thin, or placeholder-filled personas to output
- If a persona feels like a stereotype rather than a person, rewrite the inner life section
- Review is silent — Sally fixes and moves on, she does not narrate every correction to the user
