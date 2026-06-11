# Reporting the data exposure to Singapore's PDPC

> This is a template and a step-by-step guide. It is **not legal advice.** Fill in the
> bracketed fields. The PDPC generally expects you to **contact the organization's
> Data Protection Officer (DPO) first**, then escalate to the PDPC if there is no
> adequate response.

## How the process works (per PDPC guidance)

1. **Contact the organization's DPO first.** The DPO's contact details are usually in
   the organization's privacy policy; if you can't find them, the PDPC has a "DPO
   enquiry" form. Use the **Step 1 letter** below.
2. **Wait for a response.** PDPC guidance indicates that if you **do not hear back
   within 10 business days**, you may escalate to the PDPC.
3. **File with the PDPC.** Submit a complaint via the PDPC e-service (you will need a
   **Singpass** login). Use the **Step 2** notes below to prepare what you'll submit.

> Note on the organization's *own* duty: under the PDPA's data-breach regime, an
> organization must notify the PDPC if a breach is **likely to cause significant harm**
> to affected individuals **or** affects **500 or more individuals**, within **3
> calendar days** of assessing it as notifiable. Whether this particular exposure was
> "notifiable" is for the PDPC to assess — your report gives them the facts to do so.

Links:
- Report a data breach / concern: https://www.pdpc.gov.sg/report-data-breach
- Personal Data Protection Complaint: https://www.pdpc.gov.sg/complaints-and-reviews/report-a-personal-data-protection-concern/personal-data-protection-complaint
- Data Breach Management Guide: https://www.pdpc.gov.sg/help-and-resources/2021/01/data-breach-management-guide

---

## Step 1 — Letter to the organization's DPO

**To:** [Organizer / company name], Data Protection Officer
**From:** [Your name], participant — UCWS Singapore Hackathon 2026
**Date:** [Date]
**Subject:** Personal data exposure — request for information and remediation under the PDPA

Dear Data Protection Officer,

I participated in the UCWS Singapore Hackathon 2026. I am writing to raise what
appears to be an exposure of participants' personal data and to ask how it is being
handled.

On or around **[date]**, a backend endpoint of the form `GET /api/teams?eventId=...`
returned participating teams' personal data, **including plaintext email addresses**,
appearing to cover all **144** participating teams. I have not retained or distributed
the underlying data.

Under the PDPA's Protection Obligation, I would be grateful for written answers to:

1. Has the endpoint been secured, and for what period was the data accessible?
2. What categories of personal data were exposed, and how many individuals are affected?
3. Have affected participants been notified, and has the PDPC been notified? If the
   breach was assessed as non-notifiable, on what basis?
4. What remediation and preventative measures have been put in place?

Please treat this as a formal request. If I do not receive a substantive response
within **10 business days**, I intend to refer the matter to the PDPC.

Sincerely,
[Your name]
[Contact details]

---

## Step 2 — Escalating to the PDPC (if no adequate response)

When you file via the PDPC e-service, have the following ready:

- **Your identity & contact** (Singpass login required for submission).
- **The organization's name** and any DPO contact you used.
- **What happened, factually:** the endpoint `GET /api/teams?eventId=...`, the date(s)
  you observed it, the categories of data returned (e.g. email addresses), and the
  approximate scale (≈144 teams).
- **Evidence:** the **redacted** screenshots from `evidence/03-data-exposure/`
  (structure only — do **not** submit files containing real personal data of others;
  describe it instead).
- **What you've done already:** your Step 1 letter to the DPO and the date sent, plus
  whether/how they responded.
- **What you're asking for:** an assessment of whether the organization met its
  Protection Obligation and breach-notification duties.

Keep a copy of everything you submit.

---

### A word on framing

Report **facts**, not characterizations. "The endpoint returned plaintext emails for
~144 teams on [date]" is a fact a regulator can act on. Avoid words like "fraud" or
"malicious" about any individual — they don't help your report and can complicate it.
Let the PDPC reach its own conclusions from the facts you provide.
