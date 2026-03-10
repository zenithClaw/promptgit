# PromptGit

> Version control for AI prompts. Stop guessing which edit made things better.

**[Try it live →](https://zenithclaw.github.io/promptgit/)**

---

## The Problem

You've been tweaking the same prompt for an hour.

You change one word — the output shifts. You change it back — you've already lost the previous version. You have no idea which version was actually the best. You're flying blind.

There's git for code. Why not for prompts?

---

## What It Does

### 📝 Version History (like git log)
Every time you save, PromptGit creates a version with:
- A short hash identifier (e.g. `a3f9bc2`)
- Your commit message (optional but useful)
- Timestamp and character count

You can click any version to restore it instantly.

### 🔍 Word-Level Diff
Click any version to see **exactly what changed** — not just line-by-line, but word-by-word:
- 🟢 Green = words added in the newer version
- 🔴 Red (strikethrough) = words removed

This is especially useful for prompt engineering where a single word change ("concise" vs "brief", "list" vs "enumerate") can dramatically affect AI output quality.

### ↔️ Side-by-Side Compare
Switch to Compare mode, select two versions, and read them side by side. Useful when you want to understand the structural difference between a simple prompt and a heavily engineered one.

### 🔒 100% Local, No Accounts
All data stays in your browser's localStorage. Nothing is sent to any server. No signup. No tracking. Works offline.

---

## Who It's For

- **Prompt engineers** iterating on system prompts
- **Developers** building AI features and tuning model behavior
- **Anyone** who's spent too long trying to remember which version of a prompt worked best

---

## Roadmap

- [ ] **AI Output Compare** — run two versions through the API, compare outputs side by side (the real killer feature)
- [ ] Export/import version history as JSON
- [ ] Keyboard shortcuts (Cmd+S to save, etc.)
- [ ] Tag versions as "best" / "baseline"
- [ ] Share a snapshot via URL

---

## Stack

- Pure HTML + CSS + JS (zero dependencies, no build step)
- localStorage for persistence
- LCS algorithm for word-level diff

---

## Running Locally

Just open `index.html` in a browser. That's it.

```bash
git clone https://github.com/zenithClaw/promptgit
open promptgit/index.html
```

---

Built by [@WowTse66900](https://x.com/WowTse66900) · [Live Demo](https://zenithclaw.github.io/promptgit/)
