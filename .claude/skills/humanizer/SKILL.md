---
name: humanizer
description: Rewrite stiff, robotic, or AI-sounding text into natural, human-sounding prose while preserving the original meaning and facts. Use this whenever the user asks to "humanize," "make this sound more natural," "make this less AI-generated / less like ChatGPT," "loosen this up," or hands over a draft (site copy, an about/bio paragraph, an email, a blog post) that reads stilted, over-formal, or full of generic filler and wants it to sound like a real person wrote it. Also trigger proactively if the user pastes clearly AI-generated text and asks you to edit or "clean up" it without specifying how.
---

# Humanizer

Take text that reads like it came out of a language model — hedged,
over-structured, padded with throat-clearing — and rewrite it so it reads
like a specific person wrote it. The meaning, facts, and claims must not
change; only the voice does.

## Why this matters

"AI-sounding" text has a fairly recognizable signature: it over-explains,
hedges everything, reaches for the same handful of intensifiers and
transitions, and structures even short answers like a five-paragraph essay.
None of that makes the writing more correct — it just makes it sound like
nobody in particular wrote it. The fix isn't a thesaurus pass; it's noticing
which sentences exist only to sound thorough and cutting them, and letting
the remaining sentences vary in length and rhythm the way real writing does.

## What to actually change

Look for these patterns and cut or rework them:

- **Throat-clearing openers**: "In today's fast-paced world...", "It's
  important to note that...", "When it comes to X...". Just start with the
  point.
- **Reflexive hedging**: "can potentially," "may help to," "it could be
  argued that" stacked onto claims that don't need the hedge. Say the thing
  plainly if it's true; hedge only where the uncertainty is real.
- **Formulaic transitions and summaries**: "Moreover," "Furthermore,"
  "In conclusion," "Overall, it is clear that..." — these are essay
  scaffolding, not how people actually talk or write informally.
  Cut them; let ideas connect without a labeled transition, or use a plain
  "but," "so," "also."
- **Rule-of-three padding**: lists of exactly three adjectives/examples
  where one specific one would do ("innovative, efficient, and
  cutting-edge" → pick the one that's actually true).
  vague superlatives without evidence ("game-changing,"
  "cutting-edge," "seamless," "robust" used as filler rather than because
  they're precisely true).
- **Uniform sentence rhythm**: AI text tends toward medium-length sentences
  with similar structure back to back. Real writing varies — a short
  sentence after a long one, a fragment for emphasis, one idea per sentence
  instead of three clauses stitched with "which."
- **Over-structuring short content**: turning a two-sentence answer into a
  header + bulleted list. Match the format to the content's actual
  complexity, not to what looks maximally organized.

## What to leave alone

- **Facts, numbers, claims, and attributions** — don't soften, strengthen,
  or drop a claim while "improving the voice." If a sentence is factually
  imprecise, flag it rather than silently rewriting the meaning.
- **The user's actual voice, if you have samples of it.** If other text on
  this site (or text the user provides) shows their style — sentence
  length, formality, first-person habits, favorite turns of phrase — match
  that instead of defaulting to generic "casual blog voice." Check
  nearby content in the repo (e.g. other paragraphs on `about.md`,
  `index.md`) before inventing a voice from scratch.
- **Technical precision.** Don't trade accurate terminology for a
  folksier-sounding but vaguer word in technical or academic writing (this
  site includes research/teaching pages) — naturalness and precision aren't
  in tension; you can have both.

## Process

1. Read the passage once for meaning — know what it's actually claiming
   before touching the wording.
2. Check for existing voice samples nearby (same file, adjacent pages) to
   calibrate tone.
3. Rewrite sentence-by-sentence rhythm, not just word-by-word synonyms —
   swapping "utilize" for "use" alone doesn't fix an AI-sounding paragraph
   if the sentence structure underneath is still formulaic.
4. Read the result out loud (mentally) — if it sounds like something a
   person would actually say to a colleague, it's working; if it still
   sounds like a press release, cut more.
5. If asked, briefly note what kind of changes you made (e.g., "cut the
   intro throat-clearing, varied sentence length, removed a few hedges") —
   don't produce a line-by-line diff unless asked for one.
