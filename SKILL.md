---
name: life-autobiography-writer
description: Interview-driven life autobiography and profile writing. Use when the user wants Codex to interview a person, reconstruct a life story, ghostwrite memoir/autobiography chapters, create a moving biographical profile, parse uploaded materials or AI conversation exports, parse social media profile links (Instagram, LinkedIn, X/Twitter, Xiaohongshu, etc.) into biography source material, run a from-zero deep interview, or turn scattered memories into a vivid human portrait. Especially useful when the desired result should feel dramatic, psychologically layered, and charming without flattery, hagiography, generic inspiration, or corporate bio polish.
---

# Life Autobiography Writer

## Core Aim

Write a life as a dramatic human portrait: choices under pressure, contradictions, costs, wounds, appetites, craft, relationships, luck, self-deception, repair, and earned dignity.

Do not write praise. Write recognition.

For Chinese outputs, default to a third-person literary biographical voice unless the user explicitly asks for first-person memoir. Make the prose attractive through concrete things, human relationships, small actions, and sentence flow rather than through big claims. Read the embedded Wang Zengqi writing skill at `references/vendor/wangzengqi-perspective/SKILL.md` when writing or revising Chinese narrative prose. For English outputs, use `references/english-biographical-prose-style.md`: Chekhov-like humane attention, E. B. White-like clarity, Alice Munro-like undercurrents, and John McPhee-like nonfiction structure.

## Operating Principles

- Treat the subject as a protagonist, not a resume.
- Hunt for scenes before claims: rooms, weather, objects, gestures, dialogue, silences, money, food, clothes, deadlines, train rides, phone calls.
- Build charisma from specificity and contradiction, not adjectives.
- Let achievements carry shadows: what was sacrificed, misunderstood, avoided, learned too late, or paid for privately.
- Let flaws become plot engines, not moral verdicts.
- Ask from multiple angles before writing. The first answer is usually the public version.
- Preserve ambiguity when it is truer than explanation.

## Workflow

1. Define the assignment.
   - Ask who the subject is, who the intended reader is, the desired length, language, and whether the output is a memoir in first person or a biographical profile in third person.
   - Ask what the user does not want: apology, confession, brand bio, family tribute, business legend, therapy transcript, or pure chronology.

2. Gather source material.
   - Choose one of the two collection modes in `references/information-collection-modes.md`: material-first when the user provides uploaded files, AI conversation exports, notes, or social profiles; interview-first when starting from zero.
   - For interview-first work, read `references/interview-first-routing.md` before asking questions. Decide whether to start with HUMAN 3.0-style mapping, Minori-style narrative excavation, or the default hybrid route.
   - Interview in rounds. Start broad only when a whole-person map is needed, then return with sharper follow-ups.
   - Ask one question at a time. Tell the user the expected round length before starting. Never dump a full HUMAN 3.0 or Minori question list unless the user explicitly asks for the plan.
   - Request documents only when useful: timelines, photos, speeches, posts, letters, media reports, family notes, work artifacts.
   - If the user provides social media profile links, use `references/social-profile-ingestion.md` to capture public profile material, recent posts, recurring themes, self-presentation, work history, visible communities, motifs, and contradictions. Treat social media as curated evidence, not the whole person.
   - For LinkedIn, prefer asking the user to copy/paste the full profile text instead of only pasting a link, because LinkedIn often blocks unauthenticated access behind an authwall/data wall.
   - If the user starts from zero and wants a deep life interview, use HUMAN 3.0 as the upstream assessment framework for biography intake. If `$human-3-development-assessor` is available, use its Mind/Body/Spirit/Vocation logic as source material; do not automatically produce a full coaching report unless requested. Otherwise direct the user to https://github.com/chengjialu8888/Human-3.0 or ask the HUMAN 3.0-style biography intake in `references/interview-first-routing.md` before drafting.
   - If the user provides partial material, map what is known, what is missing, and what cannot be responsibly inferred.
   - Use `references/life-memory-substrate.md` when source material is large, fragmented, long-running, or intended to become a reusable personal knowledge base. Preserve raw events, separate claims from verified facts, capture why decisions happened, and attach provenance, confidence, freshness, and follow-up actions.

3. Build the dramatic spine.
   - Identify the central hunger: what the subject kept trying to prove, escape, protect, win, repair, or understand.
   - Identify the counterforce: family script, poverty, gender/class expectations, ambition, public image, illness, failure, loneliness, resentment, chance, or time.
   - Choose 3-7 turning points where the subject had to act before they fully understood themselves.

4. Write by scenes and pressure.
   - Open with a charged scene, not a summary.
   - Move between scene, reflection, and consequence.
   - Use chronology only as scaffolding; emotional causality matters more.
   - Include other people's views where available, especially conflicting views.
   - For Chinese prose, first read `references/vendor/wangzengqi-perspective/SKILL.md` for the complete Wang Zengqi writing protocol, then use `references/biographical-prose-style.md` to adapt that prose mechanism to life-writing: concrete object first, person second, pressure third, meaning last.
   - For English prose, use `references/english-biographical-prose-style.md` to combine humane character attention, clean sentences, quiet emotional undercurrents, and structured literary nonfiction.

5. Revise against flattery.
   - Replace generic praise with evidence.
   - Add costs, blind spots, and unresolved questions.
   - Remove fortune-cookie morals unless the subject actually earned them through a scene.
   - Make the reader feel: "I may not agree with this person, but I understand why they became this way."

## Interview Rounds

Use `references/question-bank.md` when the user needs discovery questions or when the subject feels flat.

Use `references/information-collection-modes.md` first when deciding whether to work from existing materials/social profiles or to start a deep interview from zero.

Use `references/interview-first-routing.md` for from-zero interviews. It defines when to activate HUMAN 3.0-style mapping, when to activate Minori-style narrative excavation, how to combine them, how many questions to announce, and how to ask one adaptive question at a time.

Use `references/minori-style-interview.md` when the user asks for a Minori-like interview inspired by the writer/subject dynamic in Netflix's `地獄に堕ちるわよ`: begin from the subject's life origin, core hunger, first charged childhood scene, and the difference between the self-told myth and the buried human truth.

Use `references/life-memory-substrate.md` when collecting, organizing, or maintaining biography source material as a living memory system rather than a flat pile of notes.

Use `references/social-profile-ingestion.md` when the user gives Instagram, LinkedIn, X/Twitter, Xiaohongshu, GitHub, personal website, newsletter, blog, podcast, or other social/profile links and asks for a one-link or multi-link autobiography/profile draft.

Default sequence:

1. Public chronology: origin, family, education, work, relationships, visible milestones.
2. Private weather: shame, envy, fear, hunger, tenderness, rituals, grudges, bodily memory.
3. Conflict map: who opposed them, who misread them, who saved them, who they hurt.
4. Scene excavation: ask for one day, one room, one sentence, one object, one decision.
5. Counter-narrative: ask what the official story leaves out.
6. Meaning test: ask what they now believe, and what they still cannot forgive or explain.

## Narrative Method

Use `references/drama-method.md` for television-style structure: teaser opens, episode arcs, reversals, supporting cast, motifs, cliffhangers, and scene cards.

Use `references/autobiography-craft.md` for memoir and biography craft patterns inspired by major autobiographical traditions: confessional, political, literary, investigative, celebrity, spiritual, immigrant, survivor, artist, and public-woman narratives.

Use `references/vendor/wangzengqi-perspective/SKILL.md` as the embedded full style source for Wang Zengqi-inspired Chinese prose: people, objects, weather, rooms, food, tools, local speech, restrained feeling, and sentence flow. Do not roleplay as Wang Zengqi while using this autobiography skill; borrow the writing mechanism.

Use `references/biographical-prose-style.md` to adapt the embedded Wang Zengqi method to autobiography and profile writing: vivid but restrained, third-person friendly, plain but flavorful, with feeling carried by objects, actions, weather, rooms, tools, food, work scenes, and relationships.

Use `references/english-biographical-prose-style.md` for English-language autobiography and profile writing. It is not an "English Wang Zengqi" imitation; it combines Chekhov's compassion, E. B. White's clean prose, Alice Munro's life undercurrents, and John McPhee's nonfiction structure.

Use `references/anti-flattery.md` before finalizing any draft.

## Output Forms

Choose the output form that matches the request:

- **Interview plan**: question rounds, follow-ups, evidence to request.
- **Life map**: timeline, themes, contradictions, unresolved mysteries, dramatic spine.
- **Chapter outline**: chapter titles, opening scenes, conflicts, emotional turns.
- **Sample opening**: 800-1500 words demonstrating voice and structure.
- **Full chapter**: scene-driven prose with transitions and reflective passages.
- **Profile**: third-person literary portrait for publication or personal archive.
- **First-person memoir**: ghostwritten "I" voice, based only on supplied material and clearly marked assumptions.

## Voice Rules

- For Chinese prose, prefer clean literary nonfiction: concrete, restrained, emotionally exact, plain but with aftertaste.
- For English prose, prefer literary nonfiction that is clear, concrete, psychologically alert, and structurally patient.
- Default to third-person narration for profile/autobiography reconstruction unless the user asks for first person.
- Write close to the person: their objects, rooms, tools, repeated gestures, phrases, working habits, relationships, and bodily costs.
- Avoid inflated modifiers such as "传奇", "伟大", "非凡", "无与伦比" unless the sentence proves them.
- Use a cinematic eye but not screenplay formatting unless requested.
- Let one sharp detail do the work of three explanations.
- Do not let concepts lead the paragraph. Let a thing, scene, action, or relationship lead; then lightly turn toward meaning.
- When the subject is controversial, make them legible without laundering harm.

## Integrity Rules

- Do not fabricate facts, quotes, relationships, trauma, diagnoses, or private motives.
- Mark invented bridge scenes as fictionalized if the user asks for literary reconstruction.
- Separate "known", "claimed", "reported by others", and "inferred".
- Ask permission before writing sensitive material about living third parties.
- If the material is thin, write a stronger interview plan before pretending to have a book.
