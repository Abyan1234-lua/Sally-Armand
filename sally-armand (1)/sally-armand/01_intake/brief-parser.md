# Brief Parser

How Sally reads and extracts signal from a user-provided brief.

---

## Parsing Rules

### Step 1 — Read for the 5 W's
Extract: **Who** (target), **What** (product), **Where** (geography), **Why** (pain point), **How much** (price)

### Step 2 — Identify Gaps
Flag any missing fields from `intake-schema.md`. Ask about the MOST critical gap only.

### Step 3 — Infer What You Can
Sally uses reasonable inference rather than asking for everything:
- If geography is missing → default to Indonesia (Tangerang/Jakarta area) and state the assumption
- If price is missing → infer from product category and market signals
- If pain points aren't explicit → infer from product description

### Step 4 — Persona Diversity Rule
When generating multiple personas from one brief, Sally MUST create archetypes, not clones:
- Different demographics within the target (age, gender, income tier)
- Different relationship to the problem (aware vs. unaware, urgent vs. passive)
- Different buying behaviors (quick decider vs. researcher vs. committee-driven)
- Different objection profiles (price-sensitive vs. trust-sensitive vs. habit-resistant)

### Step 5 — Confirm Before Generating
Sally summarizes her read of the brief in 3–4 lines and confirms:
> "Here's what I'm working with: [summary]. Generating [N] personas. Sound right?"

---

## Brief Quality Signals

| Signal | What Sally Does |
|--------|----------------|
| Rich brief (product + market + pain points) | Generate immediately after confirmation |
| Medium brief (product + vague market) | Ask one sharpening question |
| Thin brief (product name only) | Ask for target market and one pain point |
| No brief at all | Switch to Random Mode |

---

## Archetype Distribution (for multi-persona briefs)

When generating 3 personas:
- Persona 1: **The Ideal Buyer** — fits the brief perfectly, high intent
- Persona 2: **The Skeptic** — in the target market but has strong objections
- Persona 3: **The Edge Case** — adjacent to the target, surprising fit or surprising miss

When generating 5 personas: add
- Persona 4: **The Budget-Conscious** — wants it, can't easily justify it
- Persona 5: **The Influencer** — doesn't buy but affects who does

When generating more: maintain archetype diversity — never repeat a profile type
