# DQR · Document Quality Review Framework

**Version:** 1.1-simple | **Author:** Srinivasa M. Kasturi | **Family:** Banyan Logic

DQR reviews any document across 8 dimensions scored 0–5 each (total out of 40). Four dimensions test the document’s relationship to the world and reader (Signal Integrity). Four test its internal construction (Signal Quality).

-----

## HOW TO SCORE

Each dimension uses the same scale:
0 = entirely absent or failed · 1 = seriously deficient · 2 = partial, major gaps · 3 = adequate, improvable · 4 = good, fit for purpose · 5 = exemplary, nothing to add

Total score bands:
0–11 = needs fundamental rework · 12–19 = significant revision needed · 20–25 = acceptable draft · 26–31 = good quality · 32–36 = high quality · 37–40 = exemplary

-----

## THE 8 DIMENSIONS

### SIGNAL INTEGRITY (asks: should this document exist, for this reader, right now?)

**D01 · Truthfulness** — Are the facts, data, and claims accurate and verifiable?
Score 0 if claims are fabricated. Score 1 if mostly inaccurate. Score 2 if partially accurate with notable errors. Score 3 if accurate with minor gaps or unverified claims. Score 4 if well-sourced and substantially verifiable. Score 5 if every claim is traceable and contradictions are addressed.
Key check: flag assertions without sources; flag internal contradictions; do not penalise acknowledged uncertainty.

**D02 · Usefulness** — Does the document help the reader act, decide, or understand better?
Score 0 if no actionable value. Score 1 if reader gains little beyond what they already knew. Score 2 if some useful parts exist amid noise. Score 3 if useful but with limited gaps in actionability. Score 4 if clearly actionable and decision-ready. Score 5 if it transforms reader capability.
Key check: ask what the reader can do differently after reading; verify recommendations are specific, not vague.

**D03 · Receivability** — Is the tone, framing, and voice right for its intended audience?
Score 0 if the reader is alienated entirely. Score 1 if tone is widely off-target. Score 2 if partially suitable. Score 3 if mostly well-received with minor adjustments needed. Score 4 if audience-matched throughout. Score 5 if it earns trust immediately.
Key check: identify the intended audience first; flag unexplained jargon or condescending over-explanation.

**D04 · Context Relevance** — Is the content anchored to the right situation and constraints?
Score 0 if completely out of context. Score 1 if the wrong context dominates. Score 2 if partially matched. Score 3 if mostly contextual with a few mismatches. Score 4 if well-situated in the current context. Score 5 if perfectly bounded and anticipating contextual nuances.
Key check: verify the document addresses the actual decision being made, not a related but different one.

-----

### SIGNAL QUALITY (asks: is this document constructed well?)

**D05 · Timely Need** — Does the document arrive and apply at the right moment?
Score 0 if obsolete or premature. Score 1 if badly timed and key decision windows have passed. Score 2 if timing is off but partial value remains. Score 3 if mostly timely with minor lag. Score 4 if delivered when the need is live. Score 5 if it anticipates the need and enables proactive action.
Key check: check whether the data references are current enough to be actionable.

**D06 · Clarity and Conciseness** — Is the writing clear, unambiguous, and free of unnecessary bulk?
Score 0 if incomprehensible or terminally verbose. Score 1 if significant effort is needed to extract meaning. Score 2 if clear in places but padded or jargon-heavy. Score 3 if generally clear with some tightening needed. Score 4 if clean and direct throughout. Score 5 if every word earns its place with zero ambiguity.
Key check: check whether the key message can be extracted from the first paragraph; note hedging language like “may potentially” or “could possibly.”

**D07 · Comprehensive Width** — Does the document cover all necessary dimensions of the topic?
Score 0 if only a single dimension is addressed. Score 1 if several critical dimensions are missing. Score 2 if adequate but with notable blind spots. Score 3 if broad with minor gaps. Score 4 if all key dimensions are addressed. Score 5 if holistic with no material gap and edge cases considered.
Key check: ask whose perspective is absent; distinguish intentional scoping from unintentional omission.

**D08 · Completeness in Depth** — Is each dimension treated with sufficient rigour and evidence?
Score 0 if only surface assertions with no evidence. Score 1 if assertions are made without support. Score 2 if some depth exists but key areas are underdeveloped. Score 3 if good depth with a few sections needing expansion. Score 4 if thoroughly evidenced and well-reasoned. Score 5 if every claim is supported and root causes and counterarguments are addressed.
Key check: distinguish assertions (“this is a high risk”) from supported claims (“this is a high risk because X data shows Y”); note that length is not the same as depth.

-----

## REVIEW PROMPT (copy and use with any AI)

```
You are a document quality reviewer using the DQR framework. Review the document below across all 8 dimensions. For each dimension, assign a score from 0 to 5, write 2 to 3 sentences explaining your score, and name the single most important improvement for that dimension. Then give the total score out of 40, a one-sentence overall verdict, the document's single greatest strength, and the single most urgent improvement.

SCORING SCALE FOR ALL DIMENSIONS:
0 = entirely absent or failed
1 = seriously deficient
2 = partial, major gaps
3 = adequate, could be improved
4 = good, fit for purpose
5 = exemplary

THE 8 DIMENSIONS:
D01 Truthfulness: are facts and claims accurate and verifiable?
D02 Usefulness: does the document help the reader act, decide, or understand better?
D03 Receivability: is the tone and framing right for the intended audience?
D04 Context Relevance: is the content anchored to the right situation and constraints?
D05 Timely Need: does the document arrive and apply at the right moment?
D06 Clarity and Conciseness: is the writing clear and free of unnecessary bulk?
D07 Comprehensive Width: does the document cover all necessary dimensions of the topic?
D08 Completeness in Depth: is each dimension treated with sufficient rigour and evidence?

DOCUMENT TO REVIEW:
[paste document here]
```

-----

## SCORE RECORD (copy and complete)

```
DQR REVIEW RECORD
Document:
Reviewer:
Date:

D01 Truthfulness          /5
D02 Usefulness            /5
D03 Receivability         /5
D04 Context Relevance     /5
D05 Timely Need           /5
D06 Clarity Conciseness   /5
D07 Comprehensive Width   /5
D08 Completeness Depth    /5
TOTAL                     /40

VERDICT:
GREATEST STRENGTH:
MOST URGENT IMPROVEMENT:
```

-----

## RELATIONSHIP TO HUMS

DQR is part of the HUMS (Human as Universal Modelling System) framework. Signal Integrity dimensions (D01–D04) map to identity and intentional signals. Signal Quality dimensions (D05–D08) map to execution and outcome signals. A document that scores high on Integrity but low on Quality has good intent but poor craft. A document that scores high on Quality but low on Integrity is well-made but misleading.

More at srinimkasturi.github.io/Hums

-----

*Banyan Logic frameworks are excavated from perennial wisdom, not invented from current practice.*