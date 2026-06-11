# Evidence Manifest · 证据清单

Fill in one row per exhibit after you add it. Keep it accurate — this table is how
readers (and, if needed, the sponsor or a regulator) navigate the evidence.

每添加一件证据，就在下表补一行。请保持准确——读者（以及必要时的赞助方或监管机构）将依此查阅证据。

| # | File · 文件 | Date captured · 截取日期 | Source · 来源 | Caption · 说明 | Redacted? · 已打码？ |
|---|---|---|---|---|---|
| 1 | `01-scoring-rules/...` | YYYY-MM-DD | e.g. official site / official chat | Official rules showing community vote = 30% | ✅ / N/A |
| 2 | `02-rankings/...` | YYYY-MM-DD | public project wall | Top-20: No. 1 project shows ~10 votes, 0 stars | ✅ |
| 3 | `02-rankings/...` | YYYY-MM-DD | public project wall | Comparison project: 2,000+ stars, hundreds of votes | ✅ |
| 4 | `03-data-exposure/...` | YYYY-MM-DD | `GET /api/teams?eventId=...` | Response **structure** only; all personal values blacked out | ✅ (required) |
| 5 | `04-organizer-responses/...` | YYYY-MM-DD | official public channel | Organizer declines to publish score breakdown | ✅ |
| 6 | `04-organizer-responses/...` | YYYY-MM-DD | official public channel | "1v1 private calls" request | ✅ |
| 7 | `04-organizer-responses/...` | YYYY-MM-DD | official public channel | "malicious scraping" remark | ✅ |

**Reminder · 提醒:** every row marked ✅ must have *all* third-party personal data
removed before the file is committed. 每一行标记 ✅ 的证据，提交前必须移除*所有*第三方个人数据。
