# Draft letter to MiroMind

> Fill in the bracketed fields, attach the redacted evidence (or link this
> repository), and send. This version is written to be **factual, evidence-anchored,
> and measured** — it asks MiroMind to use its influence to obtain transparency,
> without asserting legal conclusions or naming individuals.

---

**To:** MiroMind — PR / Partnerships / Compliance
**From:** [Your name], participant — UCWS Singapore Hackathon 2026
**Date:** [Date]
**Subject:** Request for transparency at a MiroMind-sponsored event (UCWS Singapore Hackathon 2026)

Dear MiroMind Team,

I am a participant in the **UCWS Singapore Hackathon 2026**, an event publicly
associated with MiroMind as a sponsor. I am writing as someone who respects
MiroMind's work, because I believe the way this event has been run may reflect poorly
on the brand attached to it, and because the issues are straightforward to fix.

I want to be precise about what I am and am not saying. I am **not** asking you to
adjudicate anyone's guilt, and I am not making legal accusations. I am asking you, as
the sponsor whose name the event carries, to help obtain **transparency** that would
either resolve these concerns or substantiate them. Here are three documented
concerns, with evidence attached.

**1. The published results are hard to reconcile with the published rules.**
The committee's "Three-Dimensional Scoring Mechanism" states that the community vote
is **30%** of the total score. In the announced Top-20, the **No. 1** project
displayed, on the public project wall, roughly **10 community votes and 0 GitHub
stars**, while other projects displayed hundreds of votes and, in some cases, 2,000+
stars. This may be fully explainable by the AI-evaluation and judge components (the
other 70%) — but the committee has **declined to publish the per-component
breakdown** that would show this. With the itemized scores published, the result is
either explained or it isn't; without them, no one can tell. *(Evidence attached.)*

**2. An apparent exposure of participants' personal data.**
A backend endpoint of the form `GET /api/teams?eventId=...` reportedly returned
participants' **plaintext email addresses and other personal data**, covering all 144
participating teams. When this was raised, an organizer publicly described accessing
the endpoint as **"malicious scraping"** rather than acknowledging the exposure. Out
of respect for the affected participants, I have **not** reproduced any of the exposed
data; my evidence shows only the endpoint's structure with all values redacted. I have
separately reported, or intend to report, this to Singapore's **PDPC** through the
proper channel.

**3. Questions were routed to private channels instead of being answered publicly.**
When participants asked, in the public channel, for an explanation of the ranking, the
organizers asked to move to **"1v1 private calls"** and stated they would **not
provide score breakdowns**. *(Evidence attached.)*

**What I am asking of MiroMind.**
MiroMind's own mission emphasizes reasoning that is *verifiable* — results that are
provably right, not merely asserted. I am asking you to hold the event that carries
your name to that same standard:

1. Encourage the UCWS organizing committee to **publish the full, itemized scoring
   data** (AI evaluation, community vote, judge) for the finalists.
2. Ask them to **confirm the data exposure is remediated**, that affected
   participants have been notified, and whether the PDPC was notified.
3. Ask them to **respond publicly and on the record.**

I have compiled the evidence here: **[link to your public repository]**. I would
welcome the chance to share specifics with the right person on your team. If any part
of my account is mistaken, I will correct it readily.

Thank you for your time, and for caring about the integrity of the developer community.

Sincerely,
[Your name]
[Contact — email / GitHub handle]
[Optional: link to the repository]

---

*Attachments: redacted screenshots of (a) the official scoring rules, (b) the
announced ranking and public vote/star counts, (c) the data-exposure endpoint
structure, and (d) the organizers' public responses.*
