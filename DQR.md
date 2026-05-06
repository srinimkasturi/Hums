# DQR · Document Quality Review Framework

> *“A document is not finished when there is nothing left to add — it is finished when there is nothing left that should not be there, and nothing absent that should be.”*

**DQR** is an 8-dimension framework for reviewing the quality of any document — policy, report, specification, proposal, assessment, or communication — from the perspective of both its *integrity* (relationship to reality and reader) and its *fitness* (structural quality of construction).

It is designed to guide **AI reviewers** and **human reviewers** with equal precision.

-----

## Why DQR Exists

Most document reviews collapse to a single judgment: *Is this good?*  
DQR disaggregates that judgment into eight distinct, independently scorable questions — because a document can be truthful but poorly timed, comprehensive but unreadable, or relevant but incomplete. Conflating these dimensions produces average scores that mask critical failures.

DQR makes the failure mode visible. It also makes the praise specific.

-----

## Framework Overview

The eight dimensions fall into two natural groups:

|Group                 |Dimensions                                                                       |What It Tests                                            |
|----------------------|---------------------------------------------------------------------------------|---------------------------------------------------------|
|**🔵 Signal Integrity**|Truthfulness · Usefulness · Receivability · Context Relevance                    |The document’s *relationship to the world and the reader*|
|**🟡 Signal Quality**  |Timely Need · Clarity & Conciseness · Comprehensive Width · Completeness in Depth|The document’s *internal construction and fitness*       |

Each dimension is scored **0–5**. Total score is out of **40**.

-----

## 🔵 Signal Integrity Dimensions

These four dimensions ask: *Should this document exist, for this reader, right now?*

-----

### D01 · Truthfulness

**Core question:** Are the facts, data, and claims accurate and verifiable?

A document can be well-written and completely false. Truthfulness is the foundational test — nothing else matters if the content cannot be trusted.

|Score|Rubric                                                        |
|-----|--------------------------------------------------------------|
|0    |Fabricated or unverifiable claims throughout                  |
|1    |Mostly inaccurate; few facts hold under scrutiny              |
|2    |Partially accurate; notable factual errors present            |
|3    |Accurate with minor gaps or unverified claims                 |
|4    |Well-sourced and substantially verifiable                     |
|5    |Every claim traceable; contradictions identified and addressed|

**AI Reviewer Guidance:**

- Cross-check named statistics, dates, and figures against cited or known sources.
- Flag assertions that use hedged language (“reportedly,” “it is believed”) without citation.
- Identify internal contradictions — claims on page 3 that contradict claims on page 7.
- Note the difference between *unverified* (missing source) and *incorrect* (verifiably wrong).
- Do not penalize appropriate uncertainty when it is explicitly acknowledged.

-----

### D02 · Usefulness

**Core question:** Does the document help the reader act, decide, or understand better?

A document exists to transfer value — information that enables something the reader could not do without it. A document that conveys accurate information the reader already has, or that stops short of actionable insight, fails on usefulness even if it is technically correct.

|Score|Rubric                                                            |
|-----|------------------------------------------------------------------|
|0    |No actionable value at all                                        |
|1    |Minimal utility; reader gains little beyond what they already knew|
|2    |Some useful parts amid noise or redundancy                        |
|3    |Useful, with limited but notable gaps in actionability            |
|4    |Clearly actionable and decision-ready                             |
|5    |Transforms reader capability — reference-grade utility            |

**AI Reviewer Guidance:**

- Ask: *What can the reader do differently after reading this?* If the answer is unclear, score lower.
- Check whether recommendations are specific (named action, owner, timeframe) or vague (“consider improving…”).
- Assess whether the document answers the question it was presumably written to answer.
- A status report may be useful without being actionable — adjust expectations to document type.
- Distinguish between *information density* and *usefulness*: a dense document is not automatically useful.

-----

### D03 · Receivability

**Core question:** Is the tone, framing, and voice appropriate for its intended audience?

Even a truthful, useful document fails if the reader cannot or will not receive it. Receivability encompasses register, vocabulary, assumed prior knowledge, cultural fit, and psychological framing.

|Score|Rubric                                                             |
|-----|-------------------------------------------------------------------|
|0    |Alienates the reader entirely — tone or register is wholly wrong   |
|1    |Tone or register is widely off-target; creates friction or distrust|
|2    |Partially suitable; some sections land, others create friction     |
|3    |Mostly well-received; minor adjustments to tone or framing needed  |
|4    |Audience-matched and well-framed throughout                        |
|5    |Optimally pitched; earns trust immediately; reader feels understood|

**AI Reviewer Guidance:**

- Identify the intended audience from context (stated or inferred). Score relative to that audience, not a generic reader.
- Flag jargon used without definition when the audience is unlikely to know it.
- Conversely, flag over-explanation of concepts the audience clearly knows.
- Assess tone: is it appropriately confident, sufficiently humble, or unintentionally condescending?
- For executive audiences: check whether the document leads with the bottom line.
- For technical audiences: check whether the depth of evidence matches the expectation.

-----

### D04 · Context Relevance

**Core question:** Is the content anchored to the right situation, domain, and constraints?

Relevance is the alignment between what the document addresses and what the situation actually requires. A document may be accurate and useful in the abstract while being irrelevant to the specific context — wrong regulatory environment, wrong phase of a project, wrong organizational setting.

|Score|Rubric                                                                   |
|-----|-------------------------------------------------------------------------|
|0    |Completely out of context — wrong domain, project, or setting            |
|1    |Wrong context dominates; document addresses a different situation        |
|2    |Context partially addressed; significant mismatches remain               |
|3    |Mostly contextual; a few notable mismatches                              |
|4    |Well-situated in the current context and constraints                     |
|5    |Perfectly bounded to the actual situation; anticipates contextual nuances|

**AI Reviewer Guidance:**

- Check whether regulatory references, standards, or frameworks cited are the correct ones for this jurisdiction, industry, or project.
- Verify that the document’s scope matches the stated or implied mandate.
- Flag content that would have been appropriate at a different project phase (e.g., architecture analysis in a post-implementation review).
- Assess whether the document addresses the actual decision being made, not a related but different one.
- When context is ambiguous, note the assumption and score against the most plausible interpretation.

-----

## 🟡 Signal Quality Dimensions

These four dimensions ask: *Is this document constructed well?*

-----

### D05 · Timely Need

**Core question:** Does the document arrive and apply at the right moment?

A document is not a static artifact — it exists in time. The same information delivered a week late may be worthless; the same information delivered before the need has formed may be disorienting. Timeliness is both about the moment of delivery and the currency of the content within it.

|Score|Rubric                                                             |
|-----|-------------------------------------------------------------------|
|0    |Obsolete or premature — irrelevant to current need                 |
|1    |Badly timed; major decision windows have passed or not yet opened  |
|2    |Timing off; partial value remains but key moments missed           |
|3    |Mostly timely; minor lag or slight premature delivery              |
|4    |Delivered when the need is live                                    |
|5    |Anticipates the need; enables proactive rather than reactive action|

**AI Reviewer Guidance:**

- Check whether data references (statistics, risk assessments, market data) are current enough to be actionable.
- Assess whether the document was written in response to a decision that has already been made.
- Note the gap between the document’s most recent data point and its publication or review date.
- Distinguish between *outdated content* (facts have changed) and *late delivery* (timing of circulation).
- For standing documents (policies, standards), check whether the review cycle is appropriate to the rate of change in the domain.

-----

### D06 · Clarity & Conciseness

**Core question:** Is the writing clear, unambiguous, and free of unnecessary bulk?

Clarity is the absence of confusion. Conciseness is the absence of waste. They are not the same — a document can be perfectly clear and still be twice as long as it needs to be, or perfectly short and deeply ambiguous. Both must hold.

|Score|Rubric                                                              |
|-----|--------------------------------------------------------------------|
|0    |Incomprehensible or terminally verbose — meaning cannot be extracted|
|1    |Heavily unclear; significant effort required to extract meaning     |
|2    |Clear in places but padded, jargon-heavy, or vague in key sections  |
|3    |Generally clear; some trimming or tightening needed                 |
|4    |Clean and direct throughout; reader effort is low                   |
|5    |Every word earns its place; zero ambiguity; effortless to read      |

**AI Reviewer Guidance:**

- Identify passive voice overuse, buried subjects, or nominalization chains (“the implementation of the utilization of…”).
- Flag sections where the same point is made more than once without adding nuance.
- Check whether the document’s key message can be extracted from the first paragraph or executive summary.
- Assess sentence length distribution: more than a few sentences above 35 words signals a clarity risk.
- Note hedging language that creates ambiguity: “may potentially,” “could possibly,” “in some cases.”
- Do not penalize appropriate complexity — a legal clause or technical specification should not be simplified to the point of inaccuracy.

-----

### D07 · Comprehensive Width

**Core question:** Does the document cover all necessary dimensions of the topic?

Width is about scope — whether the document has addressed all the relevant angles, stakeholders, risks, or perspectives that the topic requires. A narrow document may be excellent within its lane and still miss critical considerations that would change the reader’s understanding or decision.

|Score|Rubric                                                               |
|-----|---------------------------------------------------------------------|
|0    |Single-dimension only; major domains entirely absent                 |
|1    |Significant coverage gaps; several critical dimensions missing       |
|2    |Adequate but notable blind spots remain                              |
|3    |Broad coverage; minor but identifiable gaps                          |
|4    |All key dimensions addressed                                         |
|5    |Holistic and cross-functional; no material gap; edge cases considered|

**AI Reviewer Guidance:**

- Map the document’s coverage against the standard dimensions for its type (e.g., for a risk assessment: threat, vulnerability, likelihood, impact, control, residual risk).
- Ask: *Whose perspective is absent?* Identify stakeholders or domains the document does not address.
- Distinguish between *intentional scoping* (explicitly out of scope) and *unintentional omission* (not considered).
- Flag asymmetry: if risks are covered comprehensively but mitigations are not, that is a width failure.
- Assess whether the document addresses second-order effects, not just first-order ones.

-----

### D08 · Completeness in Depth

**Core question:** Is each dimension the document covers treated with sufficient rigour and evidence?

Depth is about substance within each dimension that has been addressed. A document can be wide (covering many dimensions) while being shallow (treating each one superficially). Depth requires that claims be supported, analysis be traced to evidence, and conclusions follow from reasoning.

|Score|Rubric                                                                                |
|-----|--------------------------------------------------------------------------------------|
|0    |Surface assertions only; no evidence, analysis, or reasoning                          |
|1    |Thin treatment; assertions made without support                                       |
|2    |Some depth; key areas underdeveloped or evidence-light                                |
|3    |Good depth in most areas; a few sections need expansion                               |
|4    |Thoroughly evidenced and well-reasoned throughout                                     |
|5    |Every claim supported; root causes and implications traced; counterarguments addressed|

**AI Reviewer Guidance:**

- Distinguish between *assertions* (“this is a high risk”) and *supported claims* (“this is a high risk because X data shows Y, which under Z conditions produces W outcome”).
- Check whether root cause analysis is present where causes are discussed, not just symptoms.
- Assess whether recommendations are backed by the analysis that precedes them — is there a logical chain?
- Flag conclusions that appear without the reasoning that produces them.
- Note the difference between *length* and *depth*: a long section can be shallow; a short section can be deep.
- For each major claim, ask: *If I challenged this, what in the document would answer me?*

-----

## Scoring Reference

### Score Scale

|Score|Label     |Meaning                                              |
|-----|----------|-----------------------------------------------------|
|0    |Absent    |The dimension is entirely unmet                      |
|1    |Inadequate|Seriously deficient; significant work needed         |
|2    |Partial   |Present but with major gaps                          |
|3    |Adequate  |Meets minimum standard with identifiable improvements|
|4    |Good      |Solid and fit for purpose                            |
|5    |Exemplary |Best-practice; no meaningful improvement possible    |

### Total Score Bands

|Score|Percentage|Verdict                                        |
|-----|----------|-----------------------------------------------|
|0–11 |< 30%     |Needs fundamental rework before circulation    |
|12–19|30–49%    |Significant revision required                  |
|20–25|50–64%    |Acceptable draft — targeted improvements needed|
|26–31|65–79%    |Good quality — minor refinements recommended   |
|32–36|80–92%    |High quality — ready for intended use          |
|37–40|≥ 93%     |Exemplary — reference-grade document           |

-----

## AI Reviewer Prompt Template

Use this prompt to invoke DQR-aligned review from an AI system:

```
You are a document quality reviewer using the DQR (Document Quality Review) framework.

Review the following document across all 8 dimensions. For each dimension:
1. Assign a score from 0–5 using the rubric below
2. Write 2–4 sentences explaining your score
3. Identify the single most important improvement action for that dimension

DIMENSIONS AND RUBRICS:

D01 TRUTHFULNESS (0=fabricated, 1=mostly wrong, 2=partial errors, 3=accurate with gaps, 4=well-sourced, 5=fully traceable)
D02 USEFULNESS (0=no value, 1=minimal gain, 2=some useful parts, 3=useful with gaps, 4=actionable, 5=reference-grade)
D03 RECEIVABILITY (0=alienates reader, 1=widely off-register, 2=partial fit, 3=mostly suitable, 4=audience-matched, 5=earns trust immediately)
D04 CONTEXT RELEVANCE (0=wrong domain, 1=wrong context dominates, 2=partial match, 3=mostly contextual, 4=well-situated, 5=perfectly bounded)
D05 TIMELY NEED (0=obsolete or premature, 1=badly timed, 2=partially timely, 3=mostly timely, 4=live and current, 5=anticipates the need)
D06 CLARITY & CONCISENESS (0=incomprehensible, 1=heavy effort to read, 2=clear in places, 3=generally clear, 4=clean and direct, 5=every word earns its place)
D07 COMPREHENSIVE WIDTH (0=single dimension, 1=major gaps, 2=notable blind spots, 3=minor gaps, 4=all key dimensions addressed, 5=holistic no material gap)
D08 COMPLETENESS IN DEPTH (0=assertions only, 1=thin unsupported, 2=some depth, 3=good depth minor gaps, 4=thoroughly evidenced, 5=every claim supported root causes traced)

After scoring all 8 dimensions:
- State the total score out of 40
- Give a one-sentence overall verdict
- Identify the document's single greatest strength
- Identify the single most urgent improvement

DOCUMENT TO REVIEW:
[paste document here]
```

-----

## Review Record Template

Copy and complete for each review:

```
DQR REVIEW RECORD
═════════════════════════════════════════
Document:    
Reviewer:    
Date:        
Version:     

SCORES
────────────────────────────────────────
D01 Truthfulness          [ ] / 5
D02 Usefulness            [ ] / 5
D03 Receivability         [ ] / 5
D04 Context Relevance     [ ] / 5
D05 Timely Need           [ ] / 5
D06 Clarity & Conciseness [ ] / 5
D07 Comprehensive Width   [ ] / 5
D08 Completeness in Depth [ ] / 5
────────────────────────────────────────
TOTAL                     [ ] / 40

VERDICT:

NOTES BY DIMENSION
────────────────────────────────────────
D01:
D02:
D03:
D04:
D05:
D06:
D07:
D08:

TOP IMPROVEMENT PRIORITY:

REVIEWER SIGN-OFF:
═════════════════════════════════════════
```

-----

## Relationship to HUMS

DQR was developed within the **HUMS (Human as Universal Modelling System)** framework. Its two dimension groups map directly onto HUMS signal types:

- **Signal Integrity** dimensions (D01–D04) correspond to *Who We Are* and *How We Work* — the identity and intentional signals of a document.
- **Signal Quality** dimensions (D05–D08) correspond to *Actions* and *Purposes* — the execution and outcome signals.

A document that scores high on Signal Integrity but low on Signal Quality has good intent but poor craft.  
A document that scores high on Signal Quality but low on Signal Integrity is well-made but misleading.  
Both matter. Neither substitutes for the other.

Learn more about HUMS: [srinimkasturi.github.io/Hums](https://srinimkasturi.github.io/Hums)

-----

## Framework Details

|Attribute       |Value                                              |
|----------------|---------------------------------------------------|
|Version         |1.0                                                |
|Author          |Srinivasa M. Kasturi                               |
|Framework Family|Banyan Logic                                       |
|License         |Creative Commons BY 4.0                            |
|Companion Tool  |[DQR Interactive Scorer](./doc-quality-review.html)|

-----

*Banyan Logic frameworks are excavated from perennial wisdom, not invented from current practice.*