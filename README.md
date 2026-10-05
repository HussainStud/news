# Kuwait Scholarship News Tracker | متتبع أخبار البعثات الكويتية

Daily monitoring of news and X (Twitter) posts about Kuwaiti students whose
government scholarships (البعثات) were revoked, frozen, or terminated.

Each daily report has: **Arabic news digest** → **English summary** → **what students are asking for / who they are contacting** → **who else can be contacted**.

## Layout
| Path | Purpose |
|---|---|
| `reports/YYYY-MM-DD.md` | One report per day |
| `data/sources.md` | News outlets, official accounts and X search queries to check |
| `data/contacts.md` | Directory of who to reach out to (verify before use) |
| `data/timeline.md` | Running timeline of events and decisions |
| `DAILY_PROMPT.md` | The exact instructions the daily routine follows |

## Daily routine
A scheduled Claude session follows `DAILY_PROMPT.md`, writes `reports/<date>.md`,
updates `data/timeline.md`, and pushes to this repo.

## Honest limits
- X posts are often not reachable by automated search/fetch. Anything from X that
  could not be opened is marked **unverified** and listed under "to check manually".
- Claims by individual students are reported as claims, not facts.
