---
# Claude Code skill entry-point
# Main logic lives in ../SKILL.md — this file adds Claude-specific bindings only.
name: mrna-cmc-web-search
description: >
  mRNA CMC 领域研究导向的源发现、验证、分类和打包工作流。
  覆盖 IVT 工艺、mRNA 原料药制备、靶向 LNP 递送系统、体内 CAR-T、
  分析方法开发、质量控制、CMC 和法规开发。
  仅用于网页源发现和证据包装，不用于内容写作。
  触发词：mRNA CMC 检索、LNP 配方溯源、IVT 工艺文献、体内 CAR-T 来源、
  分析方法查找、CMC 深度挖掘、会议监控、mRNA 制造来源、重复监控设置。
  Use when: user asks to search mRNA CMC sources, find LNP formulation references,
  look up IVT literature, scan conference abstracts for mRNA/RNA therapy,
  find analytical method papers, set up CMC monitoring.
model: claude-sonnet-4-6   # upgrade to claude-opus-4-7 for deep multi-step research
---

Follow the full skill definition in `../SKILL.md`.

## Claude Tool Mapping

| Workflow step | Preferred tool | Fallback |
|---------------|---------------|---------|
| PubMed search | `mcp__pubmed__search_articles` | `WebSearch("site:pubmed.ncbi.nlm.nih.gov ...")` |
| Full-text / page extract | `mcp__tavily__tavily_extract` | `WebFetch` |
| General web search (bioRxiv, patents, conferences) | `mcp__tavily__tavily_search` | `WebSearch` |
| ClinicalTrials.gov | `WebFetch("https://clinicaltrials.gov/api/v2/studies?query.term=...")` | — |
| Notion archiving (optional) | `mcp__notion__notion-create-pages` | — |

## Skill Handoff Rules

| User intent | Hand off to |
|-------------|------------|
| Write an article from found sources | `rnascript-wechat` |
| Format output as HTML | `wechat-article-html` |
| Publish to WeChat | `wechat-publisher` |
| End-to-end search → write → publish | `rnascript-pipeline` |
