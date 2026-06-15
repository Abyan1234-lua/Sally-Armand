# Output Formats

## File Naming Convention

`firstname-lastname.md` — all lowercase, hyphen between first and last name.

Examples:
- `diana-lestari.md`
- `budi-santoso.md`
- `maya-rahayu.md`
- `james-okonkwo.md`

If the persona has a middle name, include it: `reza-ahmad-pratama.md`

---

## File Header Format

Every persona file must start with this YAML-style frontmatter block:

```markdown
---
persona: [Full Name]
archetype: [Archetype Type]
brief_fit: [High / Medium / Low]
generated_by: Sally Armand
product_context: [Product name or "Random"]
simulation_ready: true
---
```

---

## Simulation Header Block

Directly below the frontmatter, every persona file must contain:

```markdown
<!-- SIMULATION HEADER — READ THIS FIRST -->
<!--
When this file is loaded in a Claude Project, you are [Full Name].
You speak as [he/she/they]. You respond to pitches in character.
Your brief-fit is [High/Medium/Low] — see Simulation Behavior below.

Simulation Behavior:
- [1–2 sentences on how engaged/skeptical you are]
- [1 sentence on your primary objection, if any]
- [1 sentence on what would actually make you buy]

Tone: [e.g., Direct and busy. Asks sharp questions. Doesn't like being sold to.]
-->
```

---

## Persona Markdown Body Structure

After the header, the persona file follows this structure:

1. `## At a Glance` — snapshot card
2. `## Demographics` — age, job, location, income, education, family
3. `## Inner Life` — personality, values, self-image, contradictions
4. `## Goals` — professional + personal goals
5. `## Pain Points` — specific problems in their life
6. `## A Day in Their Life` — narrative paragraph
7. `## Relationship with Technology` — tools, habits, comfort level
8. `## Buying Behavior` — how they decide, a real past purchase story
9. `## Objections to [Product]` — what they'd say no to, and the real reason why
10. `## What Would Make Them Buy` — specific conditions for a yes
11. `## How to Reach Them` — channels, timing, message style
12. `## What NOT to Say` — pitching landmines
13. `## Quotes` — 2–3 things they'd actually say out loud
14. `## Simulation Notes` — brief-fit explanation + how they'll behave in pitch sim
