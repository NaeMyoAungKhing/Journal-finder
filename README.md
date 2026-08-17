# Journal Finder

A single-page, offline-capable tool to (1) match academic journals to a research topic and (2) check any journal's percentile / quartile — built over a SCImago Journal Rank (SJR) snapshot of ~18,000 journals across 27 subject areas.

**Live site:** `https://<your-username>.github.io/<repo-name>/`

## Features
- **Match journals to my research** — enter a title plus optional *means* (methods) and *ends* (aims); ranks journals by keyword + subject-category fit, filterable by subject area and quartile.
- **Check a journal's percentile** — type a journal name, or paste a paper's **DOI** (resolved live via the free Crossref API) to jump to its journal's ranking. Shows overall SJR percentile and per-subject-area percentiles.
- **Clickable links** to SCImago and Google Scholar for every journal.
- **Export** the match list or any single journal to Markdown (.md) or Word (.doc).

## How it works
Everything runs client-side in one `index.html` (data embedded). The only network call is the optional DOI lookup to Crossref.

## Data & caveats
Data derived from the open SJR-Journal-Ranking dataset (SCImago / Scopus), a single-year snapshot (~2020). Percentiles are computed from SJR scores; rankings shift each year, so treat figures as a guide, not an official current number.
