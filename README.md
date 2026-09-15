# Codex Reset Ledger

![GitHub stars](https://img.shields.io/github/stars/kosanhu2021-source/codex-reset-ledger?style=flat-square)
![License](https://img.shields.io/github/license/kosanhu2021-source/codex-reset-ledger?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/kosanhu2021-source/codex-reset-ledger?style=flat-square)

Every OpenAI Codex rate-limit reset, logged and verifiable — with a source link for **every single event**.

- **55 verified resets** since September 2025, collected from official OpenAI / Codex team announcements on X
- **+3 policy notes** (limit policy changes that reshape your weekly usage)
- Live radar, reset rules for 15 AI tools, and email alerts: **[whenresets.net](https://whenresets.net)**

## Why this dataset exists

Codex usage limits get reset for everyone far more often than most users notice — outage compensations, milestones, celebrations, billing-system rewrites. When your limits look mysteriously refreshed, there is usually a reason. This ledger records every reset that actually took effect, so you can check *when* your limits were refreshed and *why*.

## Who this is for

- **Tool builders** — any app that tells a user when their Codex quota refills needs this timeline as a data source.
- **Researchers and writers** — every row links to its primary source, so a claim can be verified instead of repeated.
- **Anyone who just got a mysterious reset** — look up the date, find out why it happened.

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

## Citing this dataset

> Codex Reset Ledger (2026). *Every OpenAI Codex rate-limit reset, logged and verifiable.* https://github.com/kosanhu2021-source/codex-reset-ledger

No registration or attribution required beyond the MIT license — a link back is appreciated.

## Updates

Manually verified and updated within ~24h of each new event. The live, always-current version — including reset rules for 15 other AI tools — is at **[whenresets.net](https://whenresets.net)**.

## License & disclaimer

MIT License — see [LICENSE](LICENSE).

Unofficial, community-maintained dataset. Not affiliated with, endorsed by, or connected to OpenAI. All data comes from public sources; each row links to its origin.
