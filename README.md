# Articulation Skill

## Repository Overview

This repository contains the **Articulation Skill** — a persuasive writing system designed as an AI skill definition. The skill teaches a structured, audience-first workflow for creating content that persuades, reframes, and educates.

**Author:** Liduo from Eazillion Global Ltd. (partner company of moody and Halliday)

## Repository Structure

```
articulationskill/
├── CLAUDE.md            # This file — guidance for AI assistants
└── articulation.md      # The complete articulation skill definition
```

This is a single-file content repository. There is no source code, build system, test suite, or CI/CD pipeline.

## What `articulation.md` Contains

The file is a skill definition written in Markdown with YAML frontmatter. It defines:

1. **Frontmatter** — Skill name, description, and trigger conditions (lines 1-13)
2. **Mandatory 4-Phase Workflow** — The core system:
   - **Phase 1: Audience & Context** — Identify audience type (Learner/Peer/Superior/Beginner) and context (Work/Newsletter-Public)
   - **Phase 2: Cognitive Operation** — Determine what happens to the reader's mind (Shift/Update/Deepening/Construction)
   - **Phase 3: Technique Selection & Writing** — Matrix of techniques per operation+audience, then structured writing execution (Hook → Preview → Key Points → Objection Handling → Ending)
   - **Phase 4: Reception Path Audit** — Post-draft quality check (single takeaway, minimum path, writer's-path contamination, length calibration, "4pm Friday" test)
3. **Key Principles** — Six core writing principles
4. **Technique Catalog** — 11 Taught Techniques (T1-T11) and 8 Hidden Techniques (H1-H8)
5. **Definition Flip Examples** — 23 worked examples of the H1 technique, plus a guide for creating new flips

## Key Conventions

### Skill Trigger Conditions

The skill activates when a user wants to write content (articles, posts, newsletters, memos, docs, presentations, talking points), frame arguments, persuade audiences, or struggles with structure. It takes priority over other writing skills for full content creation.

### Mandatory Workflow Order

The system enforces a strict sequential workflow:
- Phase 1 and Phase 2 must be completed with user confirmation **before** any writing begins
- Phase 4 (Reception Path Audit) must run on **every** draft before presenting to the user
- Never guess the audience type — ask follow-up questions if unclear

### Audience Types (4 categories)

| Type | Key Need |
|------|----------|
| **Learner** | The "aha" connecting vague feelings to precise names |
| **Peer** | New input, not new frameworks |
| **Superior** | Missing puzzle piece, delivered densely |
| **Beginner** | Cognitive map first, then small concrete steps |

### Context Types (2 categories)

- **Work** — Reader didn't opt in; respect their time; front-load core message
- **Newsletter/Public** — Reader opted in; earn continued attention; hook hard

### Cognitive Operations (4 types)

- **Shift** — Flip how they see it (requires Definition Flip + Pre-emptive Objection Handling)
- **Update** — Fill a gap (requires Cross-Domain Synthesis + Preview/Promise)
- **Deepening** — Make it hit harder (requires Evolution Ladder + Gentle Confrontation)
- **Construction** — Build from scratch (requires Teach-your-past-self + Progressive Key Points)

### Technique Notation

Techniques are referenced by ID throughout the document:
- **T1-T11** — Taught Techniques (explicitly named writing structures)
- **H1-H8** — Hidden Techniques (implicit patterns woven into writing)

## Development Guidelines

### Editing `articulation.md`

- Preserve the YAML frontmatter block (lines 1-13) — it defines how the skill is discovered and triggered
- Maintain the 4-phase structure — the workflow is sequential and each phase depends on the previous
- Keep technique IDs (T1-T11, H1-H8) consistent — they are cross-referenced throughout the technique selection matrix
- When adding new techniques, assign the next sequential ID and update the Technique Selection Matrix in Phase 3
- When adding definition flip examples, follow the established pattern: **N. Term** — Common meaning. Flip: reframed meaning. Effect: what changes.

### Content Integrity Rules

- The Technique Selection Matrix (Phase 3) must stay in sync with the Technique Catalog — every technique referenced must exist in the catalog
- Audience-Specific Technique Defaults section must cover all 4 audience types
- The Reception Path Audit (Phase 4) is non-negotiable — do not remove or weaken it
- The "4pm Friday test" is the final quality gate — keep it as the last audit step

### Writing Style Within the Skill

- Use imperative/instructional tone ("Ask the user...", "ALWAYS run this audit...")
- Use tables for structured comparisons (audience types, context types)
- Use bold for emphasis on key terms and technique names
- Use quoted dialogue format for example objection handling ("But what about X?")
- CAPS for critical workflow instructions (NEVER, ALWAYS, DO NOT)

## Branch Conventions

- `master` — Primary branch with the stable skill definition
- Feature branches for changes and updates
