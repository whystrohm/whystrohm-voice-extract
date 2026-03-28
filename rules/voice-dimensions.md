---
name: voice-dimensions
description: The 6 dimensions used to profile a brand's voice from website content
---

# Voice Dimensions

Score each dimension 1-5. Cite exact quotes from the scraped content as evidence.

## 1. Authority (1-5)

How much command does the voice carry?

| Score | Signal | Example Language |
|-------|--------|-----------------|
| 1 | Tentative | "We try to," "hopefully," "we think this might" |
| 2 | Cautious | "We believe," "in our experience," "we've found that" |
| 3 | Confident | "The pattern is clear," "this is what works," "here's what we know" |
| 4 | Expert | "The data shows," "after 200 implementations," "the research confirms" |
| 5 | Absolute | "This is the only way," "everything else is wrong," "non-negotiable" |

**Detection method:** Count hedge words (might, maybe, hopefully, try to, we think) vs. direct statements in the first 3 paragraphs of each page. Ratio determines score.

## 2. Formality (1-5)

How structured is the communication?

| Score | Signal | Detection |
|-------|--------|-----------|
| 1 | Casual | Slang, emojis, sentence fragments, rhetorical questions as structure |
| 2 | Conversational | Contractions, "you" heavy, approachable, short paragraphs |
| 3 | Professional | Clean prose, some contractions, no slang, industry terms used correctly |
| 4 | Formal | No contractions, structured paragraphs, third-person references |
| 5 | Academic | Dense, citation-heavy, passive voice dominant, jargon-heavy |

**Detection method:** Check for contractions (casual signal), passive voice (formal signal), average sentence length, paragraph length distribution.

## 3. Emotional Temperature (1-5)

How much feeling is in the writing?

| Score | Signal | Detection |
|-------|--------|-----------|
| 1 | Clinical | Data-only, no personality, reads like a spec sheet |
| 2 | Warm-Professional | Occasional human touch, mostly fact-driven |
| 3 | Engaging | Personality present, stories used, reader feels connection |
| 4 | Passionate | Strong opinions, exclamation points, emotional appeals |
| 5 | Hype | Urgency, FOMO, superlatives, emotional manipulation |

**Detection method:** Count exclamation marks, emotional adjectives (amazing, incredible, passionate), urgency words (now, today, don't miss), personal stories or anecdotes.

## 4. Specificity (1-5)

How concrete vs. abstract is the language?

| Score | Signal | Detection |
|-------|--------|-----------|
| 1 | Vague | "Solutions," "help businesses grow," "drive results" |
| 2 | General | Names the industry but not the problem |
| 3 | Targeted | Names the problem and the audience |
| 4 | Precise | Names the problem, audience, mechanism, and outcome |
| 5 | Surgical | Includes numbers, timeframes, named outcomes, proof |

**Detection method:** Count concrete nouns vs. abstract nouns. Count numbers and specific timeframes. Look for "how" explanations vs. "what" claims.

## 5. Buyer Orientation (1-5)

Who is the writing about?

| Score | Signal | Detection |
|-------|--------|-----------|
| 1 | Self-centered | 80%+ sentences about the company, "we" dominant |
| 2 | Mixed-self | More "we" than "you," features over benefits |
| 3 | Balanced | Roughly equal "we" and "you," mix of features and benefits |
| 4 | Buyer-focused | "You" dominant, problems named, benefits lead |
| 5 | Buyer-obsessed | Buyer's world described in detail, company barely mentioned |

**Detection method:** Count "we/our/us" vs. "you/your." Check whether headlines reference the buyer's problem or the company's capability.

## 6. Rhythm (1-5)

What's the sentence cadence?

| Score | Signal | Detection |
|-------|--------|-----------|
| 1 | Monotone | All sentences roughly same length, no variation |
| 2 | Mostly uniform | Slight variation, no intentional rhythm |
| 3 | Natural | Mix of short and medium sentences, readable flow |
| 4 | Dynamic | Intentional short punches mixed with longer explanation |
| 5 | Crafted | Clear rhetorical rhythm, fragments used for effect, pacing is a tool |

**Detection method:** Calculate sentence length variance. Look for one-word or two-word sentences (intentional rhythm). Check for parallel structure.

## Output Format

```
VOICE DIMENSIONS
════════════════════════════════════

  Authority:          [X]/5  [bar]
  Formality:          [X]/5  [bar]
  Emotional Temp:     [X]/5  [bar]
  Specificity:        [X]/5  [bar]
  Buyer Orientation:  [X]/5  [bar]
  Rhythm:             [X]/5  [bar]

════════════════════════════════════
```

For each dimension, include a one-line evidence quote from their actual content.
