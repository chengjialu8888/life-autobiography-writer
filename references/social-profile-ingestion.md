# Social Profile Ingestion

Use this when the user provides one or more social media/profile links and wants a biography, autobiography sample, life map, or interview plan.

Supported sources include Instagram, LinkedIn, X/Twitter, Xiaohongshu, GitHub, personal websites, blogs, newsletters, podcasts, YouTube, TikTok, Medium, Substack, and public portfolio pages.

## Core Principle

Social profiles are curated evidence, not the whole person.

Treat profile content as:

- public self-presentation;
- timestamped raw events or claims;
- clues for interview questions;
- evidence of recurring interests, communities, work, taste, relationships, and identity;
- a surface that may hide what matters most.

Do not infer private motives, trauma, diagnoses, relationships, income, politics, sexuality, or family dynamics from social media alone.

## Access And Privacy

- Use only public or user-provided material.
- If a platform blocks access, requires login, hides posts, or rate-limits scraping, ask the user to export screenshots, text, archives, or selected posts.
- Do not bypass paywalls, privacy controls, account restrictions, or platform protections.
- Do not quote private comments, DMs, closed-group material, or third-party personal data unless the user has rights and permission.
- When writing about living third parties visible in social posts, anonymize or ask permission unless they are public figures in public contexts.

## Ingestion Workflow

1. **Inventory links**
   - List every provided profile URL.
   - Identify platform, handle/name, visible bio, and access status.
   - Ask whether the subject is the user, a consenting person, or a public figure.

2. **Capture public raw material**
   - Profile bio, tagline, pinned posts, profile image description, link-in-bio destinations.
   - Recent posts and high-signal older posts if accessible.
   - Work/education history from professional profiles.
   - Repeated topics, hashtags, communities, locations, collaborations, and media formats.
   - Visible milestones: launches, talks, jobs, moves, awards, failures, public reflections.

3. **Convert to life-memory substrate**
   - Save each observed item as `raw-event` or `claim`, not truth.
   - Attach URL, platform, handle, timestamp if visible, and capture date.
   - Mark confidence and freshness.
   - Link recurring people, projects, places, themes, and motifs.

4. **Extract profile signals**
   - Self-story: how the subject introduces themself.
   - Public role: what others are invited to see.
   - Repeated hunger: recognition, craft, freedom, belonging, impact, beauty, money, mastery, repair, escape, control, play.
   - Contradictions: what the profile emphasizes versus what it avoids.
   - Motifs: objects, places, tools, outfits, foods, phrases, work scenes, travel routes, screenshots, notebooks, stages, desks.
   - Communities: who appears around the person and what social worlds they move through.

5. **Build a provisional life map**
   - What can be known from public material.
   - What can only be inferred weakly.
   - What must be asked in interview.
   - Which posts or artifacts could become opening scenes.

6. **Write only after the source check**
   - Use social content as evidence and texture.
   - Avoid writing a full psychological biography from public posts alone.
   - If material is thin, produce an interview plan plus a short sample opening instead of pretending completeness.

## Platform-Specific Signals

### LinkedIn

Capture:

- headline, about section, work history, education, projects, featured links;
- career pivots, industry language, endorsements, public achievements;
- gaps, repeated positioning, claims of expertise, causes, communities.

Use for:

- chronology;
- vocation arc;
- public professional myth;
- contradictions between polished career story and other profiles.

Guardrail: LinkedIn is often the most resume-like source. Do not let it dominate the portrait.

### X / Twitter

Capture:

- pinned post, bio, recurring topics, replies, quote posts, long posts, threads;
- language habits, obsessions, enemies, intellectual communities, taste, humor;
- public shifts in opinion or identity over time.

Use for:

- mind and voice;
- social graph;
- repeated questions and intellectual hunger;
- public conflict or stance.

Guardrail: X rewards performance and compression. Treat intensity as platform behavior unless corroborated.

### Instagram

Capture:

- bio, highlights, captions, visual motifs, places, people, objects, aesthetic pattern;
- travel, family, work backstage, rituals, body presentation, lifestyle signals;
- repeated scenes: desk, studio, meals, events, streets, mirrors, landscapes.

Use for:

- sensory texture;
- public self-image;
- relationships and life rhythms;
- objects and places that can carry feeling.

Guardrail: Instagram is curated visual theater. Do not equate beauty with inner truth.

### Xiaohongshu

Capture:

- profile bio, notes, collections if visible, repeated life problems, practical advice, comments tone;
- consumption, identity, city life, career anxiety, beauty/body, travel, study, product choices;
- "what kind of life is being tested or desired."

Use for:

- lifestyle archetype;
- aspiration and anxiety;
- concrete objects and daily scenes;
- social comparison and self-making.

Guardrail: Xiaohongshu often blends diary, guide, commerce, and performance. Separate lived experience from content format.

### GitHub

Capture:

- profile README, repositories, commit activity, pinned projects, issues, stars, forks;
- project names, technical taste, learning trajectory, collaboration style.

Use for:

- craft evidence;
- builder identity;
- actual artifacts rather than self-description;
- recurring technical interests.

Guardrail: Do not infer work ethic, seniority, or private labor from commit graphs alone.

### Personal Website / Blog / Newsletter

Capture:

- about page, essays, project pages, archive chronology, topic clusters, public values;
- long-form voice, self-narrative, repeated metaphors, turning-point essays.

Use for:

- intellectual autobiography;
- mature self-story;
- source quotes and scene leads.

Guardrail: Long-form writing may be a retrospective construction. Ask what the draft left out.

## Source Note Template

```yaml
type: raw-event | claim | scene | motif | relationship-note | decision-log | action-memory
platform:
url:
handle:
captured_at:
post_date:
source_ref:
visible_text_summary:
visual_summary:
entities:
  people:
  places:
  projects:
  organizations:
themes:
motifs:
claim:
confidence: high | medium | low
freshness: active | stale | archived | unknown
privacy: public | sensitive | third-party-sensitive
follow_up:
  - question to ask
narrative_use:
```

## Social-to-Interview Questions

After ingesting links, ask 6-12 follow-ups:

- Your profile shows you repeatedly return to [theme]. What is the first scene behind that?
- Which post looks true but incomplete?
- Which public description of you has become too smooth?
- What part of your life never appears online?
- Which post would someone who loves you misunderstand?
- Which post would an enemy use against you, and what would they get right?
- What did you stop posting about, and why?
- Which object, room, tool, or place appears again and again?
- What public role do you perform well? What does it protect?
- Which turning point is visible only as a tiny caption, job change, deleted project, or sudden silence?

## Output Modes

Choose based on available material:

- **Social profile source map**: what each platform reveals, hides, and cannot prove.
- **Life map from links**: provisional timeline, themes, contradictions, motifs, open questions.
- **Interview plan**: follow-up questions generated from profile evidence.
- **Third-person profile draft**: clearly grounded in public material and marked as provisional where needed.
- **Opening scene options**: 3-5 possible openings drawn from visible posts, artifacts, or motifs.

## Autobiography Drafting Guardrails

- Say "the public profile suggests" when evidence is only public-facing.
- Say "what can be seen" rather than "what she/he/they secretly felt."
- Do not turn platform metrics into life value.
- Do not mistake content strategy for personality.
- Do not include exact quotes from posts unless allowed and relevant; summarize when possible.
- Do not write the final biography as a collage of posts. Use posts to find scenes, motifs, questions, and contradictions.
