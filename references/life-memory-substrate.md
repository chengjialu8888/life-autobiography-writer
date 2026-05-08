# Life Memory Substrate

Use this when collecting source material for a memoir, autobiography, life profile, family archive, or long-running personal knowledge base. The goal is to avoid turning life material into a flat pile of notes.

Treat the source base as a living memory system:

- **Factual memory**: what happened, where the evidence is, who owns or confirms it, and whether it is still valid.
- **Interaction memory**: why a decision happened, which alternatives existed, who disagreed, what assumptions were fragile, and what got lost when the event became an official story.
- **Action memory**: what the memory should trigger now: follow up, verify, revisit, ask someone, write a chapter, mark stale, or archive.

## Core Rule

Never turn raw life material directly into polished truth.

Move through this ladder:

1. **Raw event**: original interview answer, message, photo, timeline entry, document, memory fragment, meeting note, or observation.
2. **Claim**: an extracted assertion that may be true, partial, biased, outdated, or contradicted.
3. **Verified fact**: a claim supported by source material, repeated testimony, documentation, or subject confirmation.
4. **Interpretation**: what the fact may mean in the person's life story.
5. **Narrative use**: how it may appear in the autobiography or profile.

Keep these layers separate when material is sensitive, contested, or important.

## Minimum Metadata

For important source notes, preserve:

```yaml
type: raw-event | claim | verified-fact | decision-log | relationship-note | scene | action-memory
source: interview | document | message | photo | public-record | secondhand | inference
source_ref: URL, file path, person, transcript section, or note id
subject:
date_of_event:
date_recorded:
owner:
confidence: high | medium | low
freshness: active | stale | archived | unknown
privacy: public | private | sensitive | third-party-sensitive
status: raw | claim | verified | contradicted | fictionalized | excluded
related:
  - "[[person-or-theme]]"
follow_up:
  - question to ask, person to contact, evidence to request, or review date
```

Do not invent metadata. Use `unknown` when needed.

## Factual Memory For Life Writing

Use factual memory to prevent vague writing and false certainty.

Capture:

- dates, places, roles, relationships, institutions, moves, jobs, illnesses, losses, awards, public events;
- source and provenance: who said it, where it appears, when it was recorded;
- ownership: who can confirm or correct it;
- confidence and freshness: whether it is confirmed, partial, old, or likely outdated.

Biography use:

- Use high-confidence facts as scaffolding.
- Use medium/low-confidence claims as interview prompts or conditional language.
- Do not build a dramatic turn on a weak claim unless clearly marked.

## Interaction Memory For Life Writing

Use interaction memory to preserve the "why" behind life decisions.

For each major turning point, collect:

```yaml
type: decision-log
decision:
context:
visible_reason:
private_pressure:
alternatives:
why_not:
supporters:
opponents_or_doubters:
assumptions:
risks_underestimated:
who_paid_the_cost:
evidence:
open_questions:
```

Ask:

- What did the official story later say?
- What was happening before the official artifact existed?
- Who disagreed, hesitated, warned, or stayed silent?
- What alternative path was not taken?
- Which assumption later proved wrong or incomplete?
- What did the person know then, and what do they only know now?

This layer creates the difference between a timeline and a life.

## Action Memory For Life Writing

Use action memory to keep the biography process alive.

Examples:

```yaml
type: action-memory
trigger: "three mentions of the same unresolved relationship"
next_action: "ask for one concrete scene with this person"
owner: writer
status: open
review_at:
evidence:
  - source note id
```

Common actions:

- ask a sharper follow-up;
- request a photo, letter, post, calendar, document, or witness view;
- verify a date or role;
- mark a claim stale;
- move a motif into the chapter outline;
- exclude sensitive third-party material;
- revisit a contradiction after more material appears.

## Source Organization

For large projects, suggest a source folder like:

```text
life-archive/
├── 00-inbox/
├── 01-raw-events/
│   ├── interviews/
│   ├── documents/
│   ├── photos/
│   └── timelines/
├── 02-claims/
│   ├── facts/
│   ├── assumptions/
│   ├── decisions/
│   └── open-questions/
├── 03-entities/
│   ├── people/
│   ├── places/
│   ├── institutions/
│   ├── projects/
│   └── themes/
├── 04-synthesis/
│   ├── life-maps/
│   ├── chapter-outlines/
│   ├── motifs/
│   └── drafts/
├── 05-actions/
│   ├── follow-ups/
│   ├── verification-queue/
│   └── stale-checks/
└── 99-archive/
```

Use Obsidian-style wikilinks when useful, but do not let formatting work replace actual interviewing.

## Ingestion Prompt

Use this prompt when processing new material:

```text
Process this source material for a life-writing knowledge base.

1. Preserve the raw event summary without polishing it into truth.
2. Extract factual memory: people, places, events, dates, source, confidence, freshness.
3. Extract interaction memory: decisions, alternatives, objections, assumptions, risks, costs, unresolved questions.
4. Extract action memory: follow-up questions, evidence to request, claims to verify, stale items, possible motifs.
5. Separate raw material, claims, verified facts, interpretations, and narrative uses.
6. Mark privacy and third-party sensitivity.
7. Use wikilinks for recurring people, places, projects, and themes when appropriate.
```

## Writing Guardrails

- Do not flatten contested memories into a single confident sentence.
- Do not treat a subject's polished story as the whole truth.
- Do not use secondhand claims about living third parties as fact without permission or corroboration.
- Do not lose the source trail when converting notes into prose.
- Do not let metadata make the prose cold. Metadata protects the truth; scenes make the life readable.

## Final Source Check Before Drafting

Before writing, identify:

1. Which facts are verified.
2. Which claims are useful but uncertain.
3. Which scenes have direct evidence.
4. Which decisions have interaction memory.
5. Which sensitive areas require permission or omission.
6. Which motifs are repeated enough to carry narrative meaning.
