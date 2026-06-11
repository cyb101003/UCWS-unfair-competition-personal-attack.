# Setup — publishing this repository

## ✅ Pre-publish checklist (do this first)

Before the repo goes public, confirm **every** item:

- [ ] Every screenshot has all third-party personal data **blacked out** (emails,
      phone numbers, real names, handles, avatars, IPs, tokens).
- [ ] The `03-data-exposure` exhibits show **structure only** — no real email or
      personal value is visible, even partially.
- [ ] No raw data files (`.json`, `.csv`, `.har`, `.xlsx`) containing personal data
      are included. (The `.gitignore` blocks these in `evidence/` by default — keep it
      that way; convert proof to a redacted image instead.)
- [ ] Redactions are **flattened** (exported to PNG/JPG, not removable layers).
- [ ] `evidence/MANIFEST.md` lists each exhibit with a caption and date.
- [ ] You've re-read the [README](README.md) and are comfortable everything stated as
      fact is backed by an exhibit, and everything else is marked as opinion/question.

> Once something is pushed to a public repo, assume it is permanent (forks, caches,
> archives). The checklist exists because there is no reliable "undo."

## Option A — GitHub website (no command line)

1. Go to https://github.com/new and create a **new repository**.
   Suggested name: `ucws-singapore-2026-transparency` (rename as you like).
2. Set it to **Public**, then **Create repository**.
3. On the next page, click **uploading an existing file** and drag in the contents of
   this folder (including the `evidence/` and `complaints/` subfolders).
4. Commit. Your repo is live at `https://github.com/[you]/[repo]`.

## Option B — Command line (git)

From inside this folder:

```bash
git init
git add .
git commit -m "Initial documentation: rules, results, data-exposure, responses"
git branch -M main
git remote add origin https://github.com/[your-username]/ucws-singapore-2026-transparency.git
git push -u origin main
```

(Create the empty repo on GitHub first, or use the `gh` CLI: `gh repo create
ucws-singapore-2026-transparency --public --source=. --push`.)

## After publishing

- Put the repo link into the two letters in `complaints/`.
- Consider enabling **Issues** so organizers, the sponsor, or participants can post
  corrections or responses — visibly engaging with feedback strengthens your case.
- If you later send the PDPC report, you can note the date in `TIMELINE.md`.

## If you receive a correction or a credible objection

Act on it quickly: edit or retract the affected item and note the change. A repository
that visibly corrects itself is far more credible — and far more defensible — than one
that doesn't.
