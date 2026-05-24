# Personal AI Agent Orchestration

A pragmatic, skeptical guide to running AI coding agents as a solo developer — built as 21 standalone HTML pages you actually read instead of skim: 15 numbered chapters plus four field notes evaluating real-world setups.

**[→ Read the guide](https://YOUR_USERNAME.github.io/agent-orchestration-guide/)**

> Replace `YOUR_USERNAME` above with your GitHub username once Pages is live.

---

## What this is

Enough theory to make defensible choices, six concrete build steps for a real stack (GitHub Copilot · OpenCode · Claude Code · VS Code), and four worked examples that climb from a ten-minute bug fix to an overnight Ralph loop in a sandbox.

The through-line: **your repetition problem is a context-engineering problem, not an agent problem.** One good `AGENTS.md` solves more of it than five role-named "team-lead" or "architect" agents ever will. Build the boring markdown layer first; add agents only where you can name the bottleneck they remove.

## Contents

**Theory**
- `01` — Context rot & why fresh windows matter
- `02` — Context engineering: the operating system
- `03` — When orchestration helps — and when it hurts
- `04` — The four patterns worth knowing

**Build**
- `05` — Write your AGENTS.md
- `06` — Wire it into Copilot, OpenCode, Claude Code
- `07` — Build a reviewer agent with teeth
- `08` — Add explorer & docs-writer agents
- `09` — Git worktrees for parallel work
- `10` — Hooks, slash commands, auto-docs

**Examples**
- `11` — A 10-minute bug fix, the right way (simple)
- `12` — Ship a feature with TDD + review + docs (medium)
- `13` — Two features in parallel with worktrees (complex)
- `14` — A sandboxed Ralph loop overnight (advanced)

**Operate**
- `15` — Evals, failure modes, and a kill criterion

**Field notes** *(standalone evaluations, not part of the numbered sequence)*
- `eval-superpowers` — Evaluating [obra/superpowers](https://github.com/obra/superpowers): a skills-first methodology, when to adopt it, when to strip it to two ideas
- `eval-colleague` — Evaluating a colleague's OpenCode agents: an eleven-agent orchestrator-worker pipeline, file by file
- `skills-vs-agents` — The architectural fork: a skill informs one mind, an agent brings a fresh one. Pros, cons, and where each belongs
- `your-stack` — Build your own, best of both: full copy-able OpenCode config fusing all three approaches, with a week-by-week growth path

## Reading it

Start at `index.html` — it's the hub. Every chapter has a dropdown in the top-right that jumps to any other chapter and shows where you are, plus prev/next links at the bottom.

- **An hour?** Read `01`, do `05`, read `11`.
- **An afternoon?** Steps `05`–`07`, examples `11`–`12`, skim the theory.
- **A weekend?** Everything, in order — then set a 90-day reminder to run the kill criterion in `15`.
- **Evaluating someone else's setup?** Jump straight to the field notes — `skills-vs-agents` first for the concepts, then `your-stack` for a build you can copy.

## Running it locally

No build step. It's plain HTML, CSS, and a few lines of vanilla JS. Either:

```bash
# just open it
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows

# or serve it
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Hosting it on GitHub Pages

1. Push these files to the **root** of a public repo (keep them flat — the inter-page links are relative).
2. **Settings → Pages → Build and deployment → Deploy from a branch**, pick `main` / `/ (root)`, save.
3. Wait a minute, then visit `https://YOUR_USERNAME.github.io/agent-orchestration-guide/`.

## A note on sourcing

The guide draws on published engineering writing and papers — Anthropic's context-engineering and multi-agent posts, the "Lost in the Middle" and Chroma context-rot studies, the MAST failure taxonomy, Reflexion, and Geoffrey Huntley's Ralph writeups, among others. Sources are listed at the foot of each theory chapter. Treat the cost figures and tool specifics as a snapshot; models and pricing move.

## License

Personal/educational use. Adapt freely for your own setup.
