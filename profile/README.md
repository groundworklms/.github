<div align="center">

# Groundwork

### Grounded AI for training that cannot make things up.

**Grounded · Verified · Offline · Human-led**

Every claim cites the manual — or the system refuses. Answers are verified on-device against the
source, the delivery loop runs with the network pulled, and a human ratifies everything before it
reaches a learner.

</div>

---

## Why Groundwork

Most AI tutors will confidently invent an answer. In a schoolhouse — where the "answer" is doctrine
people are tested and evaluated on — that is unacceptable. Groundwork is built so it **can't**:

1. **Grounded** — every answer quotes the exact paragraph of the source, or it says "I don't know."
2. **Verified** — an on-device entailment check confirms the specifics are actually supported.
3. **Offline** — the delivery loop runs on a small edge device with no internet. $0 per answer.
4. **Human-led** — AI drafts; an instructor approves, edits, or rejects. Nothing unreviewed ships.

## The platform

**SchoolCircle** is the learning management app instructors and students use.
**Anchor** is the grounding engine that every answer flows through. The rest of the repos are
single-purpose services the app composes into two closed loops:

- **Instructor loop** — build a grounded course, review AI-drafted items, see class-wide gaps, improve.
- **Learner loop** — learn, ask a cited tutor, get calibrated by confidence-vs-correctness, master it.

## The repositories

| Repo | Role |
|---|---|
| [**anchor**](../../anchor) | The grounding engine — cite-or-refuse, on-device verification |
| [**quarry**](../../quarry) | Ingests source documents into searchable, cited passages |
| [**sourcerer**](../../sourcerer) | Resolves and formats citations (document, page) |
| [**coursewright**](../../coursewright) | Drafts course and lesson structure from doctrine |
| [**rubricon**](../../rubricon) | Turns standards into rubrics the AI is graded against |
| [**understudy**](../../understudy) | The tutor layer that answers learner questions via Anchor |
| [**whetstone**](../../whetstone) | Mastery & calibration — confidence vs. correctness |
| [**cadence**](../../cadence) | Spaced-repetition scheduling |
| [**waypoint**](../../waypoint) | Learner progress and pathing |
| [**sextant**](../../sextant) | Analytics — where a class is struggling |
| [**hotwash**](../../hotwash) | After-action review of a course's performance |
| [**cartridge**](../../cartridge) | Exports finished courses (SCORM / LTI) |

All repositories are standalone, tested, and Apache-2.0 licensed.

## Principles we don't bend

> Grounded, verified, offline, human-led. If a claim isn't in the source, the system refuses rather
> than guesses. That guarantee is the product.
