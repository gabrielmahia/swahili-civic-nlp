# swahili-civic-nlp

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![DPGA](https://img.shields.io/badge/DPGA-GID0093743-green)](https://digitalpublicgoods.net)
[![HuggingFace](https://img.shields.io/badge/🤗-Dataset-yellow)](https://huggingface.co/datasets/gmahia/swahili-civic-nlp)

**Swahili civic NLP datasets and tools for East Africa AI coordination infrastructure.**


## The Data Gap This Addresses

**AfricaNLP 2025/2026 findings:**
- Only **4 African languages** receive consistent NLP research attention: Amharic,
  Swahili, Afrikaans, Malagasy
- **98%+ of African languages** have no meaningful AI coverage (Hussen et al., 2026,
  arXiv:2506.02280)
- Swahili is one of the 4 supported — but civic and legal Swahili is severely
  underrepresented even within Swahili NLP corpora
- AfricaNLP 2025 identifies healthcare, civic, and legal as the domains with the
  most critical accuracy and trust requirements — and the most data gaps

**What this dataset provides:**
Constitutional rights, government service descriptions, M-PESA terms, and
civic process explanations in Swahili — the domain-specific civic language
that general Swahili corpora do not cover.

**Why it matters:**
AI systems deployed in civic contexts (rights information, service navigation,
accountability) that hallucinate or mistranslate cause measurable harm. Domain-
specific grounding in verified civic Swahili is a prerequisite for safe deployment.


Part of the [AI-KungFU Nairobi Stack](https://github.com/gabrielmahia/nairobi-stack) —
the largest open-source MCP coordination infrastructure for the Global South.

## What This Is

NLP resources for Swahili civic language, including:
- Intent detection for civic queries (health, land, education, government)
- Sentiment analysis on civic text
- Named entity recognition for Kenyan civic context
- M-PESA, health, education, and government domain vocabulary
- KCSE/KCPE education terminology
- County government terminology for all 47 counties

## Dataset

The dataset is published on HuggingFace:
- **[gmahia/swahili-civic-nlp](https://huggingface.co/datasets/gmahia/swahili-civic-nlp)**
- Available on HuggingFace and PyPI
- License: CC BY 4.0

## Why Swahili NLP Matters

> Swahili AI fails at 4× the rate of English on civic tasks.

Most open NLP benchmarks are English-first. Swahili has 200M+ speakers across East and
Central Africa but is severely underrepresented in civic-domain training data.

This dataset addresses that gap: civic terminology that actually appears in government
documents, health worker guidance, and community coordination contexts.

## Data Sovereignty

All data in this collection is designed for local-first deployment:
- Process with [offline-mcp](https://github.com/gabrielmahia/offline-mcp) (no API key)
- Run via [SII Stack](https://github.com/gabrielmahia/sii-stack) sovereign inference tier
- No community data transmitted to foreign servers

## Digital Public Good

This project is submitted to the [DPGA](https://digitalpublicgoods.net) as a Digital Public Good (GID0093743).

## Related Projects

- [tafsiri-mcp](https://github.com/gabrielmahia/tafsiri-mcp) — Swahili translation MCP server
- [civic-agent-kit](https://github.com/gabrielmahia/civic-agent-kit) — unified SDK
- [nairobi-stack](https://github.com/gabrielmahia/nairobi-stack) — full portfolio

## License

MIT © 2024-2026 Gabriel Mahia (AI-KungFU)

## Part of the East Africa Coordination Stack

This MCP server is one of 32 tools in the Kenya coordination infrastructure.
Connect it to [`africa-coord-bus`](https://github.com/gabrielmahia/africa-coord-bus) —
the coordination event bus that routes signals between domains automatically.

```bash
pip install africa-coord-bus
```

All 32 servers: [pypi.org/user/gmahia](https://pypi.org/user/gmahia/)
Live demo: [coord-cascade-demo](https://github.com/gabrielmahia/coord-cascade-demo)