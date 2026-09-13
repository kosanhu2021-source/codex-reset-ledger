# Codex Reset Ledger

Every OpenAI Codex rate-limit reset, logged and verifiable — with a source link for **every single event**.

- **55 verified resets** since September 2025, collected from official OpenAI / Codex team announcements on X
- **+3 policy notes** (limit policy changes that reshape your weekly usage)
- Website with live radar & email alerts: **https://whenresets.net**

## Why this dataset exists

Codex usage limits get reset for everyone far more often than most users notice — outage compensations, milestones, celebrations, billing-system rewrites. When your limits look mysteriously refreshed, there is usually a reason. This ledger records every reset that actually took effect, so you can check *when* your limits were refreshed and *why*.

## Counting rule (methodology)

**One row per reset that actually took effect.** Announcement posts and confirmation posts are **not** double-counted — if a reset was both announced and later confirmed, only the moment it took effect is logged. Every reset row carries a link to its official source.

## Files

| File | Contents |
|---|---|
| `data/codex-reset-ledger.csv` | Full ledger, oldest first — 58 rows (55 resets + 3 policy notes) |
| `data/codex-reset-ledger.json` | Same data as JSON, with `type_label` and dataset metadata |

**Columns:** `date_utc`, `time_utc`, `type`, `description`, `source_url`, `source_platform`

## Event types

| type | meaning | count |
|---|---|---|
| `incident` | Outage compensation | 15 |
| `other` | Reset | 11 |
| `launch` | Launch / new model | 9 |
| `banked` | Banked / carried over | 8 |
| `celebration` | Celebration / holiday | 6 |
| `milestone` | Milestone | 6 |
| `policy` | Limit-policy change (not a reset itself) | 3 |

> Note: 8 resets in total are tied to milestone announcements (6 tagged `milestone` + 2 tagged `other`) — that is the "milestone-tied" count used on the website.

## Key stats (as of 2026-09-13)

- 55 resets over 360 days → one every **6.7 days** on average
- Last 30 days: 12 resets → one every **2.5 days** (pace is accelerating)
- Most common reason: outage compensation (15 events)

## Updates

Manually verified and updated within ~24h of each new event. The live, always-current version is at **https://whenresets.net**.

## License & disclaimer

MIT License — see [LICENSE](LICENSE).

Unofficial, community-maintained dataset. Not affiliated with, endorsed by, or connected to OpenAI. All data comes from public sources; each row links to its origin.
