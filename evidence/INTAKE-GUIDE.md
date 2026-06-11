# Evidence intake & sorting guide · 证据收集与整理指南

A simple, safe workflow for turning raw screenshots into published exhibits.
一套简单、安全的流程，把原始截图变成可发布的证据。

```
        ┌─────────────┐   redact + rename   ┌──────────────────────┐   log
raw  →  │  _INBOX/     │  ───────────────→   │  01–04 (public)      │  ──→  MANIFEST.md
upload  │  (gitignored)│   打码 + 重命名      │  01–04（公开目录）   │       清单
        └─────────────┘                     └──────────────────────┘
```

## Step 1 — Drop raw files in `_INBOX/` · 把原始文件放进 `_INBOX/`

`_INBOX/` is **gitignored** — its contents are **never published**, so it is the safe
place to hold raw, unredacted screenshots while you work.
`_INBOX/` 已被 **gitignore** ——其内容**永不会被发布**，因此是你处理时暂存**未打码**原始截图的安全位置。

> In this chat you can simply **upload** your screenshots and ask me to sort them — I'll
> place them, propose names, and flag exactly what needs redacting before anything is
> published.
> 在本对话中，你也可以直接**上传**截图并让我整理——我会归位、建议命名，并明确指出发布前**必须打码**的内容。

## Step 2 — Decide which folder · 判断该放哪个目录

| If the screenshot shows… · 如果截图内容是…… | → Folder · 目录 |
|---|---|
| The official scoring rules / the 30% community-vote rule · 官方评分规则 / 社区投票 30% 规则 | `01-scoring-rules/` |
| The Top-20 list, vote counts, GitHub stars · Top 20 名单、票数、star 数 | `02-rankings/` |
| The `GET /api/teams?eventId=...` request/response (structure only) · 该接口的请求/响应（仅结构） | `03-data-exposure/` |
| Organizers' public messages (no breakdown / "1v1" / "scraping") · 主办方公开消息 | `04-organizer-responses/` |

## Step 3 — Redact, then rename · 先打码，再重命名

1. **Black out all third-party personal data** (emails, phone, real names, handles,
   avatars, IPs, tokens). For `03-data-exposure`, show **structure only** — no real
   values. **涂黑所有第三方个人数据**；`03-data-exposure` 只展示**结构**，不含真实取值。
2. **Flatten** the redaction (export to PNG/JPG so black boxes can't be removed).
   将打码**压平**（导出 PNG/JPG，使黑框不可还原）。
3. **Rename** with a dated, descriptive name, e.g.:
   用带日期的描述性名称**重命名**，例如：
   - `2026-06-01_official-rules_community-vote-30pct.png`
   - `2026-06-09_top20_no1-project-10votes-0stars.png`
   - `2026-06-05_api-teams_response-structure_REDACTED.png`
   - `2026-06-09_public-channel_no-breakdown.png`
4. **Move** it from `_INBOX/` into the right numbered folder.
   将其从 `_INBOX/` **移动**到对应编号目录。

## Step 4 — Log it · 登记

Add one row to [`MANIFEST.md`](MANIFEST.md): file, date, source, caption, redacted ✅.
在 [`MANIFEST.md`](MANIFEST.md) 增加一行：文件、日期、来源、说明、是否打码 ✅。

## Step 5 — Clear the inbox · 清空暂存区

When done, delete the raw originals from `_INBOX/`. (It's gitignored, but keeping raw
PII around longer than needed is best avoided.)
完成后，删除 `_INBOX/` 中的原始文件。（虽已 gitignore，但不必要地长期保留原始个人数据应尽量避免。）

---

**The one rule that matters most:** nothing leaves `_INBOX/` for a public folder until
its third-party personal data is redacted and flattened. When unsure, redact.
**最重要的一条：** 在第三方个人数据被打码并压平之前，任何文件都不得从 `_INBOX/` 进入公开目录。拿不准就打码。
