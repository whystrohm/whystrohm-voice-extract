# Changelog

## [Unreleased]

### Added
- The profile is saved as `brand/voice-profile.json`, in the shared format in `contracts/voice-profile.v1.schema.json`. whystrohm-voice-scorer reads it.
- `examples/voice-profile.example.json`, a filled profile for a fictional brand.
- CI checks the schema, the example, and that the schema matches the canonical copy in whystrohm/shotkit.
- Social preview image and demo GIF.
- README and SKILL.md links to Digital Twin, Voice Scorer, Content Audit, and Ritual.

### Changed
- CTAs point straight at https://whystrohm.com/scan and https://whystrohm.com/system, with UTM tags in the README.
- CTA and README no longer state prices or a pricing model.
- README keeps one Other WhyStrohm Skills table.
- PR template and issue templates now name this skill's files and steps.
- Voice Scorer cross-reference states which dimensions the two skills share.
- Copy pass: no speed claims, no em dashes. The sample profile is labelled as an example.

## [1.0.0] - 2026-03-28

### Added
- Initial release
- 6-dimension voice profiling (Authority, Formality, Emotional Temperature, Specificity, Buyer Orientation, Rhythm)
- Vocabulary fingerprint extraction (signature phrases, power words, absent language)
- Positioning signal mapping
- Starter guardrail generator (15-20 rules per profile)
- Portable output format
- MIT license
