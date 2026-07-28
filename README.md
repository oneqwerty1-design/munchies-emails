# MUNCHIES! Campaign Emails

Visual mockups, copy, and send notes for one-off campaign sends.

**Live:** https://munchies-campaign-emails.vercel.app

## Files

| File | What it is |
|---|---|
| `index.html` | The whole page — one `.tab-panel` per email |
| `styles.css` | All styling. Per-email blocks are commented and prefixed |

## Emails currently in the deck

| Tab | Send | Type |
|---|---|---|
| Hall of Fame — Top 5 Reordered | one-time | Campaign |
| August Preview — What's Coming | Jul 31 (Fri) | Teaser |
| War On August — Dog Days Kickoff | Aug 4 (Tue) | Content |
| CBD Day — A Holiday You've Never Heard Of | Aug 6 (Thu) | Teaser |
| CBD Day Sale — The Balanced Ones | Aug 7 (Fri) | Sale, 20% off Fri–Sun |

## Adding an email

1. Add a `.tab-btn` inside `.tab-bar` with a new `data-tab="your-id"`
2. Add a matching `<div class="tab-panel" id="tab-your-id">` before the `<script>`
3. Add an active-state colour rule in `styles.css`:
   `.tab-btn[data-tab="your-id"].active { ... }`
4. Commit and push — Vercel deploys automatically

Tab id and panel id must match (`data-tab="x"` → `id="tab-x"`) or the switcher throws.

## Deploying

Push to `main`. Vercel builds and deploys on every commit — no build step, it's static.
