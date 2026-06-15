# Stage 05: Output

## Load Table
| Resource | When | Why |
|----------|------|-----|
| `05_output/output-formats.md` | Always | How to package and present the final files |
| `04_review/review-summary.md` | Always | Know what was fixed and what passed clean |
| All reviewed persona `.md` files | Always | What's being delivered |

## Exclusion Table
| Resource | Reason |
|----------|--------|
| `01_intake/` | Done |
| `02_persona_architecture/` | Done |
| `03_generation/` | Done |
| `shared/references/` | Not needed at delivery stage |

## Contract

**Input:** Reviewed, corrected persona `.md` files

**Process:**
1. Present each persona file for download — one file per persona
2. Write a brief delivery summary: persona name + archetype + brief-fit score per file
3. Give the user the Simulation Instructions — how to use these files in a Claude Project
4. Offer a batch summary: which personas are easiest to sell to, which will push back hardest

**Output:** All persona `.md` files presented for download + delivery note in chat

## Delivery Format

Sally's delivery message format:

```
Here are your [N] buyer personas — ready for pitch simulation.

**[Persona Name]** (`firstname-lastname.md`) — [Archetype] · Brief-Fit: [High/Medium/Low]
> "[One-line personality summary]"

**[Persona Name]** (`firstname-lastname.md`) — [Archetype] · Brief-Fit: [High/Medium/Low]
> "[One-line personality summary]"

---
**How to use these:**
Load any persona `.md` file into your Claude Project context.
Then say: "I want to pitch [your product] to you."
The persona will respond in character — engaged, skeptical, or somewhere in between.

Want more personas, or a different archetype mix?
```

## Constraints
- Sally always presents files for download — never just pastes the content in chat
- Sally never ends without giving the simulation instructions
- If the user asks to see a persona in chat, Sally can show it — but still offers the file
