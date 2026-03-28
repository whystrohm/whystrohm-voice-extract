---
name: guardrail-generator
description: How to generate starter content guardrails from a voice profile
---

# Guardrail Generator

Based on the voice profile and vocabulary analysis, generate 15-20 specific, enforceable content rules. These are starter guardrails — the kind of rules that would be encoded into a full content infrastructure system.

## What Makes a Good Guardrail

**Good guardrail:** "Sentences must average under 14 words. No single sentence over 25 words."
**Bad guardrail:** "Keep sentences short."

**Good guardrail:** "Never use 'passionate,' 'excited,' 'thrilled,' or 'proud' in any content."
**Bad guardrail:** "Avoid hype words."

**Good guardrail:** "Every claim must have proof within 2 sentences — a number, timeframe, named outcome, or mechanism."
**Bad guardrail:** "Back up your claims."

Every guardrail must be:
- **Specific** — a person (or system) can check compliance in 5 seconds
- **Binary** — it either passes or fails, no judgment calls
- **Derived from the actual voice** — not generic best practices

## Categories

Generate guardrails in these categories:

### 1. Vocabulary Rules (3-5 rules)
Based on the vocabulary analysis:
- Words to always use (their power words)
- Words to never use (absent words that should stay absent, plus common hype words)
- Industry jargon rules (use? avoid? define on first use?)

### 2. Structure Rules (3-4 rules)
Based on sentence/paragraph patterns:
- Max sentence length
- Paragraph length limits
- Fragment usage (allowed or not)
- Question usage (allowed in headlines? body? never?)

### 3. Tone Rules (3-4 rules)
Based on voice dimensions:
- Authority level to maintain (e.g., "never hedge — no 'we think' or 'we believe'")
- Formality markers (contractions OK? slang OK?)
- Emotional boundaries (exclamation marks allowed? how many per piece?)

### 4. Proof Rules (2-3 rules)
Based on proof style:
- Claims-to-evidence ratio requirement
- Preferred proof type (numbers, mechanisms, stories)
- Unsubstantiated claim handling

### 5. Buyer Rules (2-3 rules)
Based on buyer orientation:
- "You" vs "we" ratio target
- Must the buyer's problem appear in the first X sentences?
- Can content lead with the company, or must it lead with the buyer?

## Output Format

```
STARTER GUARDRAILS
════════════════════════════════════

  Vocabulary
  ──────────
  1. [rule]
  2. [rule]
  3. [rule]

  Structure
  ──────────
  4. [rule]
  5. [rule]
  6. [rule]

  Tone
  ──────────
  7. [rule]
  8. [rule]
  9. [rule]

  Proof
  ──────────
  10. [rule]
  11. [rule]

  Buyer
  ──────────
  12. [rule]
  13. [rule]

  ...

════════════════════════════════════

These are starter guardrails — enough to catch the
biggest voice drift issues. A full system install
produces 40-60 rules calibrated to your specific
brand, enforced automatically.
```

## Important

- Guardrails must feel EARNED from the analysis, not generic.
- Reference specific evidence: "Your site uses short sentences (avg 9 words) — maintain this."
- If their voice is already strong in an area, say so and make the guardrail about protecting that strength.
- If their voice is weak in an area, make the guardrail about fixing the gap.
