# Vibe Coding — 6 Documents Before Code

Cursor rules + templates based on the [**Vibe Coding docs framework**](https://docs.google.com/document/d/1aPSJm7CGJ-MtRSOs82WWu7Rxtcrzn43_Sodqd652RRE/mobilebasic).

AI coding agents are powerful — but they're not mind readers. These **6 documents** eliminate ambiguity so Cursor and Claude Code build faster, with fewer hallucinations and less back-and-forth.

| # | Document | One-line purpose |
|---|----------|------------------|
| 01 | [PRD](docs/01-prd.md) | What you're building and for whom |
| 02 | [TRD](docs/02-trd.md) | Which tech, tools, and APIs you'll use |
| 03 | [App Flow](docs/03-app-flow.md) | Every page, every click, every navigation path |
| 04 | [UI/UX Brief](docs/04-ui-ux-brief.md) | How your app looks and feels |
| 05 | [Backend Schema](docs/05-backend-schema.md) | Data structure, tables, auth, relationships |
| 06 | [Implementation Plan](docs/06-implementation-plan.md) | The exact step-by-step build sequence |

## Quick start

### 1. Copy rules into your project

Copy the `.cursor/rules/` folder from this repo into your project root:

```bash
git clone https://github.com/yash0208/vibe-coding-cursor-rules.git
cp -r vibe-coding-cursor-rules/.cursor/rules your-project/.cursor/
```

Or install only the master rule if you want a lighter setup:

```bash
cp vibe-coding-cursor-rules/.cursor/rules/vibe-coding-master.mdc your-project/.cursor/rules/
```

### 2. Fill in the 6 documents

Copy the templates from `docs/` into your project:

```bash
cp -r vibe-coding-cursor-rules/docs your-project/docs
```

Fill each file before your first coding session. Use ChatGPT or Claude to draft them from a short conversation — paste the template and answer the prompts.

### 3. Start every AI session with context

Paste or reference your docs at the start of each Cursor or Claude Code session:

> Here are my 6 project documents. Use these as the source of truth for everything you build.

## What's included

```
.cursor/rules/
  vibe-coding-master.mdc          # Always-on: require docs before code
  vibe-coding-prd.mdc
  vibe-coding-trd.mdc
  vibe-coding-app-flow.mdc
  vibe-coding-ui-ux.mdc
  vibe-coding-backend-schema.mdc
  vibe-coding-implementation-plan.mdc
docs/
  01-prd.md … 06-implementation-plan.md   # Ready-to-fill templates
```

## Suggested workflow

1. **PRD** — get the product idea out of your head
2. **TRD** — lock the stack before anything else
3. **App Flow** — map navigation and journeys
4. **UI/UX Brief** — even "dark mode, minimal, like Notion" helps
5. **Backend Schema** — tables first, relationships second
6. **Implementation Plan** — phases with done criteria, not a flat task list

## Works with

- [Cursor](https://cursor.com) — rules in `.cursor/rules/`
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) — copy `docs/` contents into `CLAUDE.md` or project instructions

## License

MIT — use freely in personal and commercial projects.
