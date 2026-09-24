# AGENTS.md — wow-dashboard

Instructions for any coding agent (Codex, Claude Code, others) working in this repo.

## What this project is

A personal progression dashboard for one character: Balashotcala, a level 70
Draenei BM Hunter on TBC Classic Anniversary. It is hardcoded to that character
on purpose and serves as the reference design for the per-player dashboard the
wow-advisor project will generate (Phase 3 of the shared plan).

- Live site: https://mavdog33.github.io/wow-dashboard
- Hosting: GitHub Pages, single self-contained `index.html`

## Rules

- Keep it a single self-contained `index.html` with no build step.
- Character data (gear, reps, badge counts, gold, to-dos) changes only when the
  owner (Michael) provides new values. Never estimate or fill in game values.
- When a value changes, update every place it appears in the file; no stale copies.
- Reputation values are never lowered without the owner's confirmation.
- Game facts (item stats, drop sources) must come from a verified source such as
  tbc.cavernoftime.com or wowpedia.fandom.com, not memory.

## What to reuse elsewhere

The tab layout (To-Do with persistent checkboxes, Gear, Reps, Session Log), the
styling, and the checkbox/session-log patterns are what wow-advisor will
generalize. Changes here that improve those patterns are welcome; changes that
add more single-character hardcoding should stay in this repo only.

## Workflow

- Branch per task, merge by pull request. No direct commits to `main`.
- One-line changelog at the top of each PR description.
- Never commit secrets.
