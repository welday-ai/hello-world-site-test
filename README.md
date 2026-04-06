# Welday Portfolio

This repository contains materials for the Welday portfolio project and related business review artifacts.

## Purpose

Provide a clear, central place for portfolio and business summary documents used in the Welday Enterprises review workflow.

## Links Dashboard

This repo now includes a browser viewer for structured datasets used in the portfolio review workflow.

- `index.html`: searchable viewer with file-type selector for `.json` and `.md` sources
- `data/links.json`: structured venture/app links dataset
- `data/portfolio_catalog.json`: structured business catalog (`name`, `description`, `url`, `icon`) sourced from the business summary

To run locally:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000/`.

Direct-view examples:

- `http://localhost:8000/?fileType=json&view=portfolio_catalog.json`
- `http://localhost:8000/?fileType=md&view=WEL-5_Business_Summary.md`
- `http://localhost:8000/#json` (base URL hash route for JSON mode)
- `http://localhost:8000/#md` (base URL hash route for Markdown mode)
