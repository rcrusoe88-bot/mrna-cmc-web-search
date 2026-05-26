---
name: mrna-cmc-web-search
description: Retrieve, verify, triage, and package high-credibility web source material on mRNA IVT, mRNA drug substance preparation, targeted LNP, mRNA-LNP formulation, in vivo CAR-T, in vivo cell engineering, analytical method development, quality control, manufacturing, and broader CMC topics. Use when Codex needs a research-only workflow for latest signal scanning, topic source packs, company or platform scans, conference monitoring, regulatory or technical guidance lookup, or recurring watch setups. Do not use this skill for drafting articles, writing outlines, or creating publication-ready copy.
---

# mRNA CMC Web Search

## Scope

Use this skill for web-based source discovery, verification, and evidence packaging only.

Focus on:

- mRNA IVT
- mRNA drug substance or bulk-solution preparation
- targeted LNP and lipid delivery systems
- mRNA-LNP drug product formulation
- in vivo CAR-T
- in vivo cell engineering
- analytical method development
- quality control, release testing, stability, and comparability
- CMC, process development, manufacturing, and regulatory development

Do not expand into content writing tasks. If the user also wants article drafting, treat that as a separate skill or a separate workflow.

## Request Types

Classify the request before searching.

1. Latest signal scan
   Use when the user wants the newest notable developments in a field slice.
2. Topic source pack
   Use when the user already has a topic and needs structured supporting material.
3. Company or platform scan
   Use when the user wants source material around a company, platform, raw material, excipient, process step, assay family, modality, or formulation route.
4. Conference monitoring
   Use when the user wants current signals from meetings, agendas, abstracts, posters, or sponsor disclosures.
5. CMC or manufacturing deep dive
   Use when the user wants process, analytical, quality, scale-up, release, stability, or regulatory CMC material.
6. Analytical or quality-method lookup
   Use when the user wants assay methods, impurity analysis, CQA discussion, sequence mapping, encapsulation metrics, or stability-indicating methods.
7. In vivo CAR-T or platform scan
   Use when the user wants source material around in vivo CAR-T programs, in vivo cell-engineering platforms, targeted immune-cell delivery, or adjacent translational signals.
8. Recurring watch setup
   Use when the user wants a durable monitoring list, cadence, or standing signal board.

## Source Priority

Use sources in this order unless the user asks otherwise.

1. Official conference portals, agendas, and abstract pages
2. Journal landing pages, DOI pages, and publisher pages
3. PubMed, FDA, EMA, NMPA, CDE, SEC, and company primary pages
4. Society or publisher news pages tied to the primary source
5. Reputable industry media only after locating the underlying primary source

If a secondary article cites a paper, abstract, company deck, filing, or regulator item, locate the original source before summarizing.

## Core Workflow

### 1. Frame the search

Extract the minimum set of search dimensions:

- modality
- platform or delivery approach
- process step, product stage, or assay family
- application or target when relevant
- angle: formulation, IVT, purification, analytical, quality, stability, manufacturing, regulatory, business
- timeframe: latest week, latest month, current year, conference season, or background

### 2. Choose references deliberately

Open only the reference file needed for the request.

- Use [references/source-map.md](./references/source-map.md) for official venues, journals, regulators, and company-source categories.
- Use [references/mrna-cmc-source-pack.md](./references/mrna-cmc-source-pack.md) when the topic is specifically about IVT, capping, purification, raw-material strategy, LNP formulation, analytical development, or RNA-focused CMC.
- Use [references/query-recipes.md](./references/query-recipes.md) when you need search-string formulas.
- Use [references/watchlist.md](./references/watchlist.md) when the user wants recurring monitoring or a stable watch routine.

### 3. Search with multiple phrasings

Always combine:

- one modality term
- one platform or delivery term
- one process-step, assay, or product-stage term
- one quality, CMC, or manufacturing term when relevant
- one date, year, or meeting constraint when the user wants the latest

Example dimensions:

- mRNA + IVT + dsRNA impurity + HPLC
- mRNA + capping efficiency + LC-MS
- LNP + targeted delivery + formulation + stability
- mRNA-LNP + release testing + encapsulation efficiency
- RNA manufacturing + comparability + scale-up
- "in vivo CAR-T" + LNP + T cell + autoimmune
- "in vivo cell engineering" + targeted delivery + manufacturing

### 4. Triage the results

Score each candidate source on:

- novelty
- credibility
- relevance
- specificity
- traceability

Prefer sources that include concrete details such as IVT conditions, capping route, purification method, lipid composition, formulation parameter, assay type, impurity profile, release criterion, stability condition, or regulatory expectation.

Discard items that are generic, duplicated, untraceable, or too weak to support a downstream research brief.

### 5. Package a research-ready output

Return a compact source pack. For each item, provide:

- title
- evidence type
- date in `YYYY-MM-DD`
- why it matters in one sentence
- confidence: high, medium, or low
- tags
- direct link

If useful, also add:

- search framing
- key unknowns
- follow-up verification actions
- monitoring suggestions

## Domain Heuristics

### mRNA drug substance and IVT workflow

Watch for terms such as:

- in vitro transcription
- IVT mRNA
- co-transcriptional capping
- post-transcriptional capping
- poly(A) tail engineering
- dsRNA impurity
- residual DNA template
- residual enzyme or NTP
- purification
- tangential flow filtration
- chromatography
- drug substance
- bulk solution

Track details that often matter:

- cap structure
- tail length
- sequence optimization
- modified nucleosides
- IVT yield
- impurity burden
- purification strategy
- concentration step
- filtration step
- storage condition

### Targeted LNP and mRNA-LNP formulation

Watch for terms such as:

- targeted LNP
- mRNA-LNP
- ionizable lipid
- helper lipid
- PEG-lipid
- ligand-targeted nanoparticle
- microfluidic mixing
- encapsulation efficiency
- particle size
- polydispersity
- zeta potential
- biodistribution
- formulation development

Track details that often matter:

- lipid composition
- N/P ratio or charge ratio
- mixing condition
- targeting ligand
- tissue or cell selectivity
- payload integrity
- potency linkage
- storage and freeze-thaw behavior
- container closure considerations

### In vivo CAR-T and in vivo cell engineering

Watch for terms such as:

- in vivo CAR-T
- in vivo cell engineering
- mRNA CAR delivery
- targeted immune-cell delivery
- T-cell targeted LNP
- gene delivery to T cells
- in situ immune-cell programming
- CAR expression in vivo
- autoimmune in vivo CAR-T

Track details that often matter:

- target antigen
- disease setting
- delivery route
- payload type
- cell selectivity
- persistence and durability
- safety signals
- manufacturability versus ex vivo CAR-T
- translational readiness

### CMC and process development

Watch for terms such as:

- process development
- analytical development
- comparability
- release testing
- raw material strategy
- closed system manufacturing
- scale-up or scale-out
- formulation and stability
- critical quality attributes
- process characterization
- tech transfer

When summarizing CMC material, make the bottleneck explicit:

- IVT yield
- impurity clearance
- batch consistency
- potency readout
- stability window
- sterility and contamination control
- assay transferability
- cost of goods

### Analytical and quality methods

Watch for terms such as:

- critical quality attributes
- identity assay
- purity assay
- dsRNA detection
- residual DNA
- residual protein
- capping efficiency
- poly(A) tail analysis
- sequence mapping
- particle characterization
- encapsulation assay
- potency assay
- stability-indicating method

Track whether the source includes:

- method principle
- sample preparation
- sensitivity or specificity
- orthogonal confirmation
- suitability for release or stability use
- comparability application

## Reliability Rules

- Do not present a claim as established if it comes only from a company press release or conference abstract.
- Label the evidence type explicitly: peer-reviewed article, review, conference abstract, company announcement, regulator notice, or news analysis.
- Use absolute dates, not only relative phrases.
- Separate `reported`, `demonstrated`, `planned`, `filed`, and `approved`.
- If the user asks for the latest developments, search live sources rather than relying on memory.
- When the same story appears in many places, cite the earliest and strongest primary source.

## Output Templates

### A. Latest signal scan

```markdown
## Search framing

- Scope:
- Timeframe:
- Priority angle:

## Source pack

| Date | Topic | Evidence type | Why it matters | Confidence | Tags | Link |
| --- | --- | --- | --- | --- | --- | --- |

## Gaps to verify

- Gap
- Gap

## Suggested next checks

- Check
- Check
```

### B. Topic source pack

```markdown
## Topic framing

- Core question:
- Why this topic matters:
- Included boundaries:
- Excluded boundaries:

## Source pack

1. Title
   Date:
   Evidence type:
   Key point:
   Why relevant:
   Confidence:
   Tags:
   Link:

## Open questions

- Question
- Question
```

### C. Conference monitoring

```markdown
## Meeting signal map

| Meeting | Release stage | Relevant session or abstract | Modality fit | Evidence strength | Follow-up action |
| --- | --- | --- | --- | --- | --- |
```

### D. Recurring watch setup

```markdown
## Monitoring scope

- Theme:
- Priority sources:
- Cadence:

## Watch table

| Source | Why watch it | What to look for | Cadence |
| --- | --- | --- | --- |

## Escalation rules

- Escalate when:
- Ignore when:
```

## Output Rules

- Default to Simplified Chinese unless the user asks otherwise.
- Keep the output concise, source-linked, and reusable for downstream analysis.
- Preserve official names, program codes, journal titles, assay names, and company names exactly as in the source.
- Prefer precise technical wording over promotional wording.
- If evidence is weak or early, say so plainly.
- Make clear whether the item is about drug substance, drug product, analytical method, manufacturing process, quality system, or regulatory guidance.
