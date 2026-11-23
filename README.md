<p align="center">
  <img src="assets/readme/hero.svg?v=2" alt="Rulebook for AI - The Agentic Engineering Standard" width="100%">
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT"></a>
  &nbsp;
  <a href="https://github.com/itsprem404/rulebook-for-ai"><img src="https://img.shields.io/badge/GitHub-itsprem404%2Frulebook--for--ai-181717.svg?logo=github" alt="GitHub Repository"></a>
  &nbsp;
  <a href="#quick-setup-for-developers"><img src="https://img.shields.io/badge/Agents-Universal%20Standard-emerald.svg" alt="Universal Standard"></a>
</p>

> **Stop AI coding agents from hand-rolling 1,200 lines of custom spaghetti when a 3-line harness exists, and leaving zombie scrap files in your repository.**

The **Agentic Engineering Standard** for developers using Claude Code, Cursor, Windsurf, Copilot, Antigravity, and autonomous AI agents.

---

## The Core Frustrations This Solves

If you build with AI coding agents, you have seen these daily failure modes:

1. **The "Mountain-Herb" Fallacy:** You ask for a feature (e.g., video clip detection, audio segmentation, search indexing), and instead of using proven open-source harnesses, the agent writes 500 lines of brittle custom mathematics from scratch.
2. **Spineless Apologies & Blind Sycophancy:** The agent praises terrible architecture ideas (*"Brilliant idea! Let's do that!"*). When you challenge it, it collapses into reflexive compliance (*"I apologize! You're completely right"*) instead of providing constructive technical pushback with real tradeoffs.
3. **The Ghost Connector Trap (Zombie Code):** You migrate from a legacy connector or auth provider (e.g., `zerino.py`) to a modern API. The new flow works, but the agent leaves the old files, dead imports, and obsolete secrets sitting in your repo as permanent junk.
4. **The Monolithic Bottleneck:** The agent tries to research docs, code backend APIs, author frontend UI, and run live browser tests in a single bloated turn, losing context and hallucinating requirements.
5. **Sequential Screenshot Amnesia:** You share a new screenshot to debug a mobile alignment bug, and the vision model gets trapped re-diagnosing errors from screenshots you solved 3 turns ago.

---

## Core Philosophy: Lego-Block Synthesis & Socratic Debate

> *"If you are sick, take the medicine already on the shelf. Never hike the mountain to pick raw herbs and compound medicine from scratch unless none exists."*

Most engineering problems do not require hand-rolling custom primitives. Proven open-source building blocks already solve 80% of foundational engineering challenges. 

`rulebook-for-ai` enforces 6 non-negotiable operational principles:

| Pillar | Problem Solved | Core Directive |
| :--- | :--- | :--- |
| **1. Socratic Sparring** | Sycophancy & spineless apologies | **Debate Path A vs Path B. Destination over vehicle. Defend sound logic.** |
| **2. Lego-Block Synthesis** | Reinventing wheels, custom code bloat | **Take medicine from the shelf. Compose 3-4 proven primitives as glue.** |
| **3. Active Scrap Audit** | Ghost files, post-migration junk | **Audit on pivot. Ask for permission before purging obsolete scrap.** |
| **4. Sub-Agent Delegation** | Monolithic context overload | **Divide multidisciplinary workflows across specialized roles.** |
| **5. Temporal Delta Focus** | Screenshot loops, stale context | **Treat latest input as active delta. Discard solved errors.** |
| **6. Surgical Execution** | Drive-by edits, untested code | **Touch only what is necessary. Loop with tests until verified.** |

---

## Real-World Case Studies

Check out **[EXAMPLES.md](./EXAMPLES.md)** for detailed side-by-side comparisons:
- **The Stream & Clip Detection Trap:** Hand-rolled custom FFT audio math vs. 30 lines of glue composing `auditok` + `whisper-timestamped`.
- **The Ghost Connector (`Zerino.py`):** Automatic deprecation audit detecting obsolete modules and prompting for clean disposal.
- **Socratic Architecture Debate:** Web scraping cron job vs. Reverse-engineered hidden API and distributed worker queues.
- **Debating Without Apologies:** Defending compute limits and synthesizing constraints with technical grounding.
- **Sequential Screenshot Debugging:** Isolating active CSS regressions without re-litigating solved runtime crashes.

---

## Quick Setup for Developers

Add `rulebook-for-ai` to your projects in under 30 seconds:

### 1. Claude Code (Marketplace Plugin)
Inside Claude Code:
```bash
/plugin marketplace add itsprem404/rulebook-for-ai
/plugin install rulebook-for-ai
```

### 2. Antigravity & Agent Runtimes
Install as a workspace plugin:
```bash
agy plugin install https://github.com/itsprem404/rulebook-for-ai.git
```
Then invoke anytime in chat via `@plugin:rulebook-for-ai` or `@skill:rulebook-for-ai`.

### 3. Cursor IDE
Save the rules directly into your Cursor rules folder:
```bash
mkdir -p .cursor/rules
curl -o .cursor/rules/rulebook-for-ai.mdc https://raw.githubusercontent.com/itsprem404/rulebook-for-ai/main/.cursor/rules/rulebook-for-ai.mdc
```

### 4. Direct Universal Setup (`AGENTS.md`)
Download the universal drop-in standard into your project root:
```bash
curl -o AGENTS.md https://raw.githubusercontent.com/itsprem404/rulebook-for-ai/main/AGENTS.md
```
*(Compatible with Claude Code, Cursor, Windsurf, Copilot Workspace, Antigravity, and Cline)*

---

## Repository Structure

```
rulebook-for-ai/
├── .claude-plugin/
│   ├── marketplace.json               # Claude Code marketplace registry
│   └── plugin.json                    # Claude Code plugin manifest
├── .cursor/
│   └── rules/
│       └── rulebook-for-ai.mdc        # Cursor IDE rulebook configuration
├── assets/
│   └── readme/
│       └── hero.svg                   # Animated README hero banner
├── rules/
│   └── AGENTS.md                      # Auto-enforced background agent rules
├── skills/
│   └── rulebook-for-ai/
│       └── SKILL.md                   # Callable skill (@skill:rulebook-for-ai)
├── AGENTS.md                          # Universal agent guidelines (drop-in)
├── CLAUDE.md                          # Claude Code workspace standard
├── EXAMPLES.md                        # Anti-patterns vs industry best practices
├── LICENSE                            # MIT open-source license
├── plugin.json                        # Universal plugin manifest
└── README.md                          # Official repository documentation
```

---

## License

This project is licensed under the [MIT License](./LICENSE). Contributions and discussions are welcome via GitHub issues and pull requests.
