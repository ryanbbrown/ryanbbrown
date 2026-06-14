# Hi, I'm Ryan 👋

> Shipping side projects at the intersection of AI, productivity, and my personal interests.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/-SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Swift](https://img.shields.io/badge/-Swift-FA7343?style=flat-square&logo=swift&logoColor=white)

## Current Projects
- 🔗 [ThinHarness](https://github.com/ryanbbrown/thinharness): A minimal, opinionated agent harness — focused scope, readable core, easy to fork
- 📝 [obsidian-drift](https://github.com/ryanbbrown/obsidian-drift): Native version control + accumulated IDE-like diff view for Obsidian (500+ downloads)
- 🚪 [AI Gate](https://github.com/inulute/ai-gate): Contributor to an Electron app for using ChatGPT, Claude, and Gemini in parallel, tmux-style workspaces
- 📚 [Kindle Storyteller](https://github.com/ryanbbrown/kindle-storyteller): iOS app for generating on-demand, live-syncing audiobook snippets using AI
- 🎨 [revealjs-skill](https://github.com/ryanbbrown/revealjs-skill): Coding agent skill for making Reveal.js presentations
- 🃏 [Web Deckbuilding](https://github.com/ryanbbrown/web-deckbuilding): Sandbox environment for deck-building games with support for live multiplayer
- 🪟 [LLM Overlay](https://github.com/ryanbbrown/llm-overlay): Always-on-top mini window for Claude, Gemini, and Perplexity on macOS
- 📸 [stylegen](https://github.com/ryanbbrown/stylegen): CLI for generating images with Gemini, supporting style references and parallel batch generation
- 💪 [LastLift](https://github.com/ryanbbrown/lastlift): iOS app for tracking workout consistency across exercise groups, built with SwiftUI and SwiftData
- 📬 [reader-notify](https://github.com/ryanbbrown/readwise-reader-feed-notifications): Cloudflare Worker that sends Pushover notifications for new Readwise Reader feed docs
- 📑 [Chrome Tab Groups Exporter](https://github.com/ryanbbrown/chrome-tab-groups-exporter): Chrome extension to export and import tab groups as JSON

## Latest Blog Posts
- [Thoughts on the AI bubble](https://blog.ryanbbrown.com/p/thoughts-on-the-ai-bubble)
- [AI will never master PowerPoint](https://blog.ryanbbrown.com/p/ai-will-never-master-powerpoint)
- [I reverse-engineered Kindle to build on-demand AI audiobooks](https://blog.ryanbbrown.com/p/i-reverse-engineered-kindle-to-build)
- [An LLM wiki won't change your life](https://blog.ryanbbrown.com/p/an-llm-wiki-wont-change-your-life)

## Other
- My [coding agent workflow](https://github.com/ryanbbrown/global-agent-context) is public and git-tracked. TLDR:
  - Agents write implementation plans for other agents; I review the durable behavior contract in `docs/behavior.md` when a project has product/workflow behavior worth preserving.
  - I use `cmux` to keep 6-9 isolated coding-agent workspaces open at once, one agent per workspace. In practice, only 3-5 are active priorities at any moment; the rest are queued, exploratory, or waiting for review. Addy Osmani's ["orchestration tax"](https://addyosmani.com/blog/orchestration-tax/) framing matches my experience: launching agents is cheap, but prioritizing, reviewing, and merging their work still bottlenecks on one human.
  - My [multi-review](https://github.com/ryanbbrown/global-agent-context/tree/main/plugins/personal/skills/multi-review) skill has Codex, Claude Code, and Factory Droid/DeepSeek review plans or implementations in parallel, then saves their feedback back into the repo.
  - New repos start with shared `CLAUDE.md`/`AGENTS.md` instructions, optional `docs/behavior.md`, local `learnings.jsonl` memory, and a promotion loop where only reviewed learnings graduate into project instructions.
  - I use my [interview](https://github.com/ryanbbrown/global-agent-context/tree/main/plugins/personal/skills/interview) skill before planning when my preferences need to be surfaced, HTML/diagram artifacts when visual explanation beats prose, and Matt Pocock's [architecture skill](https://github.com/mattpocock/skills/tree/main/skills/engineering/improve-codebase-architecture) for refactoring and simplification.
- I maintain a living set of things I believe in [OPINIONS.md](OPINIONS.md), inspired by [Kun Chen's post](https://blog.kunchenguid.com/p/everyone-should-have-an-opinionsmd).
- [ryanbbrown.com](https://ryanbbrown.com) is my personal hub, including a full list of [tools I use](https://ryanbbrown.com/tools/) and a tracked [book list](https://ryanbbrown.com/books/).

<!--
**ryanbbrown/ryanbbrown** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
