# Hi, I'm Ryan 👋

> Shipping side projects at the intersection of AI, productivity, and my personal interests.

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/-SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Swift](https://img.shields.io/badge/-Swift-FA7343?style=flat-square&logo=swift&logoColor=white)

## Current Projects
- 🏆 [Retrodict](https://github.com/ryanbbrown/Retrodict): Highest-scoring ARC-AGI-3 agent — 99.86% RHAE, all 25 games solved, 5.5x fewer tokens
- 🔗 [ThinHarness](https://github.com/ryanbbrown/thinharness): A minimal, opinionated agent harness — focused scope, readable core, easy to fork
- ⚔️ [Deckfront](https://github.com/ryanbbrown/Deckfront) *(in progress)*: Building a digital board game that combines deck building and tactical skirmish
- 🧠 [OPINIONS.md Agent](https://github.com/ryanbbrown/opinions-agent): Agent that evolves my living beliefs file from my weekly reading highlights
- 📝 [Obsidian Drift](https://github.com/ryanbbrown/obsidian-drift): Native version control + accumulated IDE-like diff view for Obsidian (750+ downloads)
- 📚 [Kindle Storyteller](https://github.com/ryanbbrown/kindle-storyteller): iOS app for generating on-demand, live-syncing audiobook snippets using AI
- 🎨 [revealjs-skill](https://github.com/ryanbbrown/revealjs-skill): Coding agent skill for making Reveal.js presentations (300+ stars)
- 🚪 [AI Gate](https://github.com/inulute/ai-gate): Contributor to an Electron app for using ChatGPT, Claude, and Gemini in parallel, tmux-style workspaces
- 📸 [stylegen](https://github.com/ryanbbrown/stylegen): CLI for generating images with Gemini/GPT Image 2, supporting style references and parallel batch generation
- 💪 [LastLift](https://github.com/ryanbbrown/lastlift): iOS app for tracking workout consistency across exercise groups, built with SwiftUI and SwiftData
- 📬 [reader-notify](https://github.com/ryanbbrown/readwise-reader-feed-notifications): Cloudflare Worker that sends Pushover notifications for new Readwise Reader feed docs

<!--
- 🃏 [Web Deckbuilding](https://github.com/ryanbbrown/web-deckbuilding): Sandbox environment for deck-building games with support for live multiplayer
- 🪟 [LLM Overlay](https://github.com/ryanbbrown/llm-overlay): Always-on-top mini window for Claude, Gemini, and Perplexity on macOS
- 📑 [Chrome Tab Groups Exporter](https://github.com/ryanbbrown/chrome-tab-groups-exporter): Chrome extension to export and import tab groups as JSON
-->

## Writing

| Type | Title | Date |
| --- | --- | --- |
| Build | [how I accidentally got the top score on ARC-AGI-3 with 5.5x fewer tokens](https://blog.ryanbbrown.com/p/how-i-accidentally-got-the-top-score) | Jul 29, 2026 |
| Analysis | [An LLM wiki won't change your life](https://blog.ryanbbrown.com/p/an-llm-wiki-wont-change-your-life) | May 3, 2026 |
| Build | [I reverse-engineered Kindle to build on-demand AI audiobooks](https://blog.ryanbbrown.com/p/i-reverse-engineered-kindle-to-build) | Jan 25, 2026 |
| Analysis | [AI will never master PowerPoint](https://blog.ryanbbrown.com/p/ai-will-never-master-powerpoint) | Dec 16, 2025 |
| Analysis | [Thoughts on the AI bubble](https://blog.ryanbbrown.com/p/thoughts-on-the-ai-bubble) | Nov 13, 2025 |

## Coding

<details>
<summary>Setup</summary>

- Pi with gpt-5.6-sol on high is my daily driver, although I also use Claude Code with Fable 5 when sub capacity permits; full configuration and skills in my [dotfiles repo](https://github.com/ryanbbrown/dotfiles).
- I use bb to keep many projects open at once, with a few terminals per project. I also use bb's built-in Markdown editor for plans, documentation, and website content.
- The [first 3–10k lines of a greenfield project should usually be built while paired with a coding agent](https://blog.sshh.io/p/designing-software-for-software-factories#:~:text=If%20you%20are%20just%20starting%20a%20project%20(greenfield)%2C%20I%E2%80%99d%20build%20the%20first%203%2D10k%20LoC%20pairing%20with%20a%20coding%20agent%20and%20same%20with%20the%20first%20few%20E2E%20features); most of my side projects live in that phase and don't have a consistent stream of user feedback, so my setup is optimized for parallel in-the-loop work.

</details>

<details>
<summary>Agent Workflow</summary>

- First step is always to plan; the document is working context for the agent, not something I review line by line. I confirm the intended behavior, ask the agent to surface decisions it is uncertain about, and use HTML artifacts to understand when it's broad/complex.
- Once the plan is ready, the main agent delegates the work to a implementation subagent, runs my [review-panel](https://github.com/ryanbbrown/global-agent-context/tree/main/skills/review-panel) skill + script to get independent feedback from Codex / Claude Code / GLM, and sends synthesized fixes back to the same subagent.

</details>

<details>
<summary>Agent Tools</summary>

- Matt Pocock's [improve-codebase-architecture](https://github.com/mattpocock/skills/tree/main/skills/engineering/improve-codebase-architecture) skill to refactor and improve my codebases.
- [Exa](https://exa.ai/) for web search, [Context7](https://github.com/upstash/context7) MCP for current technical documentation, and [grep.app](https://grep.app/) MCP for real code examples from public GitHub repositories.
- `papercut` is a small bash CLI that lets agents log workflow friction to a shared file; I review the list periodically and fix recurring problems (inspired by [this tweet](https://x.com/steveruizok/status/2075303919664734295) from Steve Ruiz).

</details>

## Other
- I maintain a living set of things I believe in [OPINIONS.md](OPINIONS.md), inspired by [Kun Chen's post](https://blog.kunchenguid.com/p/everyone-should-have-an-opinionsmd).
- [ryanbbrown.com](https://ryanbbrown.com) is my personal hub, including a [board game log](https://ryanbbrown.com/gamelog/), a tracked [book list](https://ryanbbrown.com/books/), and the [tools I use](https://ryanbbrown.com/tools/).
