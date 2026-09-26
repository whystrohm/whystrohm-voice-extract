# Changelog

## [Unreleased]

## [1.1.0] - 2026-09-26

### Added
- Saves the profile as `brand/voice-profile.json` in the shared format in `contracts/voice-profile.v1.schema.json`. whystrohm-voice-scorer and whystrohm-audit read this file.
- `examples/voice-profile.example.json` shows a filled profile for a fictional brand.
- CI checks the schema and the example, and checks that the schema matches the canonical copy in whystrohm/shotkit.
- Social preview image and demo GIF.
- README and SKILL.md link to Digital Twin, Voice Scorer, Content Audit, and Ritual.

### Changed
- CTAs link straight to https://whystrohm.com/scan and https://whystrohm.com/system. README links carry UTM tags.
- The CTA and README point to whystrohm.com/scan and whystrohm.com/system for next steps.
- The README has one Other WhyStrohm Skills table.
- The PR template and issue templates name this skill's files and steps.
- The Voice Scorer cross-reference states which dimensions the two skills share.
- Copy uses short, plain statements. The sample profile is labelled as an example.

## [1.0.0] - 2026-03-28

### Added
- Initial release
- 6-dimension voice profiling (Authority, Formality, Emotional Temperature, Specificity, Buyer Orientation, Rhythm)
- Vocabulary fingerprint extraction (signature phrases, power words, absent language)
- Positioning signal mapping
- Starter guardrail generator (15-20 rules per profile)
- Portable output format
- MIT license
