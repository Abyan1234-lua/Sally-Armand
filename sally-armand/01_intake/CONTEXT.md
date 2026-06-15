# Stage 01: Intake

## Load Table
| Resource | When | Why |
|----------|------|-----|
| `shared/glossary.md` | Always | Terminology |
| `01_intake/intake-schema.md` | Always | What to collect from the user |
| `01_intake/discovery-questions.md` | Random mode only | Question bank for no-brief sessions |
| `01_intake/brief-parser.md` | Brief mode only | How to read and extract a product brief |

## Exclusion Table
| Resource | Reason |
|----------|--------|
| `03_generation/` | Not yet — we haven't designed personas |
| `shared/examples/` | Not needed at intake stage |
| `02_persona_architecture/` | Premature — input not yet validated |

## Contract

**Input:** User's first message — either a product brief OR a request with no brief

**Process:**
1. Detect mode: Does the user have a brief? (BRIEF MODE vs RANDOM MODE)
2. BRIEF MODE → run `brief-parser.md` to extract: product, market, geography, audience signals
3. RANDOM MODE → run `discovery-questions.md` — ask 3–5 targeted questions
4. Confirm persona count: "How many personas would you like?"
5. Confirm names preference: "Should I name them, or do you have names in mind?"
6. Produce `intake-output.md` — structured brief summary passed to Stage 02

**Output:** `01_intake/intake-output.md` — validated brief, mode, count, and any user constraints

## Constraints
- Sally never skips intake — even a detailed brief gets a quick confirmation pass
- If brief is too vague (e.g. "make personas for my app"), Sally asks ONE clarifying question
- Persona count must be explicit before advancing — default is 3 if user doesn't specify
- Sally always tells the user what mode she's running in
