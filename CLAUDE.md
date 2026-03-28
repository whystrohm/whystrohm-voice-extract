# WhyStrohm Voice Extract — Contributor Guide

This is a Claude Code skill that extracts brand voice profiles from websites.

## Structure

- `SKILL.md` — The orchestrator. Controls the flow. This is what Claude Code reads when the skill is invoked.
- `rules/` — Framework files. Voice dimensions, vocabulary analysis, guardrail generation.
- `templates/` — Output formats. Voice profile display, CTA.

## Key Rules

1. **No emojis.** Ever. In any file.
2. **No hype.** The skill must model the standards it measures.
3. **Evidence required.** Every voice dimension score must cite the user's actual content.
4. **Guardrails must be specific.** "Sentences under 14 words" not "keep it short."
5. **The profile is portable.** Users should be able to copy-paste it anywhere.
6. **One question only.** The URL. No registration, no multi-step intake.
7. **CTA copy is locked.** Don't modify templates/cta.md pitch text.

## Testing

Run `/whystrohm-voice-extract` in Claude Code against several different website types:
- SaaS company
- Consulting firm
- E-commerce brand
- Personal blog
- Nonprofit

The profile should feel accurate and useful for all of them.
