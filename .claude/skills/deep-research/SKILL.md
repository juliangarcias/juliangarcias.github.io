---
name: deep-research
description: Conduct thorough, multi-source research on a topic and produce a synthesized, well-cited writeup. Use this whenever the user asks to research a topic in depth, investigate a question, look into a person/paper/organization/technology, fact-check a claim, prepare background for an academic page (research.md, teaching.md, a CV entry, a talk abstract), or wants a "deep dive," "literature review," or "state of the art" summary. Trigger even if the user just says "look into X" or "what's known about X" — don't wait for the word "research." Prefer this over a single quick search whenever the question has more than one plausible answer or the user's credibility depends on getting it right.
---

# Deep Research

Produce research that a careful person would trust enough to put their name
on — accurate, sourced, and honest about what's uncertain. The point isn't
to generate a lot of text; it's to reduce the user's uncertainty about a
real question using evidence they can check.

## Why this matters

A single search result or a single source read in isolation is often
misleading: it can be outdated, wrong, unrepresentative, or written by
someone with an axe to grind. The value of "deep" research is specifically
in triangulation — checking whether independent sources agree — and in
being explicit about confidence. Skipping that and writing confidently from
one source is the main failure mode to avoid.

## Process

1. **Clarify the actual question.** Restate it in one sentence before
   searching. If the request is ambiguous (e.g., "research this paper" could
   mean "summarize it" or "assess whether its claims hold up"), make a
   reasonable assumption and say so, rather than stalling on a clarifying
   question for something you can infer from context.

2. **Search broadly, then go deep on what matters.** Start with a few
   different queries/phrasings to map the landscape — don't anchor on the
   first result. Prefer primary sources (the paper itself, the original
   dataset, the org's own docs, primary reporting) over secondhand summaries
   when a primary source exists and is accessible. Use secondary sources
   (review articles, expert commentary, journalism) for context and for
   claims that are hard to verify directly.

3. **Corroborate, don't just accumulate.** For any claim that's central to
   the answer, actively check whether a second independent source agrees.
   If sources disagree, that disagreement is itself a finding — report it
   rather than silently picking the source that sounds most authoritative.

4. **Track provenance as you go.** For every source, note: what it is, who
   published it, when, and what specific claim you're drawing from it. This
   makes the final citations trivial and stops you from misattributing a
   claim later.

5. **Notice what you couldn't confirm.** If a claim shows up in only one
   low-quality source, or you ran out of time to verify something, say so
   explicitly rather than presenting it with the same confidence as
   well-corroborated facts. "I found this claimed in one source but
   couldn't independently confirm it" is a useful, honest sentence — use it.

## Output

Default structure (adapt as the question calls for it — a fact-check needs
less scaffolding than a literature review):

```markdown
## Summary
2-4 sentences answering the actual question, up front.

## Findings
The substantive content, organized by theme or sub-question rather than
by source. Cite inline as you go (see below).

## Open questions / uncertainty
What's contested, unconfirmed, or out of scope. Skip this section only
if there's genuinely nothing to flag.

## Sources
Numbered list, one entry per source actually cited, with enough
detail (author/org, title, date, URL) that the user could go verify it.
```

**Citations**: cite inline next to the specific claim it supports (e.g.,
"[1]"), not just in a bibliography at the end — a reader should be able to
tell which source backs which sentence. Never cite a source for a claim it
doesn't actually make; if you're synthesizing across sources, say so rather
than pinning the synthesis on one citation.

**Calibrate confidence in your language.** Match the phrasing to how solid
the evidence actually is: "X reports..." / "multiple sources confirm..." /
"it's widely believed but not verified that..." — don't flatten a shaky
claim and a well-established one into the same declarative tone.

## When writing for this site specifically

This repo is an academic personal site (`research.md`, `teaching.md`,
`about.md`). When the research feeds one of those pages, match the existing
tone in that file (concise, factual, first person where the site already
uses it) and keep citation formatting consistent with how other entries on
the page cite work — check the file before assuming a format.
