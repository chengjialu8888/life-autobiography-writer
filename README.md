![Life Autobiography Writer](assets/github-header.svg)

# Life Autobiography Writer

[中文 README](README.zh-CN.md)

> An Agent Skill for writing vivid, interview-driven life autobiographies and literary profiles.
>
> Do not write praise. Write recognition.

Most biography prompts produce a polished resume with nicer adjectives.

This skill does something else. It helps a personal agent interview a person from multiple angles, find the life origin, excavate charged scenes, question the official story, and write a portrait with charisma, contradiction, cost, tenderness, and human texture.

It is built for memoir ghostwriting, personal archives, founder profiles, family biographies, creator stories, reflective self-narratives, and any life story that should feel alive instead of promotional.

New: paste social profile links (Instagram, LinkedIn, X/Twitter, Xiaohongshu, GitHub, personal websites, newsletters, etc.) and let your agent turn public traces into a provisional life map, interview plan, and biography draft.

## Why It Exists

Many life stories fail in one of two ways:

- They become a career timeline.
- They become flattery.

Real people are more interesting than both. A good portrait should let the reader hold several truths at once:

- why the person became admirable,
- why the person became difficult,
- what the person paid for becoming themselves,
- why the person could not easily have become someone else.

Life Autobiography Writer gives your agent a repeatable writing system for that.

## What It Does

- Builds deep interview plans around origin, hunger, shame, ambition, family, work, body, relationships, and turning points.
- Converts scattered notes, user profiles, transcripts, or timelines into a dramatic life map.
- Supports two collection modes: material-first from uploads/social profiles/AI conversation exports, or interview-first via a HUMAN 3.0-style deep assessment.
- Parses social media/profile links into biography source material while preserving provenance, confidence, privacy, and open questions.
- Writes third-person literary profiles or first-person memoir chapters.
- Uses a Minori-style interview method inspired by writer-versus-subject biography dynamics: attracted, skeptical, patient, and unwilling to accept the polished version too quickly.
- Embeds a Wang Zengqi-inspired Chinese prose system for plain but flavorful writing: objects first, people second, pressure third, meaning last.
- Adds an English literary nonfiction mode: Chekhov-like humane attention, E. B. White-like clarity, Alice Munro-like undercurrents, and John McPhee-like structure.
- Runs an anti-flattery revision pass so the final text feels intimate, not worshipful.

## Best For

- Personal memoirs and autobiographies
- Founder, creator, or researcher profiles
- Family life stories
- Public figure portraits
- Career transition narratives
- Self-discovery documents
- Chinese literary nonfiction with human texture
- Agent-assisted interview and ghostwriting workflows

## Repository Structure

```text
life-autobiography-writer/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── anti-flattery.md
│   ├── autobiography-craft.md
│   ├── biographical-prose-style.md
│   ├── drama-method.md
│   ├── english-biographical-prose-style.md
│   ├── information-collection-modes.md
│   ├── life-memory-substrate.md
│   ├── minori-style-interview.md
│   ├── question-bank.md
│   ├── social-profile-ingestion.md
│   └── vendor/
│       └── wangzengqi-perspective/
│           └── SKILL.md
└── assets/
    └── github-header.svg
```

## Quickstart: Codex / Codex App

Install as a personal skill:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/chengjialu8888/life-autobiography-writer.git \
  ~/.codex/skills/life-autobiography-writer
```

Restart Codex so the skill metadata is reloaded.

Try:

```text
Use $life-autobiography-writer to interview me and write a third-person literary life profile.
```

Or provide material directly:

```text
Use $life-autobiography-writer to write a vivid autobiography sample from this profile.
Make it third-person, Chinese, restrained, and not flattering.
```

Or start from zero:

```text
Use $life-autobiography-writer to start from a deep interview.
Use HUMAN 3.0 / $human-3-development-assessor first if available.
Then turn the assessment into a psychologically layered autobiography.
```

Or start from social links:

```text
Use $life-autobiography-writer to parse these social profiles and write a provisional life map:
LinkedIn: [paste full profile text here if possible; LinkedIn links often hit an authwall]
X/Twitter: ...
Instagram: ...
Xiaohongshu: ...
Then ask me follow-up questions before drafting.
```

## Quickstart: Claude Code

Claude Code supports Agent Skills as folders with a `SKILL.md` file.

Install as a personal skill:

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/chengjialu8888/life-autobiography-writer.git \
  ~/.claude/skills/life-autobiography-writer
```

Or install as a project skill:

```bash
mkdir -p .claude/skills
git clone https://github.com/chengjialu8888/life-autobiography-writer.git \
  .claude/skills/life-autobiography-writer
```

Restart Claude Code, then ask:

```text
Use $life-autobiography-writer to turn these interview notes into a chapter outline and opening scene.
```

Claude may also load the skill automatically when your request matches the description.

## Quickstart: Other Personal Agents

If your agent supports the Agent Skills folder format, install this repository as a skill folder and make sure `SKILL.md` is at the root of the skill directory.

If your agent does not support skills yet:

1. Add `SKILL.md` as high-priority instructions.
2. Add the `references/` folder as retrievable context or knowledge.
3. Tell the agent to read only the reference files needed for the task.
4. Use prompts like:

```text
Follow the Life Autobiography Writer skill.
First build a life map from the source material.
Then write a third-person literary profile.
Use the anti-flattery pass before finalizing.
```

## Example Prompts

```text
Use $life-autobiography-writer to interview me.
Start from the question: what is the origin point of my life?
Do not write yet. First ask 10 sharp questions.
```

```text
Use $life-autobiography-writer to turn this founder timeline into a literary profile.
Make the person legible, complex, and attractive without sounding like PR.
```

```text
Use $life-autobiography-writer to write a Chinese third-person autobiography sample.
Use concrete objects, work scenes, relationships, and body costs.
Do not start with education or job titles.
```

```text
Use $life-autobiography-writer to revise this draft.
Remove flattery, add contradiction, and make the feeling land in scenes instead of abstract praise.
```

```text
Use $life-autobiography-writer to analyze this LinkedIn + X + personal website.
I pasted the full LinkedIn profile text below because LinkedIn may block unauthenticated page access.
Extract public self-story, recurring themes, contradictions, motifs, and missing interview questions.
Then write a third-person profile opening.
```

## Writing Philosophy

This skill follows four principles:

1. A life is not a resume.
2. A person is more interesting than their public myth.
3. Charisma comes from specificity and contradiction.
4. The best emotional writing often hides feeling inside objects, actions, weather, rooms, tools, food, and relationships.

In Chinese, the default style is third-person literary nonfiction with a Wang Zengqi-inspired mechanism: plain language, concrete things, human relationships, restrained feeling, and sentence flow.

In English, the skill uses a composite literary nonfiction mechanism rather than a single imitation: Chekhov for humane character attention, E. B. White for clean sentences, Alice Munro for undercurrents, and John McPhee for structure.

## Included Reference Modules

- `question-bank.md`: interview questions for origin, family, work, shame, ambition, relationships, and meaning.
- `information-collection-modes.md`: choose material-first or interview-first collection; interview-first can call Human-3.0.
- `minori-style-interview.md`: origin-point and core-hunger interview method.
- `drama-method.md`: television-style dramatic spine, reversals, supporting cast, motifs, and endings.
- `life-memory-substrate.md`: source-material management for raw events, claims, verified facts, interaction memory, and follow-up actions.
- `social-profile-ingestion.md`: one-link or multi-link social/profile ingestion for Instagram, LinkedIn, X/Twitter, Xiaohongshu, GitHub, blogs, and personal sites.
- `autobiography-craft.md`: memoir and biography craft patterns.
- `biographical-prose-style.md`: Chinese third-person prose adaptation.
- `english-biographical-prose-style.md`: English prose mode for humane, clear, undercurrent-rich literary nonfiction.
- `anti-flattery.md`: final revision pass against generic praise and brand-bio language.
- `vendor/wangzengqi-perspective/SKILL.md`: embedded full writing-style source for Wang Zengqi-inspired Chinese prose.

## Suggested GitHub Topics

`agent-skills`, `codex`, `claude-code`, `personal-agent`, `memoir`, `autobiography`, `biography`, `writing`, `ghostwriting`, `chinese-writing`, `literary-nonfiction`

## Contributing

Contributions are welcome, especially:

- better interview question sets,
- examples for different biography types,
- stronger anti-flattery revision rules,
- installation notes for more personal agents,
- multilingual writing adaptations.

Open an issue or PR with a concrete example of the writing problem you want the skill to solve.

## Star This Project

If this helps your agent write people as whole human beings instead of polished LinkedIn summaries, please star the repo. It helps more writers, founders, researchers, and personal-agent builders discover it.

## Placeholder Note

This README contains no benchmark numbers or fabricated usage metrics. Replace only the repository URL if you fork the project.
