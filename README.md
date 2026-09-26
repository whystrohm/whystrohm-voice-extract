# WhyStrohm Voice Extract

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code Skill](https://img.shields.io/badge/Claude%20Code-Skill-7C3AED)](https://claude.ai/code)
[![whystrohm.com](https://img.shields.io/badge/WhyStrohm-whystrohm.com-00D4FF)](https://whystrohm.com)

**A free Claude Code skill that extracts a structured brand voice profile from any website. One URL in, a portable voice document out.**

Your website already has a voice. This skill quantifies it: 6 dimensions scored, vocabulary patterns mapped, positioning signals identified, and 15-20 starter guardrails generated. The output is yours to keep, share, and use anywhere.

---

## How It Works

| Step | What Happens |
|------|-------------|
| **1. Scrape** | Pulls your homepage, about page, and blog to analyze voice patterns |
| **2. Dimension** | Scores your voice across 6 measurable dimensions (each 1-5) |
| **3. Vocabulary** | Extracts signature phrases, power words, and notably absent language |
| **4. Position** | Maps what you call yourself, who you serve, and how you differentiate |
| **5. Guardrails** | Generates 15-20 specific, enforceable content rules based on YOUR voice |
| **6. Export** | Shows the profile and saves it as `brand/voice-profile.json`, which the voice scorer reads |

## The 6 Dimensions

| Dimension | What It Measures |
|-----------|-----------------|
| **Authority** | Tentative → Absolute. How much command does the voice carry? |
| **Formality** | Casual → Academic. How structured is the communication? |
| **Emotional Temperature** | Clinical → Hype. How much feeling is in the writing? |
| **Specificity** | Vague → Surgical. How concrete vs. abstract is the language? |
| **Buyer Orientation** | Self-centered → Buyer-obsessed. Who is the writing about? |
| **Rhythm** | Monotone → Crafted. What's the sentence cadence? |

---

## Install

**One command:**

```bash
git clone https://github.com/whystrohm/whystrohm-voice-extract.git ~/.claude/skills/whystrohm-voice-extract
```

**Or manually:** Download this repo and copy the `whystrohm-voice-extract/` folder to `~/.claude/skills/`.

### Requirements

- [Claude Code](https://claude.ai/code) (CLI, desktop app, or IDE extension)
- No API keys. No external tools. No configuration.

---

## Run

```
/whystrohm-voice-extract
```

You'll be asked for one thing: your website URL. That's it.

---

## What You'll See

Example output for a placeholder domain. The scores below are for illustration only.

```
═══════════════════════════════════════════════════
  VOICE PROFILE: yourcompany.com
═══════════════════════════════════════════════════

  VOICE DIMENSIONS
  ────────────────────────────────────

  Authority:          4/5  ████████░░
  Formality:          2/5  ████░░░░░░
  Emotional Temp:     3/5  ██████░░░░
  Specificity:        3/5  ██████░░░░
  Buyer Orientation:  4/5  ████████░░
  Rhythm:             3/5  ██████░░░░

  ────────────────────────────────────
```

Followed by:
- Per-dimension evidence with exact quotes from your site
- Signature phrases, power words, and notably absent vocabulary
- A positioning summary (what a first-time visitor sees)
- 15-20 starter guardrails derived from YOUR voice patterns
- A portable profile you can copy and use immediately

---

## What This Is (and Isn't)

**This is** a diagnostic tool. It tells you what your voice looks like, quantified. You can use the output to brief writers, evaluate content, or build internal documentation.

**This is not** a system. A profile describes your voice. A system enforces it. The difference: a profile gets ignored under deadline pressure. A system checks every piece for drift before it ships.

---

## File Structure

```
whystrohm-voice-extract/
├── SKILL.md                      # Orchestrator: controls the extraction flow
├── rules/
│   ├── voice-dimensions.md       # The 6-dimension scoring framework
│   ├── vocabulary-analysis.md    # Vocabulary fingerprint extraction
│   └── guardrail-generator.md    # How starter guardrails are derived
├── templates/
│   ├── voice-profile.md          # Output formatting
│   └── cta.md                    # Closing pitch
├── contracts/
│   └── voice-profile.v1.schema.json  # Format of brand/voice-profile.json (shared)
├── examples/
│   └── voice-profile.example.json    # Example profile, fictional brand
├── CLAUDE.md                     # Contributor guide for AI agents
├── .github/                      # Issue templates, PR template
├── CHANGELOG.md                  # Version history
├── CONTRIBUTING.md
├── SECURITY.md
├── LICENSE                       # MIT
└── README.md
```

---

## Want the Full System?

This skill extracts a voice profile. A full content infrastructure install turns that profile into a longer set of enforceable guardrails, a video production pipeline, and scheduled publishing across platforms. You own everything that gets built.

**Score your site:** [whystrohm.com/scan](https://whystrohm.com/scan?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop)
**See how the system is built:** [whystrohm.com/system](https://whystrohm.com/system?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop)

---

## Other WhyStrohm Skills

| Skill | What It Does | Install |
|-------|-------------|---------|
| [**Ritual**](https://github.com/whystrohm/ritual) **· NEW** | Scans your machine, ranks the top 5 recurring tasks worth scheduling, and drafts a Claude Code scheduled trigger that runs Voice Extract across your brands on a set cadence. | [Download `.skill` ↗](https://github.com/whystrohm/ritual/releases/latest) |
| [Digital Twin](https://github.com/whystrohm/digital-twin-of-yourself) | Reverse-engineer how you think and talk. Stress-tested AI System Prompt of yourself. | `git clone https://github.com/whystrohm/digital-twin-of-yourself.git ~/.claude/skills/digital-twin` |
| [Content Audit](https://github.com/whystrohm/whystrohm-audit) | Score your content against a 5-layer framework, get a live rewrite. | `git clone https://github.com/whystrohm/whystrohm-audit.git ~/.claude/skills/whystrohm-audit` |
| [Voice Scorer](https://github.com/whystrohm/whystrohm-voice-scorer) | Measure voice drift between your website and social content. | `git clone https://github.com/whystrohm/whystrohm-voice-scorer.git ~/.claude/skills/whystrohm-voice-scorer` |

## About WhyStrohm

[WhyStrohm](https://whystrohm.com) builds content infrastructure for founder-led companies. You own what gets built.

## Brand Infrastructure Consulting

This skill is one piece of the brand infrastructure I build for founder-led brands: voice extraction, programmatic video, and scheduled publishing. You own everything.

→ [whystrohm.com/system](https://whystrohm.com/system?utm_source=github&utm_medium=repo-cta&utm_campaign=2026-04-10-closed-loop)

## License

MIT. See [LICENSE](LICENSE).
