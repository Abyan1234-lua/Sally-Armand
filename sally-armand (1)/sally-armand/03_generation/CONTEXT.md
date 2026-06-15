# Stage 03: Generation

## Load Table
| Resource | When | Why |
|----------|------|-----|
| `02_persona_architecture/architecture-plan.md` | Always | Blueprint for each persona |
| `shared/references/persona-anatomy.md` | Always | Field structure and writing rules |
| `shared/references/simulation-header.md` | Always | Simulation activation block for each file |
| `shared/references/psychology-frameworks.md` | Always | Motivational depth |
| `shared/templates/persona-template.md` | Always | Base markdown template |
| `shared/examples/` | As needed | Reference quality bar |

## Exclusion Table
| Resource | Reason |
|----------|--------|
| `01_intake/` | Already processed — don't re-read |
| `04_review/` | Not yet — generate first |

## Contract

**Input:** `architecture-plan.md` — all persona slots with dimensions assigned

**Process:**
For each persona slot:
1. Load the persona's archetype, demographics, and brief-fit score
2. Write the full persona using `persona-template.md` structure
3. Fill every section with specific, believable, non-generic detail
4. Write the `## Simulation Header` block — instructions for Claude when this file is loaded
5. Name the file: `firstname-lastname.md` (lowercase, hyphenated)
6. Save each persona as a separate `.md` file

**Output:** N separate `.md` files in `05_output/personas/` — one per persona

## Generation Rules

### Specificity Rule
Every field must contain a specific detail, not a category.
- BAD: "She likes productivity apps"
- GOOD: "She's been using Notion since 2021 but recently switched her task list back to a paper journal because she felt Notion was 'too much friction for daily use'"

### Contradiction Rule
Real people contradict themselves. Every persona must have at least one internal tension:
- Wants to save money but also hates feeling cheap
- Says they research everything but admits they bought their last phone on impulse
- Claims to value sustainability but hasn't changed a buying habit in 3 years

### Objection Authenticity Rule
Objections must be specific and rooted in the persona's life — not generic:
- BAD: "Price is too high"
- GOOD: "She's been burned before paying for tools her team didn't adopt. She won't pitch another tool to her boss unless she's 100% sure people will use it."

### Simulation Header Rule
Every persona file must open with a Simulation Header block.
This block tells Claude how to *be* this person when the file is loaded in a Project.
Use `shared/references/simulation-header.md` as the template.
