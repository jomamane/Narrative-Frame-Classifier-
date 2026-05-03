# Narrative Frame Classifier
### Saudi-UAE Information Operation — Appendix A
**Vinesight Home Assignment | Johanna Mamane | May 2026**

---

Live demo of an LLM-based narrative frame classifier applied to the Saudi-UAE information war that erupted on December 30, 2025.

**[→ Open the classifier](https://jomamane.github.io/vinesight-classifier)**

---

## What it does

Classifies Arabic and English social media posts by narrative frame using semantic LLM analysis — not keyword matching. Detects rhetorical intent regardless of surface phrasing, which is critical for Arabic-language discourse where indirect framing is culturally embedded.

**Frame taxonomy (derived from Section 3 of the report):**

| Code | Frame | Alignment |
|------|-------|-----------|
| F1 | Zionist Proxy | PRO_SAUDI |
| F2 | Regional Destabilizer | PRO_SAUDI |
| F3 | Accords Betrayal | PRO_SAUDI |
| F4 | Sovereignty Defense | PRO_UAE |
| F5 | Sacrifice Narrative | PRO_UAE |
| F6 | Boycott Mobilization | PRO_SAUDI |
| F7 | Neutral Reporting | NEUTRAL |
| F8 | Other | — |

**Output per post:** primary frame, confidence score, alignment (PRO_SAUDI / PRO_UAE / NEUTRAL), key signals, reasoning.

## Usage

1. Open the [live demo](https://jomamane.github.io/vinesight-classifier)
2. Enter your Anthropic API key (get one at [console.anthropic.com](https://console.anthropic.com))
3. Click **RUN ALL POSTS** or classify individual posts
4. Use the custom input to classify any Arabic or English post

Your API key is never stored — it lives in memory only and is sent directly to `api.anthropic.com`.

## Corpus

8 posts derived from documented rhetoric in open sources (see report footnotes). Arabic posts are representative reconstructions based on documented statements; English posts are paraphrases of documented content.

## Context

This tool is Appendix A of a narrative intelligence report analyzing the influence campaign that followed Saudi Arabia's December 30, 2025 airstrikes on a UAE-linked weapons shipment at the port of Mukalla, Yemen. Full methodology and sourcing in the main report.

---

*Model: claude-sonnet-4-6 | Languages: AR / EN | Framework: vanilla JS, no build step*
