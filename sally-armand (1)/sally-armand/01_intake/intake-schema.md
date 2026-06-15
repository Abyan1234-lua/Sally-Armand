# Intake Schema

Sally collects these fields before generating any persona.

## BRIEF MODE — Required Extractions

| Field | Description | Required? |
|-------|-------------|-----------|
| `product_name` | What is the product or service called | Yes |
| `product_category` | SaaS, physical product, service, app, etc. | Yes |
| `product_description` | What it does in 1–2 sentences | Yes |
| `target_market` | Who it's for — as specific as possible | Yes |
| `geography` | Country, city, region — or global | Yes |
| `price_range` | Rough price point or tier | Optional |
| `pain_points` | Problems the product solves | Optional |
| `competitors` | Who else is solving this | Optional |
| `persona_count` | How many personas to generate | Yes (default: 3) |

## RANDOM MODE — Discovery Questions

Sally picks 3–5 questions from `discovery-questions.md` based on what the user has already said.
At minimum, Sally always asks:
1. What industry or world should this persona live in? (or "truly random — surprise me")
2. What's the persona's approximate age range or life stage?
3. How many personas do you want?

## Validation Rules

- If `product_description` is under 10 words → ask for more detail
- If `target_market` is "everyone" or "anyone" → flag this and ask for a narrower slice
- If `geography` is missing in Brief Mode → default to Indonesia and confirm
- If `persona_count` > 10 → warn the user this will take longer and confirm

## intake-output.md Format

```markdown
## Intake Summary

**Mode:** [BRIEF / RANDOM]
**Product:** [name + 1-line description]
**Target Market:** [who they are]
**Geography:** [location]
**Price Point:** [if known]
**Pain Points:** [list]
**Persona Count:** [N]
**Special Instructions:** [any user-specific constraints]
```
