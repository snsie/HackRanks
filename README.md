# HackRanks: IC3 Judging Desk

A judging site for the **IC3 AI Passport Showcase & Hackathon 2026** (Track A, November 17–18, 2026). It helps judges review and compare the 21 team submissions against the six-criterion judges' rubric.

**Live site: https://snsie.github.io/HackRanks/**

## What's on the site

| View | What it does |
| --- | --- |
| **Overview** | Sortable table of all 21 teams: validation accuracy, error counts, scores on each rubric criterion, totals, flags, and a download link for each team's deck. |
| **Team sheets** | Each team's summary, method, results, strengths, gaps and questions for the finalist round, next to a scoring sheet that follows the rubric (1–5 per criterion, comments, recusal box, live total out of 100). |
| **Compare** | Up to four teams side by side. |
| **Field analysis** | Validation-accuracy chart, a matrix of the techniques each team used, and patterns across the field. |
| **Rubric** | Criteria, level descriptors, tie-break rules and finalist-round weighting. |

## Submissions

All 21 original submissions are in [`submissions/`](submissions/). Download them one at a time from the site, or all at once as [`hackathon_presentations.zip`](submissions/hackathon_presentations.zip).

## Scoring

- **Draft scores** are suggestions from Claude, based only on the slide decks (no code, demos or hidden-test results). Turn them off with the **Draft scores** switch in the top bar to score blind.
- **Your scores** stay separate from the drafts. On this site they're saved in your browser only, so other judges can't see them, but they don't follow you to another device or browser.
- **Export my scores** downloads your scores as a CSV to return to the event coordinator.

## Running locally

The site is a single static `index.html` with no build step. Open it in a browser, or serve the folder:

```
python -m http.server 8000
```

Then open http://localhost:8000. Deck downloads need the `submissions/` folder next to `index.html`.
