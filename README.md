# Creator Deal Desk

A single-file tool for pricing creator and influencer partnerships on **CPM**, checking creator rate cards, modelling **ROI / ROAS** and planning the content calendar.

Built by an affiliate and partnership manager to replace a multi-tab Excel workbook with one calculator that covers every channel.

> **Demo build.** All creators, view counts, rates and conversion assumptions are sample data.

**[▶ Live demo](https://fabriziodemel-stack.github.io/creator-deal-desk/)**

---

## Why

Pricing creator deals usually means a spreadsheet per channel, manual averages skewed by one viral video, and no quick way to tell whether a rate card is fair. This tool answers three questions in seconds:

1. **What is this creator's real reach?** (clean average views, spikes removed)
2. **Is the price right?** (effective CPM against a ceiling, with a counter-offer)
3. **Will it pay back?** (funnel-based revenue, ROAS and ROI over 12 months)

## Features

| Tab | What it does |
|---|---|
| **Views** | Paste up to 30 recent view counts per channel. Viral spikes and inconsistent 1M+ videos are excluded automatically, and every exclusion is shown. |
| **Package & CPM** | Build a package from 10 content types (YouTube, Shorts, TikTok, Reels, Stories, blog). Get CPM, max budget at ceiling and a traffic-light verdict. Solve any one of views, CPM or budget from the other two. |
| **Rate card check** | Paste a creator's rate card or emailed proposal. Each item gets an effective CPM, a verdict (accept, negotiate, counter) and a counter price at your target CPM. |
| **ROI scenarios** | Funnel model: reach → engagement → site visits → sales → revenue → commission, by follower tier. Pessimistic, realistic and optimistic long-tail scenarios at 1, 3, 6 and 12 months. |
| **Calendar** | Spreads content across a 1 to 12 month collaboration, weighted by seasonality, minimum one item per month. Export as CSV or `.ics` for Google Calendar. |
| **Lead log** | Record every creator tested with CPM, outcome and notes. Export to CSV. |
| **Settings** | Ceiling CPM, good-deal threshold, spike filter rules, FX rates. |

**Every number shows its working.** Each result has a "Show working" panel with the full calculation, so figures can be explained to a manager or a creator.

## Pricing rules (defaults)

- CPM is always calculated in **EUR**; budgets and rate cards can be entered in EUR, AUD, USD or GBP
- **Ceiling CPM: €22**, good deal below €15
- Views above **3× the median** are treated as spikes
- **1M+ views** count only if at least **4 of the last 6** videos reached 1M+
- CPM = total budget / (average views × number of items) × 1000

All rules are editable in Settings.

## Run it

No build step, no dependencies, no backend.

```bash
git clone https://github.com/fabriziodemel-stack/creator-deal-desk.git
open creator-deal-desk/index.html
```

Or publish with **GitHub Pages**: Settings → Pages → Deploy from branch → `main` / root.

## Tech

Plain HTML, CSS and JavaScript in one file. Light and dark mode, mobile friendly. The lead log uses `localStorage` and never leaves the browser.

## Roadmap

- Screenshot upload with automatic view extraction (OCR)
- Push calendar and deal to a CRM (HubSpot)
- Renewal analysis from affiliate network performance exports
- Multi-user version with logins

## Author

**Fabrizio De Mel** · Senior Affiliate & Partnership Manager
[LinkedIn](https://it.linkedin.com/in/fabriziodemel) · fabrizio.demel@outlook.com

## License

MIT
