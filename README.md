# vault-system-explainer

The full interactive map of my personal AI infrastructure: every system audited against its real scripts, launchd logs and last-run timestamps, with the current state, the target end state (from the Vault Restructure Plan), and the gap between them.

Live at: https://izzyisotta.github.io/vault-system-explainer/

## What's on it

- **Map** — the four-layer target architecture (Capture → Process → Surface → Think/Act, plus Infrastructure), every system a clickable node with a status pill
- **System detail pages** — 17 systems, each with verified current state, end state, and a numbered A-to-B plan
- **Roadmap** — the Stage 0–5 build ladder plus a near-term punch list found by the audit
- **Skills** — all 35 slash skills with maturity ratings, filterable by system
- **Scripts & Jobs** — the 14 launchd jobs with last-run evidence, hooks, and called-out strays
- **Metadata & MOCs** — the proposed schema (current vs proposed), the 38 MOC pages, and what's blocking Stage 0
- **Freddie's Playbook** — his documented system components mapped against mine, with the ideas most worth copying next

## Structure

Single self-contained `index.html` (vanilla JS, no build step). System detail content lives in the `SYSTEMS` object at the bottom of the file; tables are static HTML. Hash routing: `#crm`, `#mail`, `#roadmap` etc. deep-link to a system or tab.

## Updating

Edit `index.html`, commit, push — GitHub Pages serves from `main`. The audit date in the hero and footer should be bumped whenever statuses are refreshed. Built and audited with Claude Code (full-system audit 2026-06-10); supersedes the late-May static explainer.
