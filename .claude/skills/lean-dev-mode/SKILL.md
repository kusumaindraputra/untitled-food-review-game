---
name: lean-dev-mode
description: "Activate lean development mode — bypass the full design/architecture pipeline and go straight to coding. For game jams, solo experiments, and prototype-to-production shortcuts. Two modes: run with no args to set up a lean project, run with a feature description to implement it immediately."
argument-hint: "[feature-description] | --status | --reset"
user-invocable: true
allowed-tools: Read, Glob, Grep, Write, Edit, Bash, Task, AskUserQuestion
model: sonnet
---

# Lean Dev Mode

Lean dev mode strips away the full studio pipeline and replaces it with one loop:

```
/lean-dev-mode          ← first time: 3 questions, then you're coding
/lean-dev-mode [what]   ← every feature after that: describe it, code appears
```

**What's skipped:** brainstorm docs, art bible, systems map, GDDs, architecture docs,
ADRs, control manifest, UX specs, epics, stories, phase gates, director reviews.

**What remains:** game concept (one sentence), engine config, direct implementation.

**Review mode** is set to `solo` — no director gates, no approval chains.

---

## Phase 1: Parse Arguments and Detect Mode

**`--status`**: Read `production/lean-config.md` and print current lean setup (game
name, concept, engine, date started, features built). Stop — do not proceed further.

**`--reset`**: Ask "This will remove the lean config and return to standard workflow.
Are you sure?" via `AskUserQuestion` (Yes / No). If Yes, delete
`production/lean-config.md` and set `production/review-mode.txt` to `lean`. Stop.

**Feature description (any other non-empty argument)**: this is a **Build run**.
Check if `production/lean-config.md` exists.
- If yes → jump to Phase 4 (Build).
- If no → run Setup first (Phases 2–3), then continue to Phase 4.

**No argument**: this is a **Setup run**.
- If `production/lean-config.md` already exists, read it and show current config:
  > "Lean mode is already active. Game: [name] | Engine: [engine]
  > Run `/lean-dev-mode [feature]` to implement a feature.
  > Run `/lean-dev-mode --status` for full config."
  Stop — do not re-run setup.
- If not configured, run Setup (Phases 2–3).

---

## Phase 2: Setup — Three Questions

Ask these **one at a time** via plain text (not AskUserQuestion widgets — keep it
conversational). Wait for each answer before asking the next.

**Q1 — Game name**
> "What's the game called? (Working title is fine.)"

**Q2 — Concept**
> "One sentence: what is the game?"
> Example: "A roguelike where you review restaurants to gain power."

**Q3 — Engine** (only if engine is not already configured)
Read `.claude/docs/technical-preferences.md`. If the `Engine:` field is NOT
`[TO BE CONFIGURED]`, skip this question and use the configured engine.
Otherwise:

Use `AskUserQuestion`:
- Prompt: "Which engine are you using?"
- Options:
  - `Godot 4` — open source, great for 2D/3D, GDScript or C#
  - `Unity` — C#, large ecosystem, best mobile support
  - `Unreal Engine 5` — C++ or Blueprint, best for 3D/AAA visuals
  - `Other` — I'll describe it

If "Other": ask (plain text) "What engine and language?" and store the answer as-is.

---

## Phase 3: Write Minimal Scaffolding

After the three questions, confirm before writing:

> "Got it. I'll create a lean config and minimal project setup. Ready?"

Use `AskUserQuestion`:
- Options: `Yes, set it up` / `Wait — let me change something`

If "Wait": ask what they want to change, update accordingly, then confirm again.

If "Yes":

### Files to create

**`production/review-mode.txt`**
```
solo
```

**`production/stage.txt`**
```
Lean
```

**`production/lean-config.md`**
```markdown
# Lean Dev Config

- **Game**: [game-name]
- **Concept**: [one-sentence concept]
- **Engine**: [engine]
- **Language**: [language — derived from engine choice]
- **Started**: [today's date]
- **Mode**: solo (no director gates)

## Features built
<!-- lean-dev-mode appends here automatically -->
```

**`design/gdd/game-concept.md`** (only if it does not exist — do not overwrite)
```markdown
# [Game Name]

> [One-sentence concept]

*Note: Created in lean dev mode. Expand as needed.*
```

**`.claude/docs/technical-preferences.md`** (update Engine/Language fields only,
leave all other fields as-is):
- Set `Engine:` to the chosen engine
- Set `Language:` to the primary language for that engine:
  - Godot 4 → `GDScript` (default) or `C#` if user specified
  - Unity → `C#`
  - Unreal → `C++ / Blueprint`
  - Other → whatever the user said

Ask: "May I write these files?" before any writes. List them explicitly.

Once written, output:

```
## Lean mode active ✓

Game: [name]
Concept: [sentence]
Engine: [engine]

You're set up. To add a feature:
  /lean-dev-mode [describe the feature]

Examples:
  /lean-dev-mode player movement with WASD
  /lean-dev-mode main menu with play and quit buttons
  /lean-dev-mode enemy that patrols and chases the player
```

---

## Phase 4: Build — Direct Feature Implementation

This phase runs when a feature description is provided.

### 4a. Load context

Read in parallel (these are independent reads):
- `production/lean-config.md` → game name, concept, engine, language
- `.claude/docs/technical-preferences.md` → engine, language, naming conventions
- `design/gdd/game-concept.md` → any additional context about the game (if it exists
  and has more content than the lean stub)

### 4b. Classify the feature

Based on the feature description, determine:

| Feature type | Examples | Agent to spawn |
|---|---|---|
| Player movement / input | "WASD movement", "jump", "dash" | `gameplay-programmer` |
| Enemy / NPC behaviour | "patrol enemy", "boss fight", "shopkeeper" | `gameplay-programmer` or `ai-programmer` |
| UI screen / menu | "main menu", "pause screen", "HUD" | `ui-programmer` |
| Game system / mechanic | "inventory", "health system", "scoring" | `gameplay-programmer` |
| Visual effect / animation | "particle burst", "screen shake", "idle animation" | `gameplay-programmer` |
| Audio / sound | "footstep sounds", "background music" | `gameplay-programmer` |
| Foundation / engine setup | "project structure", "scene manager", "save system" | `engine-programmer` |
| Data / config | "enemy stats in JSON", "level config" | No agent — implement directly |

Also determine engine specialist to spawn alongside (only if the feature involves
engine-specific APIs or the engine has a post-cutoff knowledge gap — see
`docs/engine-reference/*/VERSION.md`):

| Engine | Specialist |
|---|---|
| Godot 4 | `godot-gdscript-specialist` or `godot-specialist` |
| Unity | `unity-specialist` |
| Unreal | `unreal-specialist` |

### 4c. Spawn programmer(s)

Spawn the programmer agent via Task with this briefing package:

```
Game: [name from lean-config]
Concept: [one-sentence from lean-config]
Engine: [engine] — [language]
Feature to implement: [feature description from argument]

This is a lean-mode project. There are no story files, ADRs, or architecture
documents to consult. Use sensible defaults for the engine and language.
Follow naming conventions from .claude/docs/technical-preferences.md if configured.

Output files should go in:
- Game code → src/
- Tests (if you write any) → tests/

Ask "May I write to [path]?" before creating any file.
```

If the engine specialist is needed, spawn them as a secondary agent with the
same briefing and instruction to validate engine-specific API usage.

### 4d. Collect and summarise

After the agent(s) complete:

1. List all files created or modified (with paths).
2. Note any engine-specific warnings the specialist raised.
3. Ask permission to append to `production/lean-config.md`:
   > "May I log this feature to your lean config?"
   Append under `## Features built`:
   ```
   - [date] [feature description] → [files created, comma-separated]
   ```

4. Output:
```
## Feature implemented: [feature description]

Files:
- src/[path] — [what it does]
- src/[path] — [what it does]

Run the game to test it. Come back with:
  /lean-dev-mode [next feature]
```

---

## Phase 5: Data / Config features (no agent)

If the feature is classified as Data/Config (Phase 4b), skip agent spawning.
Implement the data file directly:
- Ask "May I create [path]?" before writing
- Write the file to `assets/data/` or `src/data/` depending on the type
- Log the feature to lean-config.md as normal

---

## Lean Dev Loop Reference

Print this only at the end of a **Setup run** (not Build runs):

```
LEAN DEV LOOP
─────────────
1. /lean-dev-mode [feature]   → implement something
2. Test it in your engine
3. Repeat until done
4. Ship

Optional escalation paths:
  /prototype [concept]    → throwaway build to test a mechanic
  /dev-story [story]      → switch to full pipeline for a story
  /gate-check             → run a formal phase gate if needed
  /lean-dev-mode --status → see what's been built so far
```

---

## Collaborative Protocol

- Always ask "May I write to [files]?" before any Write or Edit operation.
- Group related files in one ask: "May I create these 3 files: [list]?"
- For spawned agents: they inherit this protocol individually.
- Never commit changes automatically — only write files when approved.

---

## What lean mode does NOT skip

- Permission to write files (always ask)
- Sensible naming conventions (use engine defaults if not configured)
- Working code (the agent must produce code that actually runs)
- The collaborative protocol from CLAUDE.md
