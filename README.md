# Articulation Skill

## 为什么做这个 Skill

这是我做的第一个 skill。

起因很简单：我见过太多 superior，在发现下属的认知需要升级时，说不清楚问题到底出在哪，更给不出一条清晰的路径。不是他们不懂，是他们没法把"懂"变成对方能接收的语言。

大多数人以为 AI 解决了写作问题——你说几句，它帮你生成一整篇。但这恰恰是最大的误解。**真正的问题从来不是"写不出来"，而是：写出来的东西，读完之后，对方不会改变任何想法，不会采取任何行动。** AI 帮你打了字，但没帮你说服任何人。

"写作"不等于"把字打出来"。写作是改变读者脑中的认知结构。

面对不同的人，你要做的事完全不同——是翻转他们的理解？补上他们不知道的一块？还是把他们已经知道的东西打得更深？你对着一个初学者和一个比你资深的上级，不可能用同一种方式写。

这个 skill 做的事情是：**先问清楚你要写给谁、你想对他们的认知做什么，然后用一套结构化的技巧帮你真正改变读者的想法。** 向下翻转下属的认知盲区，向上给上级递一块他缺的拼图——都能用。

**Author:** Liduo from Eazillion Global Ltd. (partner company of moody and Halliday)

## Repository Overview

This repository contains the **Articulation Skill** — a persuasive writing system designed as an AI skill definition. The skill teaches a structured, audience-first workflow for creating content that persuades, reframes, and educates.

## Repository Structure

```
articulationskill/
├── README.md            # This file — repo overview and guidance
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
