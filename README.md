# Design Skills for Claude & AI Agents

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Skills Standard](https://img.shields.io/badge/Format-Agentic%20Skills%20(SKILL.md)-blue)](https://github.com)
[![npm version](https://img.shields.io/npm/v/design-skills.svg?style=flat)](https://www.npmjs.com/package/design-skills)

A curated collection of modular, production-grade design, UI, and UX skills for Claude and AI coding agents. These skills give your AI assistant expert guidance on design systems, visual hierarchy, layout polish, accessibility, and component refinement.

---

## ⚡️ Quick Start (No Install Needed)

You can run and install design skills on-demand using `npx`:

```bash
# 1. View all available design skills
npx design-skills list

# 2. Install for Claude Code (into .claude/skills/)
npx design-skills add improve-ui-ux --claude

# 3. Install for Antigravity & Agent IDEs (into .agents/skills/)
npx design-skills add improve-ui-ux --agent

# 4. Install globally across all projects on your machine
npx design-skills add-all --claude --global
npx design-skills add-all --agent --global
```

---

## 📌 Table of Contents

- [Overview](#overview)
- [How to Use](#how-to-use)
- [Available Skills](#available-skills)
- [Authoring New Skills](#authoring-new-skills)
- [License](#license)

---

## 📖 Overview

Design consistency and UI polish often get lost when writing code with AI assistants. **Design Skills** solve this by injecting structured, battle-tested design constraints and workflows directly into your agent's execution context.

Each skill follows the standard **`SKILL.md`** specification with YAML frontmatter, strict constraints, and actionable design checklists.

---

## 🚀 How to Use

### Via CLI (Recommended)

```bash
# See all skills
npx design-skills list

# Install a specific skill (current project)
npx design-skills add <skill-name> --claude
npx design-skills add <skill-name> --agent

# Install all skills at once
npx design-skills add --claude
npx design-skills add --agent
```

> **`--global`** installs to your home directory (`~/.claude/skills/` or `~/.gemini/config/skills/`), making the skills available across **every project** on your system.

---

## 🎨 Available Skills

| Skill | Focus | Description |
|---|---|---|
| **`improve-ui-ux`** | UI Polish & Ergonomics | Refines React component layouts, spacing, typography, responsiveness, accessibility, and state handling without breaking business logic. |

*(More design, design-system, and UX audit skills coming soon!)*

---

## 🛠 Authoring New Skills

To add a new skill to this repository:

1. Create a new directory named after your skill (e.g. `audit-accessibility`).
2. Add a `SKILL.md` file with standard YAML frontmatter:
   ```markdown
   ---
   description: Audits UI components for WCAG 2.1 AA accessibility compliance.
   ---

   # Task:
   ...
   ```
3. Add the folder name to `"files"` in `package.json`.

---

## 📄 License

MIT © [Sandeep Tripathy](https://github.com/thrisswell)
