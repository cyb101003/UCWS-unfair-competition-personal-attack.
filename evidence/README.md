# Evidence Index · 证据索引

This folder holds the primary-source exhibits referenced in the
[README](../README.md). Read the redaction policy below **before** adding anything.

本目录存放 [README](../README.md) 中引用的原始证据。在添加任何文件**之前**，请先阅读下方的打码规范。

> **New to this? Start with the [Intake & Sorting Guide](INTAKE-GUIDE.md).** Drop raw
> screenshots in `_INBOX/` (gitignored), redact, then move them into the numbered
> folders below.
> **第一次用？请先看[证据收集与整理指南](INTAKE-GUIDE.md)。** 把原始截图放进 `_INBOX/`
> （已 gitignore），打码后再移入下方的编号目录。

---

## ⚠️ Redaction policy — read first · 打码规范——务必先读

**This is the single most important rule in the repository.**
**这是本仓库最重要的一条规则。**

1. **Never upload anyone's personal data.** Before adding any screenshot, black out
   (redact) every: email address, phone number, real name, student/employee ID,
   IP address, account handle that identifies a private individual, profile photo,
   and any auth token, cookie, API key, or session value.
   **绝不上传任何人的个人数据。** 添加任何截图前，请涂黑（打码）每一处：邮箱地址、电话号码、
   真实姓名、学号/工号、IP 地址、可识别到具体私人的账号昵称、头像，以及任何鉴权 token、
   cookie、API key 或 session 值。

2. **The data-exposure exhibit especially.** For `03-data-exposure`, the point is to
   show *that* the endpoint returned personal data — **not** the data itself. Show the
   request URL shape and the field **names/structure**, with every value blacked out.
   **Do not** paste the raw response body containing real emails. Redact the count of
   records, not the records.
   **数据暴露证据尤其如此。** 对 `03-data-exposure`，目的是证明该接口**返回了**个人数据，
   **而非**展示数据本身。只展示请求 URL 的形态与字段**名称/结构**，所有取值一律涂黑。
   **不要**粘贴包含真实邮箱的原始响应体。

3. **Flatten redactions.** Don't draw a black box in a layered editor and export a
   format that keeps layers — the box can be removed. Export to PNG/JPG, or
   screenshot the redacted image again, so the blackout is permanent.
   **打码要"压平"。** 不要在分层编辑器里画个黑框就导出可保留图层的格式（黑框可能被还原）。
   请导出为 PNG/JPG，或对打码后的图片再截一次图，确保涂黑不可逆。

4. **Strip metadata.** Screenshots can carry EXIF/location/device metadata. Re-saving
   as a fresh PNG generally removes it; verify if in doubt.
   **清除元数据。** 截图可能携带 EXIF/位置/设备信息。重新另存为 PNG 通常即可清除；不确定时请核对。

5. **The organizers' own public statements** may be shown without redacting the
   organizers, per the repository owner's decision — but **other participants in the
   same screenshot must still be redacted** (names, handles, avatars).
   **主办方自己的公开发言**可按仓库所有者的决定不为主办方打码——但**同一张截图中其他参赛者
   仍须打码**（姓名、昵称、头像）。

> If you are unsure whether something counts as personal data, redact it. There is no
> downside to over-redacting; there is real harm in under-redacting.
> 若不确定某项是否属于个人数据，就打码。多打码没有坏处；少打码会造成真实伤害。

---

## Folder map · 目录结构

| Folder | What goes here · 存放内容 | Referenced by · 对应关切 |
|---|---|---|
| `01-scoring-rules/` | Screenshots of the official "Three-Dimensional Scoring Mechanism," especially the **30% community-vote** rule. 官方"三维评分机制"截图，尤其是**社区投票 30%**的规则。 | Concern 1 |
| `02-rankings/` | The announced Top-20; the No. 1 project's public vote/star count; comparison projects with high votes/stars. 公布的 Top 20；第 1 名项目的公开票数/star 数；高票数/高 star 的对比项目。 | Concern 1 |
| `03-data-exposure/` | Evidence that `GET /api/teams?eventId=...` returned personal data — **structure only, all values redacted.** 证明 `GET /api/teams?eventId=...` 返回了个人数据——**仅结构，所有取值打码。** | Concern 2 |
| `04-organizer-responses/` | Organizers' public messages: refusal to publish breakdowns, request for "1v1 private calls," the "malicious scraping" remark. 主办方公开消息：拒绝公开明细、要求"1 对 1 私聊"、"恶意爬取"言论。 | Concerns 1–3 |

## Naming exhibits · 证据命名

Use descriptive, dated filenames so each exhibit is easy to cite, e.g.:
请使用带日期的描述性文件名，便于引用，例如：

```
01-scoring-rules/2026-06-01_official-rules_community-vote-30pct.png
02-rankings/2026-06-09_top20_no1-project-10votes-0stars.png
02-rankings/2026-06-09_project-wall_high-vote-comparison.png
03-data-exposure/2026-06-05_api-teams_response-structure_REDACTED.png
04-organizer-responses/2026-06-09_public-channel_no-breakdown.png
```

After adding exhibits, list them in `MANIFEST.md` (a template is provided) with a one-
line caption and the date/source for each, so the record is self-describing.
添加证据后，请在 `MANIFEST.md`（已提供模板）中为每件证据写一行说明并标注日期/来源，
使记录可自我说明。
