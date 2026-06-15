# Sally Armand — Buyer Persona Architect

> "I don't build marketing segments. I build people you can actually pitch to."

---

## What Sally Does

Sally Armand generates psychologically rich buyer persona markdown files — one file per persona —
designed for pitch simulation. Load a persona into your Claude Project and pitch your product
to a real-feeling human being who will engage, object, probe, and either come around or walk away.

---

## Two Modes

### BRIEF MODE
You have a product. Give Sally a brief.

```
/sally-armand

Brief: I'm building a WhatsApp-based order management tool for Indonesian warung owners.
Target: Small food/drink stall owners in tier-2 cities, 35–55 years old.
Price: IDR 50k/month flat.
Generate: 4 personas
```

Sally extracts the market signals, designs 4 distinct archetypes, and generates 4 persona `.md` files.

---

### RANDOM MODE
No brief. Sally asks 2–3 quick questions and surprises you.

```
/sally-armand

No brief. Give me 2 random personas. Somewhere in Indonesia. Any industry.
```

Sally runs discovery, picks from her industry pool, and generates fully-formed personas
you didn't expect — but can still learn from.

---

## Pipeline Stages

| Stage | What Happens |
|-------|-------------|
| `01_intake` | Mode detection, brief parsing or discovery questions, count confirmation |
| `02_persona_architecture` | Archetype assignment, demographic design, brief-fit scoring |
| `03_generation` | Full persona markdown written — every field filled with specific detail |
| `04_review` | Quality gate — realism check, simulation header verification, diversity audit |
| `05_output` | Files packaged and delivered for download |

---

## How to Use Persona Files for Pitch Simulation

1. Download one or more persona `.md` files from Sally's output
2. Upload the file to your Claude Project (as a Project document)
3. Open a new conversation in that Project
4. Say: **"I want to pitch [your product] to you."**
5. Claude will respond as the persona — in character, with their real objections and buying signals
6. Practice until you can consistently reach their Win Condition

**Pro tip:** Each persona file has a `<!-- SIMULATION HEADER -->` block at the top. This block tells Claude exactly how to be that person. You never see it — it just works.

---

## Persona File Naming

Files are named: `firstname-lastname.md`

Example: `diana-lestari.md`, `budi-santoso.md`, `rahel-tadesse.md`

Each file is self-contained and simulation-ready as soon as it's downloaded.

---

## Sally's Quality Standard

Every persona Sally ships must pass these bars:

- **Specificity** — no generic fields; every detail is grounded in a real person's life
- **Contradiction** — every persona has at least one internal tension (human, not cardboard)
- **Objection authenticity** — objections are rooted in biography, not generic risk aversion
- **Simulation readiness** — the simulation header is filled, tested, and character-consistent
- **Archetype diversity** — no two personas in a batch are the same type

---

## Folder Structure

```
sally-armand/
├── SKILL.md                              ← Trigger description
├── CONTEXT.md                            ← Master pipeline contract
├── README.md                             ← This file
├── 01_intake/
│   ├── CONTEXT.md
│   ├── intake-schema.md
│   ├── discovery-questions.md
│   └── brief-parser.md
├── 02_persona_architecture/
│   ├── CONTEXT.md
│   └── archetype-matrix.md
├── 03_generation/
│   └── CONTEXT.md
├── 04_review/
│   ├── CONTEXT.md
│   └── review-checklist.md
├── 05_output/
│   ├── CONTEXT.md
│   └── output-formats.md
└── shared/
    ├── glossary.md
    ├── references/
    │   ├── persona-anatomy.md
    │   ├── simulation-header.md
    │   ├── psychology-frameworks.md
    │   └── industry-pool.md
    ├── templates/
    │   └── persona-template.md
    └── examples/
        └── diana-lestari.md
```

---

## Triggering Sally

In any Claude session, say:
- `/sally-armand` + your brief or request
- "Sally, generate me 3 personas for..."
- "Create buyer personas for [product]"
- "Random buyer persona, no brief"
- "Buat buyer persona untuk..."

Sally will take it from there.
