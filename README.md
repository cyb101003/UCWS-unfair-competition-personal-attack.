# UCWS Singapore Hackathon 2026 — A Call for Transparency

*English · [中文版本](README.zh-CN.md) · [中英对照 Bilingual](README.bilingual.md)*

> A participant's documented account, with primary-source evidence, asking the
> organizers and the event's sponsor for transparent, itemized judging and a
> proper response to an apparent exposure of participants' personal data.

---

## 📂 Repository map

**Start here:** read the case below → review the [evidence index](evidence/README.md).
To add evidence, follow the [intake guide](evidence/INTAKE-GUIDE.md). To escalate, use
the letters in [`complaints/`](complaints).

| Path | What it is |
|---|---|
| [`README.md`](README.md) · [`README.zh-CN.md`](README.zh-CN.md) · [`README.bilingual.md`](README.bilingual.md) | The case for transparency — English · 中文 · side-by-side |
| [`evidence/`](evidence) | All exhibits, organized by concern (01–04) |
| [`evidence/README.md`](evidence/README.md) | Evidence index + redaction policy |
| [`evidence/INTAKE-GUIDE.md`](evidence/INTAKE-GUIDE.md) | How to add & sort screenshots safely |
| [`evidence/MANIFEST.md`](evidence/MANIFEST.md) | Caption + date for each exhibit |
| [`complaints/letter-to-miromind.md`](complaints/letter-to-miromind.md) | Draft letter to the sponsor (MiroMind) |
| [`complaints/pdpc-complaint.md`](complaints/pdpc-complaint.md) | PDPC / DPO data-breach templates |
| [`TIMELINE.md`](TIMELINE.md) | Dated sequence of events |
| [`SETUP.md`](SETUP.md) | How to publish & maintain this repo |

---

## What this repository is

This repository documents the first-hand experience and concerns of a participant
in the **UCWS Singapore Hackathon 2026**, an event publicly associated with sponsor
**MiroMind**. It collects the organizers' own published rules and public statements,
the announced results, and a description of an apparent personal-data exposure, and
it asks a set of specific, answerable questions.

The goal is narrow and constructive: **publish the itemized scoring data**, and
**acknowledge and properly remediate the data exposure**. If the organizers do
that, the central concerns here are resolved.

## What this repository is *not*

- **It is not a verdict.** Where this document states a fact, it links to evidence.
  Where it draws an inference or expresses an opinion, it says so explicitly.
- **It does not allege a crime.** Nothing here should be read as a finding that any
  person committed a criminal offence or a civil wrong. Those are determinations for
  the appropriate authorities, not for this page.
- **It does not name individual organizers,** and it does not target any individual
  personally. Concerns are directed at the **organizing committee** and the process.
- **It does not publish anyone's personal data.** All participant personal data has
  been redacted from every screenshot before it was added here (see
  [evidence/README.md](evidence/README.md)).

If anything in this repository is inaccurate, **please open an issue** — corrections
and retractions will be made promptly. Good faith and accuracy are the whole point.

---

## Background

The UCWS Singapore Hackathon 2026 published a **"Three-Dimensional Scoring
Mechanism"** in which the final score combines three components:

1. **AI evaluation**
2. **Community vote — stated as 30% of the total score**
3. **Judge scores**

A **Top-20 finalist list** was subsequently announced. The concerns below arise from
the relationship between the published rules, the announced results, and the
organizers' responses to questions about both.

---

## Concern 1 — Result transparency

**Documented facts (from the organizers' own materials and the public project wall):**

- The published rules state that the **community vote is worth 30%** of the total
  score. *(See [evidence/01-scoring-rules](evidence/01-scoring-rules).)*
- In the announced Top-20, the project listed at **No. 1** displayed, on the public
  project wall, **about 10 community votes and 0 GitHub stars** at the time of
  capture. *(See [evidence/02-rankings](evidence/02-rankings).)*
- Other projects on the same wall displayed **hundreds of community votes and, in
  some cases, 2,000+ GitHub stars.** *(See [evidence/02-rankings](evidence/02-rankings).)*
- When asked, in public, to explain the ranking against the published 30% rule, the
  organizers **declined to publish a score breakdown.** *(See
  [evidence/04-organizer-responses](evidence/04-organizer-responses).)*

**A fair acknowledgement.** Community vote is only 30% of the score. In principle a
project could rank highly on the strength of the AI-evaluation and judge components
(the other 70%) despite a low public vote count. **That is exactly why the itemized
breakdown matters:** with the per-component scores published, an unusual-looking
result is either explained or it isn't. Without them, neither participants nor the
sponsor can tell.

**This is not a complaint about the top-ranked team.** The team behind the
No. 1 project is not accused of anything here; they may well have earned strong AI
and judge scores. The question is directed at the **committee's transparency**, not
at any competitor.

**Open questions to the organizing committee:**

1. What were the per-component scores (AI evaluation, community vote, judge) for each
   finalist?
2. How was the 30% community-vote weight applied to a project with ~10 votes relative
   to projects with hundreds of votes?
3. Will the full, itemized scoring table be published for all projects?

---

## Concern 2 — Apparent exposure of participants' personal data

**Documented facts:**

- A backend endpoint of the form **`GET /api/teams?eventId=...`** returned data for
  participating teams **including plaintext email addresses and other personal
  fields**, reportedly covering **all 144 participating teams**. *(See
  [evidence/03-data-exposure](evidence/03-data-exposure) — all personal data redacted.)*
- After this was raised, an organizer publicly characterized the act of accessing the
  endpoint as **"malicious scraping,"** rather than acknowledging the exposure. *(See
  [evidence/04-organizer-responses](evidence/04-organizer-responses).)*

**Why this matters (factual context, not a legal conclusion).** Under Singapore's
**Personal Data Protection Act (PDPA)**, organizations must make reasonable security
arrangements to protect personal data in their control. A data breach is **notifiable
to the Personal Data Protection Commission (PDPC)** if it is likely to result in
**significant harm** to affected individuals, **or** if it affects **500 or more
individuals**; notification must be made within **3 calendar days** of assessing it as
notifiable. Even where the headcount is below 500, the **significant-harm** limb can
still apply (for example, exposed contact details that enable targeted phishing).
*(Sources at the bottom of this page.)*

**Important — responsible disclosure.** This repository **does not** republish the
exposed data. Doing so would itself harm the affected participants and would be the
very kind of disclosure the PDPA guards against. The evidence here shows only that the
exposure existed (endpoint shape, field names, counts), with every address and
personal field blacked out.

**Open questions to the organizing committee:**

1. Has the endpoint been secured, and from what date to what date was it accessible?
2. Have the affected participants been notified?
3. Has the PDPC been notified, and if not, on what basis was the breach assessed as
   non-notifiable?

---

## Concern 3 — Handling of questions and feedback

**Documented facts:**

- When participants asked, in the public channel, for an explanation of the ranking,
  the organizers asked to move the discussion to **"1v1 private calls"** and stated
  they **would not provide score breakdowns.** *(See
  [evidence/04-organizer-responses](evidence/04-organizer-responses).)*

**Why this matters (opinion).** A public competition with public rules and a public
vote invites public accountability. Routing every question into private channels,
while declining to publish the data that would settle the questions, is — in the
author's view — the opposite of the transparency the format promises. Reasonable
people can disagree; the remedy is simple and is the same in every case: **publish
the breakdown.**

**Open question:** Will the committee respond to these questions **on the record**,
in the same public channel where the rules and results were announced?

---

## What we are asking for

1. **Publish the full, itemized scoring table** — AI evaluation, community vote, and
   judge scores — for all finalists, ideally for all projects.
2. **Acknowledge and remediate the data exposure:** confirm it is fixed, notify
   affected participants, and confirm whether the PDPC was notified.
3. **Answer on the record,** in public, rather than only in private calls.

## A note to MiroMind (sponsor)

MiroMind's stated mission is reasoning that is **"not merely plausible, but
verifiable"** — AI that is **provably right** rather than merely appearing correct.
That is precisely the standard being requested of the event that carries MiroMind's
name: results that are **verifiable**, not merely asserted. A draft letter to
MiroMind is in [complaints/letter-to-miromind.md](complaints/letter-to-miromind.md).

---

## How to read the evidence

All exhibits are in [`evidence/`](evidence), organized by concern, with an index and a
strict redaction policy in [evidence/README.md](evidence/README.md). A chronological
account is in [TIMELINE.md](TIMELINE.md).

## Corrections

This is a good-faith account. If you are an organizer, sponsor, or participant and
believe something here is wrong or unfair, **open an issue**. Factual errors will be
corrected or retracted promptly, and your response can be linked here.

## Disclaimer

This repository reflects the documented experience and honest opinions of its author.
Statements of fact are supported by the linked evidence; characterizations and
inferences are the author's own opinions, offered in good faith on a matter of
legitimate concern to participants. Nothing here is a legal conclusion or an
allegation that any individual committed a criminal or civil wrong, and nothing here
is legal advice.

## Sources (public, third-party)

- PDPC — Report Your Organisation's Data Breach: https://www.pdpc.gov.sg/report-data-breach
- PDPC — Personal Data Protection Complaint: https://www.pdpc.gov.sg/complaints-and-reviews/report-a-personal-data-protection-concern/personal-data-protection-complaint
- PDPC — Guide on Managing and Notifying Data Breaches: https://www.pdpc.gov.sg/help-and-resources/2021/01/data-breach-management-guide
- MiroMind: https://www.miromind.ai/
