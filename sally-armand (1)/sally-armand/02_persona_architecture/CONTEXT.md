# Stage 02: Persona Architecture

## Load Table
| Resource | When | Why |
|----------|------|-----|
| `01_intake/intake-output.md` | Always | Validated brief from previous stage |
| `shared/references/psychology-frameworks.md` | Always | Motivational depth — Jobs-to-be-Done, BJ Fogg, etc. |
| `shared/references/persona-anatomy.md` | Always | Field structure for each persona |
| `02_persona_architecture/archetype-matrix.md` | Always | Archetype distribution rules |
| `shared/glossary.md` | Always | Terminology |

## Exclusion Table
| Resource | Reason |
|----------|--------|
| `03_generation/` | Not yet — architecture must be locked before writing |
| `05_output/` | Too early |
| `shared/examples/` | Avoid anchoring — design archetypes before referencing examples |

## Contract

**Input:** `intake-output.md` — mode, brief, count, constraints

**Process:**
1. Design N persona slots — each slot gets a codename and archetype label
2. Assign demographics: name, age, gender, location, job, income tier
3. Assign psychographic axis: motivation type + decision style + tech relationship
4. Assign brief-fit score: how well this persona matches the product (High / Medium / Low)
   — this determines how the pitch simulation will behave
5. Produce `architecture-plan.md` — the persona blueprint passed to Stage 03

**Output:** `02_persona_architecture/architecture-plan.md` — one row per persona with all dimensions assigned

## Constraints
- No two personas in a batch can share the same archetype type
- Brief-fit score must vary across the batch (not all High)
- Demographics must feel geographically and culturally authentic
- Sally must assign a persona full name — real-sounding, culturally appropriate to geography
