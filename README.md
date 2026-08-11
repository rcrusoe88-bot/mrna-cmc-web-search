# mRNA CMC Web Search

<p align="center">
  <img src="https://img.shields.io/github/stars/rcrusoe88-bot/mrna-cmc-web-search?style=flat-square" alt="Stars">
  <img src="https://img.shields.io/github/last-commit/rcrusoe88-bot/mrna-cmc-web-search?style=flat-square" alt="Last Commit">
  <img src="https://img.shields.io/github/repo-size/rcrusoe88-bot/mrna-cmc-web-search?style=flat-square" alt="Repo Size">
  <img src="https://img.shields.io/github/languages/top/rcrusoe88-bot/mrna-cmc-web-search?style=flat-square" alt="Top Language">
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=rcrusoe88-bot&repo=mrna-cmc-web-search&theme=vue&show_owner=true" alt="mrna-cmc-web-search 仓库数据">
</p>

`mrna-cmc-web-search` is a Codex skill for research-only source discovery, verification, triage, and packaging across:

- mRNA IVT
- mRNA drug substance or bulk-solution preparation
- targeted LNP and lipid delivery systems
- mRNA-LNP drug product formulation
- in vivo CAR-T
- in vivo cell engineering
- analytical method development
- quality control, release testing, stability, comparability, and broader CMC topics

This repository is designed for users who want a reusable web-search and source-packaging workflow, not a writing workflow.

## What This Skill Does

This skill helps Codex:

- scan latest field signals
- build topic-specific source packs
- monitor conferences and recurring watchlists
- look up regulatory or technical guidance
- trace claims back to primary sources
- package findings into research-ready outputs with evidence labels

It is intentionally scoped to research and source packaging. It does not handle article drafting, publication copy, or public-account writing.

## Research Scope

The skill covers both core mRNA CMC topics and adjacent translational search areas that often overlap with delivery and manufacturability questions:

- IVT process and productivity
- capping strategy
- purification and impurity clearance
- raw materials and manufacturing readiness
- targeted LNP and formulation development
- analytical and quality methods
- release, stability, and comparability
- in vivo CAR-T and in vivo cell engineering

## Repository Structure

```text
mrna-cmc-web-search/
|-- SKILL.md
|-- agents/
|   |-- openai.yaml
`-- references/
    |-- mrna-cmc-source-pack.md
    |-- query-recipes.md
    |-- source-map.md
    `-- watchlist.md
```

## Included Files

- `SKILL.md`
  The main skill definition, workflow, scope, heuristics, and output templates.

- `agents/openai.yaml`
  UI-facing metadata such as display name, short description, and default prompt.

- `references/source-map.md`
  A high-level map of journals, meetings, regulators, company-source categories, and discovery routes.

- `references/query-recipes.md`
  Reusable query patterns for latest-signal scans, conference scans, journal searches, CMC lookups, and topic shaping.

- `references/watchlist.md`
  A recurring monitoring framework for journals, meetings, regulators, companies, and workflow-specific mRNA CMC topics.

- `references/mrna-cmc-source-pack.md`
  A tighter source pack for IVT, purification, LNP formulation, analytics, in vivo CAR-T, and adjacent RNA CMC research.

## Installation

Copy this folder into your Codex skills directory.

Typical location:

```text
~/.codex/skills/mrna-cmc-web-search
```

If you use a custom `CODEX_HOME`, place it under:

```text
$CODEX_HOME/skills/mrna-cmc-web-search
```

## Example Usage

Example prompts:

- `Use $mrna-cmc-web-search to find the latest mRNA IVT analytical-method updates relevant to dsRNA impurity control.`
- `Use $mrna-cmc-web-search to build a source pack on targeted LNP formulation and stability methods.`
- `Use $mrna-cmc-web-search to scan recent in vivo CAR-T conference signals and package the strongest primary sources.`
- `Use $mrna-cmc-web-search to create a recurring watchlist for mRNA drug substance, LNP, and analytical CMC topics.`

## Design Principles

- Prefer primary sources over summaries.
- Treat recency as important.
- Use absolute dates when time matters.
- Label evidence strength and evidence type explicitly.
- Keep outputs concise, reusable, and research-ready.
- Separate source discovery from downstream writing workflows.

## Notes

- This repository contains the skill itself, not a standalone application.
- The skill is written to be modular: the main instructions stay in `SKILL.md`, while reusable research references live under `references/`.

---

## 📊 作者 GitHub 数据

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=rcrusoe88-bot&show_icons=true&theme=vue" alt="rcrusoe88-bot 的 GitHub 统计">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=rcrusoe88-bot&layout=compact&theme=vue" alt="rcrusoe88-bot 的常用语言">
</p>
