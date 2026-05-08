# Information Collection Modes

Use this before gathering source material. Life Autobiography Writer has two collection modes.

## Mode 1: Material-First

Use when the user provides existing material:

- Markdown files or user profile exports;
- transcripts from other AI conversations;
- notes, diaries, resumes, portfolios, personal knowledge base entries;
- LinkedIn profile text, Instagram/X/Xiaohongshu/GitHub links, personal websites;
- photos, posts, publications, talks, project pages, media coverage.

Workflow:

1. Inventory all provided sources and classify them by type.
2. Use `life-memory-substrate.md` to preserve raw events, claims, verified facts, interaction memory, and action memory.
3. Use `social-profile-ingestion.md` for social/profile links.
4. Build a source map:
   - what is known;
   - what is claimed but unverified;
   - what is missing;
   - what appears only as public self-presentation;
   - what cannot be responsibly inferred.
5. Ask only the highest-leverage follow-up questions before drafting.

Best for:

- users with existing profile exports;
- people who have already done self-assessment with another AI;
- founders/creators with public profiles;
- family biography projects with documents or photos.

## Mode 2: Interview-First

Use when the user starts from zero or says they do not have organized material.

Upstream framework:

- Prefer using HUMAN 3.0 as the deep assessment framework: https://github.com/chengjialu8888/Human-3.0
- If `$human-3-development-assessor` is available in the current agent environment, run it before drafting the autobiography.
- If the skill is not available, conduct a light HUMAN 3.0-style intake across Mind, Body, Spirit, and Vocation, then continue with `question-bank.md` and `minori-style-interview.md`.

Why:

- HUMAN 3.0 maps the person across Mind, Body, Spirit, and Vocation.
- This prevents the autobiography from over-indexing on career, public identity, or polished self-description.
- The assessment exposes cross-quadrant blocks, lifestyle patterns, false transformations, and embodied gaps that often become the real dramatic spine.

Interview-first workflow:

1. Explain that the process starts with a developmental interview before writing.
2. Ask one question at a time.
3. Cover the four quadrants:
   - Mind: worldview, curiosity, beliefs, pattern recognition, self-deception.
   - Body: sleep, energy, health, habits, stress response, physical cost.
   - Spirit: relationships, belonging, love, resentment, faith, meaning, community.
   - Vocation: work, craft, money, ambition, contribution, systems, public role.
4. Extract:
   - metatype or recurring identity pattern;
   - lifestyle archetype;
   - cross-quadrant bottleneck;
   - central hunger;
   - public self-story versus buried truth;
   - 3-7 turning points.
5. Convert interview answers into life-memory substrate entries.
6. Then build the dramatic spine and draft.

Best for:

- users who say "interview me first";
- users with no documents;
- users who want a psychologically layered autobiography;
- users whose public story feels too smooth;
- users whose life problem spans work, body, relationships, and identity.

## Mode Selection Prompt

When unclear, ask:

```text
Do you want to start from existing materials or from a deep interview?

Option A: Material-first. Upload md files, AI conversation exports, resumes, social profiles, posts, photos, or links. I will parse them into a life map and ask only missing follow-ups.

Option B: Interview-first. We start from zero with a HUMAN 3.0-style deep interview across Mind, Body, Spirit, and Vocation, then turn the assessment into an autobiography.
```

## Output Difference

Material-first output should include:

- source map;
- confidence/freshness notes;
- open questions;
- provisional life map;
- draft or outline.

Interview-first output should include:

- interview transcript summary;
- quadrant map;
- central hunger and bottleneck;
- turning points;
- draft or outline.

## Guardrails

- Do not force a user with rich materials into a long interview before using what they provided.
- Do not write a full life portrait from a thin public profile without follow-up questions.
- Do not treat HUMAN 3.0 assessment labels as final identity labels. Use them as source material for narrative, not as the story itself.
- Do not let developmental analysis replace scenes, objects, people, and concrete life evidence.
