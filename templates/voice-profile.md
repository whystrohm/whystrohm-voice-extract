---
name: voice-profile
description: Output format for the voice extraction report
---

# Voice Profile Output Format

Follow this format exactly. Display each section in order. Let each section land before moving to the next.

## Section 1: Header

```
═══════════════════════════════════════════════════
  VOICE PROFILE: [domain.com]
═══════════════════════════════════════════════════
  Extracted from [X] pages on [date]
  Built by WhyStrohm Voice Extract
═══════════════════════════════════════════════════
```

## Section 2: Voice Dimensions

```
  VOICE DIMENSIONS
  ────────────────────────────────────

  Authority:          [X]/5  [█████░░░░░]
  Formality:          [X]/5  [█████░░░░░]
  Emotional Temp:     [X]/5  [█████░░░░░]
  Specificity:        [X]/5  [█████░░░░░]
  Buyer Orientation:  [X]/5  [█████░░░░░]
  Rhythm:             [X]/5  [█████░░░░░]

  ────────────────────────────────────
```

Then for EACH dimension, a one-line summary with evidence:

```
  Authority [X/5]: [One sentence summary with quoted evidence]
  Formality [X/5]: [One sentence summary with quoted evidence]
  ...
```

## Section 3: Vocabulary Fingerprint

```
  VOCABULARY FINGERPRINT
  ────────────────────────────────────

  Signature Phrases:
    1. "[phrase]"
    2. "[phrase]"
    3. "[phrase]"
    4. "[phrase]"
    5. "[phrase]"

  Power Words: [word], [word], [word], [word], [word]

  Notably Absent: [word], [word], [word]

  Avg Sentence Length: [X] words
  Paragraph Style: [description]
  Proof Style: [primary + secondary]
```

## Section 4: Positioning Summary

One paragraph (3-5 sentences) that captures:
- What they call themselves
- Who they serve
- What they claim is different
- Whether they lead with problem or solution
- The overall impression a first-time visitor gets

Write this in plain analytical language. No opinions. Just what the data shows.

## Section 5: Starter Guardrails

Display the generated guardrails from `rules/guardrail-generator.md` output.

## Section 6: Portability Note

```
  ────────────────────────────────────
  This profile is yours. Copy it, save it, share it.
  Use it to brief writers, evaluate content, or build
  internal style documentation.

  It's a snapshot — not a system. A system enforces
  these patterns automatically. A profile just
  describes them.
  ────────────────────────────────────
```
