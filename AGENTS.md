# Course practice repository

## Agent skills

### Issue tracker

GitHub Issues in `cedrick5355-gif/cohort-004-project`. See `docs/agents/issue-tracker.md`. Verify the owner repository before writing; the instructor's repository is an upstream source.

### Triage labels

Use the five default triage labels. See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: root `GLOSSARY.md` and `docs/adr/`. See `docs/agents/domain.md`.

## Local development

Use the packageManager version pinned in package.json through Corepack: `corepack pnpm <command>`.
The existing app runs at http://127.0.0.1:5173/ with a local SQLite database. It is a practice platform with sample courses; the downloaded Matt Pocock course reference is separate.

Run the appropriate existing checks for changed behavior: `corepack pnpm test`, `corepack pnpm typecheck`, `corepack pnpm build`.
`db:seed` resets local sample data. `reset` can discard exercise work. Get explicit approval for a reset or reseed that replaces existing progress.

## Course reference

When this local reference exists, use `../../outputs/Matt Pocock Course/course-catalog.json` to find Matt's original videos, transcripts, and written lessons. Open `../../outputs/Matt Pocock Course/index.html` to watch and read together. These private course-reference files stay outside this Git repository.

The 38 pinned Matt skills live in `.agents/skills/` for Codex and are mirrored byte-for-byte in `.claude/skills/` for Claude Code. Keep both copies synchronized if deliberately updating them. Existing Claude course helper skills remain alongside the mirrors.
