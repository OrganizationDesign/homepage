---
layout: default
title: Contribute
permalink: /pages/contribute
---

# Contribute

We welcome corrections and improvements to the database and documentation.  
Before submitting, please review our [Terms & Disclaimer]({{ '/pages/terms' | relative_url }}) and license (data: CC BY-NC 4.0).

## 1) Report a data issue (fastest)
Open a GitHub **Issue** with this template:

**Subject:** Data correction — <Firm>, <Year>, <Field>

**Details**
- Firm (and GVKEY/ticker if known):
- Year (or filing date):
- Field/variable affected:
- Current value:
- Proposed fix:
- Evidence (link to SEC filing or annual report; page/URL):
- Notes (optional):

> Please include links (10-K/DEF 14A/Annual Report). Screenshots help.

[Open an Issue]({{ site.github.repository_url }}/issues/new)

## 2) Submit a pull request (advanced)
- Edit only the relevant rows in `/data/*.csv`. Keep:
  - **UTF-8**, **comma** separators, **unchanged headers**, one record per row.
  - No stray commas inside cells (use quotes if needed).
- If you change variables, update `data/codebook.csv`.
- If coverage totals change, update `data/coverage_by_year.csv` / `data/coverage_by_sector.csv`.
- Add a short note to `CHANGELOG.md` (new or updated).
- Open a PR describing exactly what you changed and why, with sources.

[Open a Pull Request]({{ site.github.repository_url }}/compare)

## 3) No GitHub? Use the form
Prefer a form? Submit a correction here:

- **Data correction form:** <add your Google Form link>
- **General feedback:** <email or form link>

## Review & acceptance
All submissions are reviewed for:
- Source documentation (SEC filings or annual reports)
- Consistency with labeling rules and codebook
- Reproducibility of the proposed change

We may edit for formatting or request more information.

## Acknowledgments
We’re grateful to community contributors. You can be listed here (optional) or in the repository contributors list.

<ul>
{% for c in site.github.contributors %}
  <li><a href="{{ c.html_url }}">{{ c.login }}</a></li>
{% endfor %}
</ul>
