---
type: system
date: 2026-06-30
tags:
  - system
  - vault-instructions
  - ai-first-rules
---

# wiki-ai-thinkers: Vault Instructions

This file governs all work in the wiki-ai-thinkers Obsidian vault. It imports global rules and defines vault-specific constraints.

---

## Import Global Rules

This vault inherits from the user's global instructions:

- **@~/.claude/rules/drafting-style.md** — NZ English, Hemingway principles, Strunk composition rules
- **@~/.claude/rules/mcp-tool-design.md** — MCP tool naming, schema, return shapes, error messages
- **@~/.claude/rules/tooling-spine.md** — GSD vs superpowers; GSD owns project state; superpowers executes craft
- **@~/.claude/rules/security.md** — Secrets, input validation, dependencies, access control, errors, files

**Override principle**: Vault-specific rules below supersede global defaults only where explicitly stated.

---

## 1. Vault Purpose and Scope

**Mission**: Collect authoritative primary sources from prominent AI researchers, founders, and policy thinkers; render them as a queryable knowledge graph that maps positions on AGI timelines, takeoff dynamics, alignment, economic impact, and policy.

**Not a contribution project**: This is a personal research vault that happens to be public. Pull requests adding or modifying thinkers will not be merged. Forks are encouraged.

**Audience**: Researchers, policymakers, investors studying AI governance and technical alignment; users querying the browser artefacts (positions matrix, force-directed graph).

---

## 2. Vault Structure and Folder Purpose

| Folder | Purpose | Governance |
|--------|---------|-----------|
| `00_Inbox/` | Unprocessed captures awaiting triage | Temporary; archive or move to 10_Sources weekly |
| `10_Sources/` | Raw ingested artefacts: papers, talks, articles, videos, media | One folder per thinker/source-slug; `source.md` schema required (see §3.2) |
| `20_People/` | One folder per thinker, holding profile, timeline, positions | `profile.md` required; `positions.md` optional; `timeline.md` optional |
| `30_Concepts/` | Atomic concept and theme pages (e.g., alignment, safety, governance) | Scaffold only; not auto-generated; hand-curated |
| `40_Domains/` | Domain overview pages | Scaffold only; not auto-generated; hand-curated |
| `50_MOCs/` | Maps of Content, dashboards, cross-cutting indexes | Both auto-generated (via wiki skill) and hand-curated |
| `60_Drafts/` | Work-in-progress essays and reports | Status: draft; move to permanent or archive |
| `70_Research/` | Active research threads; NotebookLM collection material | Ephemeral; archive when thread closes |
| `80_Attachments/` | Binary attachments (PDFs, images, cached copies) | Excluded from version control; not shipped in public vault |
| `90_Templates/` | Frontmatter and body templates used by Templater | Locked; changes require vault maintainer review |
| `99_Meta/` | Vault infrastructure: schema, build scripts, automation index, wiki-thinker state | **Locked schema** in `schema.md`; per-thinker state under `wiki-thinkers/` |
| `.workspace/` | Browser artefacts: `graph.html`, `positions.html`, server scripts | Read-only rendering layer; source of truth in vault frontmatter, not .workspace/ |

---

## 3. Frontmatter Schema and Controlled Vocabulary

**Master schema definition**: See `[[99_Meta/schema.md]]`. This section summarises and extends.

### 3.1 Fields Required on Every Note

| Field | Type | Enum values | Notes |
|-------|------|-------------|-------|
| `type` | string | `source`, `person`, `concept`, `moc`, `draft`, `question`, `timeline`, `position`, `meta` | Governs template applied; determines browser rendering |
| `status` | string | `inbox`, `draft`, `review`, `permanent`, `archived` | Lifecycle state; `permanent` means stable and part of core knowledge graph |
| `created` | date | ISO format (YYYY-MM-DD) | Creation date; immutable |
| `updated` | date (optional) | ISO format | Last modification; omit if never revised |
| `tags` | list | Free strings | Folksonomy; not controlled; lowercase, hyphenated preferred |

### 3.2 Person Notes (`type: person`)

**Template**: `90_Templates/person.md`

| Field | Type | Enum or format | Notes |
|-------|------|---|---|
| `name` | string | Display name | Full name or preferred form |
| `slug` | string | kebab-case | Must match folder name under `20_People/<slug>/` |
| `role` | string | `lab-leader`, `researcher`, `safety`, `economist`, `policy`, `forecaster`, `critic`, `hardware` | Primary role; one value only |
| `domain` | list | See 3.5 | Research focus areas; 1–3 preferred |
| `affiliations` | list | Freeform institution names | Current and past; no date ranges (use timeline.md for dates) |
| `timelines_view` | string | One-line summary | Stated position on AGI timeline; e.g., "AGI by 2030 with 50% confidence" |
| `takeoff_view` | string | One-line summary | Stated position on takeoff dynamics; e.g., "Fast takeoff via capability overhang" |
| `alignment_view` | string | One-line summary | Stated position on alignment difficulty; e.g., "Hard problem; requires architectural innovation" |
| `economic_view` | string | One-line summary | Stated position on economic impact; e.g., "Massive productivity gains in knowledge work" |
| `policy_view` | string | One-line summary | Stated position on governance/policy; e.g., "Prefers industry self-regulation" |
| `key_papers` | list | Wikilinks | Links to `10_Sources/Papers/[slug]/source.md`; top 5–7 |
| `key_talks` | list | Wikilinks | Links to `10_Sources/Media/[slug]/source.md`; top 5–7 |
| `key_essays` | list | Wikilinks | Links to `10_Sources/Articles/[slug]/source.md`; top 5–10 |
| `interview_archive` | list | Wikilinks | Podcast appearances, panel discussions; 3–5 |
| `first_public_work` | string | Freeform | Notable debut work or milestone; e.g., "char-rnn and Stanford CS231n (2015)" |

**Profile body structure**:
1. **One-line thesis**: 1–2 sentences capturing the thinker's core intellectual contribution
2. **Current role and affiliations**: Latest position and employer/institution
3. **Stated positions**: Subsections for timelines, alignment, economic impact, policy (mirrors frontmatter)
4. **Intellectual trajectory**: Brief chronology of key moves (institution, role change, founding)
5. **Key works**: Links to papers, essays, talks (can transcode from frontmatter)
6. **Related thinkers**: Wikilinks to peers or collaborators (3–5)
7. **Sources behind this profile**: Placeholder; populated by wiki-thinker-researcher agent

### 3.3 Source Notes (`type: source`)

**Template**: `90_Templates/source.md`

| Field | Type | Enum or format | Notes |
|-------|------|---|---|
| `title` | string | Artefact title | Publication title or talk name |
| `authors` | list | Author/speaker names | Include all primary authors; no wikilinks in this field |
| `thinker` | list | Wikilinks to `20_People/[slug]/profile` | Links to thinker profiles; must match at least one thinker in vault |
| `source_type` | string | `paper`, `talk`, `essay`, `interview`, `report`, `thread` | Artefact type; governs .workspace/ rendering |
| `venue` | string | Conference, journal, podcast, URL | Publication venue; e.g., "NeurIPS 2023", "Lex Fridman Podcast #333", "Blog" |
| `year` | integer | YYYY | Publication year |
| `url` | URL | Canonical link | Must be resolvable; use https:// |
| `doi` | string (optional) | DOI identifier | If applicable (papers, preprints) |
| `canonical_url` | string | Same as `url` | Used by PDF cache rebuilds; must match |
| `domain` | list | See 3.5 | Research domains covered by the work; 1–3 |

**Source body structure**:
1. **Citation**: Formatted citation in New Zealand Law Style Guide format where applicable; otherwise scholarly conventions
2. **One-line summary**: 1–2 sentences on the work's core claim or finding
3. **Key claims**: Bulleted list of major arguments or results
4. **Excerpts**: Quoted passages from the work supporting the claims above
5. **Significance**: Why this work matters to the knowledge graph; how it changes understanding of the thinker
6. **Related**: Wikilinks to related sources or thinkers

### 3.4 Timeline Notes (`type: timeline`)

**Template**: `90_Templates/timeline.md`

Used for `20_People/<slug>/timeline.md` only. Tracks institutional moves, role changes, major publications by year.

| Field | Type | Format | Notes |
|-------|------|--------|-------|
| `subject` | string | Wikilink | Link to the thinker's `profile.md` |
| `timeframe` | list | Entries with year and event | One entry per significant move; no date ranges unless ongoing |

### 3.5 Domain Enum (Controlled)

**Permitted values**:
- `alignment` — AGI alignment, safety, interpretability research
- `capability` — Model scaling, capability emergence, capabilities research
- `compute` — GPU/TPU hardware, training infrastructure, compute constraints
- `economics` — Economic impact, labour displacement, productivity, markets
- `governance` — Policy, regulation, international coordination, corporate governance
- `interpretability` — Model interpretability, mechanistic understanding, circuits
- `iot` — AI for Internet of Things, robotics, embedded systems
- `philosophy` — Philosophical foundations, consciousness, ethics
- `policy` — Government policy, regulation, international frameworks
- `robotics` — Robotics, embodied AI, autonomous systems
- `safety` — AI safety, alignment, long-term risks, s-risk
- `scaling` — Model scaling laws, training dynamics, emergent capabilities
- `takeoff` — Takeoff dynamics, fast takeoff, discontinuity, timelines

**Use**: Exactly one per source (preferred); up to three if the work spans multiple domains.

### 3.6 Browser Artefact Fields (Read-Only)

| Field | Type | Notes |
|-------|------|-------|
| `wiki_indexed` | ISO timestamp | Last time vault was indexed by the browser artefacts; auto-generated by wiki skill |
| `wiki_hash` | hex string | Content hash; changes trigger re-render in .workspace/ |
| `wiki_role` | string | Role in the knowledge graph; `wiki` = included, `meta` = system, `archive` = excluded |

---

## 4. Linking and Reference Conventions

### 4.1 Thinker References

**Format**: `[[20_People/<slug>/profile|Display Name]]`

**Example**: `[[20_People/andrej-karpathy/profile|Andrej Karpathy]]`

**Rule**: Always use the full path; use display name in pipe; link text should be the thinker's name, not description.

### 4.2 Source References

**Format**: `[[10_Sources/<Type>/<slug>/<source-id>|Source Title]]`

**Examples**:
- `[[10_Sources/Papers/andrej-karpathy/deep-visual-semantic-alignments-2015|Deep Visual-Semantic Alignments (2015)]]`
- `[[10_Sources/Media/andrej-karpathy/state-of-gpt-2023|State of GPT (2023)]]`

**Rule**: Link text should include year for disambiguation when a thinker has multiple sources on similar topics.

### 4.3 MOCs and Concept References

**Format**: `[[50_MOCs/<moc-name>|MOC Title]]` or `[[30_Concepts/<concept-name>|Concept Name]]`

**Rule**: Avoid transclusion (`![[...]]`). MOCs collect wikilinks; concepts list related sources.

### 4.4 Bidirectional Linking

**Rule**: Every source note must link to at least one thinker. Every thinker profile must link to at least one source (key_papers, key_talks, key_essays). Maintain symmetry.

---

## 5. Vault-Specific Workflows

### 5.1 Adding a New Thinker

1. **Create folder**: `20_People/<slug>/` (kebab-case, 2–3 words max)
2. **Create profile**: `20_People/<slug>/profile.md` using template; fill all frontmatter fields
3. **Write one-line thesis**: ~2 sentences
4. **Link to key sources**: Search 10_Sources for existing papers/talks by this thinker; add wikilinks to key_papers, key_talks, key_essays frontmatter
5. **Optionally create timeline**: `20_People/<slug>/timeline.md` if the thinker has a complex career arc worth tracking
6. **Set status to `draft`**: Change `status: draft` in frontmatter. Once sources are added and linked, change to `permanent`.

### 5.2 Adding a New Source

**Manual approach** (for urgent or one-off sources):
1. Create file: `10_Sources/<Type>/<thinker-slug>/<source-id>.md` (use title slug)
2. Copy template from `90_Templates/source.md`
3. Fill frontmatter: title, authors, thinker (wikilink), source_type, venue, year, url, domain
4. Write one-line summary and key claims
5. Add excerpt(s) and significance section
6. Link back to thinker profile: append wikilink to the profile's key_papers / key_talks / key_essays list

**Automated approach** (via wiki-thinker-researcher agent):
- Trigger the `wiki-thinker-researcher` subagent with a thinker slug
- Agent finds new primary-author papers, talks, articles, videos
- Agent writes one `source.md` per accepted candidate
- Agent appends wikilinks to the thinker's profile automatically
- Agent updates state under `99_Meta/wiki-thinkers/[slug]/`

### 5.3 Updating a Thinker Profile (Positions)

**When to update**:
- Thinker makes a major public statement that changes their stated position (timelines, alignment view, policy stance)
- New sources are added and shift the understanding of the thinker's position

**How to update**:
1. Edit the one-line thesis if the core thesis changes
2. Update the subsections under "Stated positions" with new quotes or evidence from new sources
3. Update frontmatter fields: `timelines_view`, `takeoff_view`, `alignment_view`, `economic_view`, `policy_view`
4. Add the thinker to a MOC if their position has changed significantly (e.g., moved from `who-believes-what` one row to another)
5. Update the `updated` date in frontmatter

**Rule**: Never rewrite historical positions. Add new sources and note shifts chronologically in the profile body.

### 5.4 Browser Artefact Workflow

**The browser artefacts** (graph.html, positions.html) in `.workspace/` are read-only rendering layers.

**Data flow**:
1. User modifies vault (adds thinker, updates profile, adds source)
2. User rebuilds vault index via wiki skill or browser script
3. `.workspace/` files read the vault's frontmatter and re-render

**Maintenance**:
- **Do not edit** `.workspace/` files manually. They are generated.
- **Do regenerate** after adding 2+ new thinkers or repositioning 3+ thinkers significantly
- **Start server** via `cd .workspace && ./serve.bat` (Windows) or `./serve.sh` (macOS/Linux)
- **Connect vault** via "Connect Vault" button in browser; pick this folder

---

## 6. Controlled Vocabulary: Role Enum

**Permitted values for person.role**:

| Role | Meaning |
|------|---------|
| `lab-leader` | Leads a research lab (e.g., Dario Amodei, Demis Hassabis) |
| `researcher` | Primary research contributor; no formal lab leadership (e.g., Andrej Karpathy at Anthropic pre-training) |
| `safety` | Focuses on AI safety, alignment, governance (e.g., Paul Christiano) |
| `economist` | Studies economic impact, labour markets (e.g., Daron Acemoglu) |
| `policy` | Works on policy, regulation, governance (e.g., Helen Toner) |
| `forecaster` | Makes AGI timelines predictions; prominent forecasting track record (e.g., Eliezer Yudkowsky historically) |
| `critic` | Public critic of AI progress or governance approach (e.g., Gary Marcus) |
| `hardware` | Focus on GPU, TPU, compute infrastructure (e.g., Brian Kernighan is NOT hardware; only if primary focus) |

**Rule**: Exactly one role per thinker. If a thinker spans multiple, choose the primary domain for 2026.

---

## 7. Version Control and Archival

### 7.1 What to Commit

**Commit to git**:
- `20_People/*/profile.md` (thinker profiles)
- `20_People/*/timeline.md` (timelines)
- `20_People/*/positions.md` (position essays)
- `10_Sources/**/source.md` (source citation notes)
- `30_Concepts/`, `40_Domains/` (scaffold)
- `50_MOCs/` (hand-curated MOCs only; auto-generated _wiki/ excluded)
- `90_Templates/` (locked schemas)
- `99_Meta/schema.md` (master schema definition)
- README.md, CLAUDE.md, LICENSE files

**Do not commit**:
- `80_Attachments/` (PDFs, cached copies; too large; excluded in .gitignore)
- `20_People/*/papers/` (cached PDFs)
- `.claude/worktrees/` (temporary work directories)
- `99_Meta/wiki-thinkers/state/` (per-thinker researcher agent state; not for publication)
- `.workspace/` (generated)

### 7.2 Archival

**When to archive a thinker**:
- Thinker dies or stops publishing for 2+ years
- Thinker moves out of AI field or becomes irrelevant to vault's mission
- Duplicate thinker (e.g., two profiles for the same person under different names)

**How to archive**:
1. Set `status: archived` in profile frontmatter
2. Set `wiki_role: archive` to exclude from browser artefacts
3. Move folder to `_archived/<year>-<slug>/` if desired (optional; status field sufficient)
4. Keep profile readable for historical reference

---

## 8. Pilot Thinker and Reference Implementation

**Pilot**: Dario Amodei

**Why**: Lab leader (Anthropic CEO); comprehensive source set; complex timeline (OpenAI researcher → co-founder → CEO); clear stated positions on timelines, safety, economics.

**Files to study**:
- `20_People/dario-amodei/profile.md` — reference implementation of person.md structure
- `20_People/dario-amodei/timeline.md` — reference implementation of timeline.md
- `20_People/dario-amodei/positions.md` — reference implementation of position essays
- `10_Sources/Papers/dario-amodei/*` (several sources linked) — reference implementations of source.md

---

## 9. Integration with Global Rules

### 9.1 Drafting Style (NZ English + Hemingway)

**Apply to**: All person profiles, MOCs, concept pages, and source summaries.

**Specifics**:
- **NZ English**: colour, favour, organise, centre, licence, realise
- **No adverbs**: Write "The takeoff will be fast" not "The takeoff will be very fast"
- **Short sentences**: Max 20 words per sentence in Stated Positions sections
- **Active voice**: "Dario argues X" not "It is argued by Dario that X"
- **Positive form**: "Alignment is a hard problem" not "Alignment is not an easy problem"

**Exception**: Quoted excerpts from thinkers preserve original language (may use adverbs, British/American spelling).

### 9.2 Security Rules (Apply to All Work)

**Secrets**: Never store API keys, GitHub tokens, or personal contact information in vault notes.

**Input validation**: When wiki-thinker-researcher agent fetches sources, validate URLs are resolvable and metadata is accurate before writing source.md.

**Data privacy**: Person profiles are public; do not include private correspondence, unpublished opinions, or personal details outside the public record.

---

## 10. Self-Check Before Committing

Run this checklist before pushing changes to vault:

- [ ] **Frontmatter complete**: All required fields filled; no blanks
- [ ] **NZ English**: No American spelling in prose (American preserved in quoted excerpts)
- [ ] **Wikilinks symmetric**: If profile links to source, source links back to profile
- [ ] **Domain enum valid**: All `domain` field values match 3.5 controlled vocabulary
- [ ] **Role enum valid**: All `role` values are in the Role enum (§6)
- [ ] **No adverbs in profiles**: Check "Stated positions" sections for very, clearly, largely, etc.
- [ ] **Short sentences**: Sentences under 20 words in position subsections
- [ ] **No secrets**: No API keys, tokens, or private contact info in any note
- [ ] **Status field set**: All notes have `status: inbox`, `draft`, `review`, `permanent`, or `archived`
- [ ] **Thinker slug matches folder**: If adding `20_People/andrej-karpathy/profile.md`, verify `slug: andrej-karpathy` in frontmatter
- [ ] **Source type valid**: All `source_type` values are paper, talk, essay, interview, report, or thread
- [ ] **URL resolvable**: Test `url` and `canonical_url` fields load without 404

---

## 11. Next Actions for Maintainers

1. **Quarterly thinker review** (Q3 2026): Add 2–3 new researchers rising in prominence; archive any who have exited AI field
2. **Source ingestion**: Run wiki-thinker-researcher agent weekly on active thinkers to capture new publications
3. **Browser artefact refresh**: Re-index and regenerate .workspace/ files monthly or after 10+ new sources
4. **MOC review**: Update cross-cutting MOCs (who-believes-what, themes) quarterly to reflect major position shifts
5. **Pilot thinker update**: Keep Dario Amodei profile current as reference implementation for new thinkers

---

## References

- **Master Schema**: `[[99_Meta/schema.md]]`
- **Templates**: `90_Templates/person.md`, `90_Templates/source.md`, `90_Templates/timeline.md`, `90_Templates/positions.md`
- **Browser Artefacts**: `.workspace/README.md` (server setup, browser API details)
- **Global Rules**: `~/.claude/rules/` (drafting-style, mcp-tool-design, tooling-spine, security)
- **Pilot Thinker**: `[[20_People/dario-amodei/profile|Dario Amodei]]`

---

**Last updated**: 2026-06-30  
**Governed by**: NZ English, Hemingway principles, security-first, vault-first rules  
**No contribution project**: Forks welcome; PRs adding or modifying thinkers will not be merged.
