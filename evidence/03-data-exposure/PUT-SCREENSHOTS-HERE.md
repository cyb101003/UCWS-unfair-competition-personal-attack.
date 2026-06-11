# 03 · Data exposure · 数据暴露

⚠️ **Highest-sensitivity folder. Redact aggressively.**
⚠️ **最敏感的目录。请大力打码。**

The goal is to prove the endpoint **returned personal data** — not to show the data.
目的是证明该接口**返回了**个人数据——而非展示数据。

Put here (all personal values blacked out):
放这里（所有个人取值一律涂黑）：

1. The **request** — URL shape `GET /api/teams?eventId=...` (you may redact the real
   eventId). 请求——URL 形态 `GET /api/teams?eventId=...`（可对真实 eventId 打码）。
2. The **response structure** — field **names** (e.g. `email`, `name`, …) with every
   **value** blacked out. A few rows is enough to show the shape.
   响应结构——字段**名称**（如 `email`、`name` 等），所有**取值**涂黑。展示几行以说明结构即可。
3. Optional: a redacted note of **how many** records were returned (e.g. "144 teams"),
   without the records themselves. 可选：注明返回了**多少**条记录（如"144 支团队"），但不含记录本身。

**Do NOT** commit any file that contains a real email address or other real personal
value, even partially. If in doubt, leave it out.
**切勿**提交任何包含真实邮箱或其他真实个人取值的文件，哪怕只是部分。拿不准就不要放。

See the full policy in [../README.md](../README.md).
完整规范见 [../README.md](../README.md)。
