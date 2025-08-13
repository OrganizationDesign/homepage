---
layout: default
title: Home
---

<div class="hero">
  <h1>Public Org-Structure Database</h1>
  <p>
    This prototype site hosts documentation and (optionally) public snapshots of a research database on senior management team structure. Use the downloads below or browse the navigation for the codebook, coverage, and methods.
  </p>
  <p>
    <a class="btn solid" href="{{ '/data/' | relative_url }}">Browse data</a>
  </p>
</div>

## About
We introduce a public, hand-collected organizational-structure database covering 521 S&P 500 firms (1993–2020) with 161,028 executive-firm-year observations across 11,658 firm-years. Executive lists were manually extracted from annual reports, 10-K filings, and DEF 14A proxy statements, then titles were categorized into six managerial role groups and twelve hierarchical levels using fine-tuned large language models. The data are linkable to standard sources via CUSIP, GVKEY, and ticker, enabling longitudinal and cross-industry research on top-management team composition and firm structure.

- Coverage: **1993–2020**, **521 firms**, **11,658 firm-years**, **161,028 executive-firm-year observations**  
- Identifiers: `GVKEY`, `CUSIP`, `ticker`  
- Sources: 10-K, DEF 14A (proxy statements), Annual Reports  
- Motivation: Public provision of a large hand-collected dataset on top-management team roles and hierarchy to enable organization-design/strategy research

## Downloads
- [CSV (master_SP500_TMT.csv)]({{ "/data/master_SP500_TMT.csv" | absolute_url }}){: .btn download="master_SP500_TMT.csv" type="text/csv" }
- [Stata (.dta)]({{ "/data/master_SP500_TMT.dta" | absolute_url }}){: .btn download="master_SP500_TMT.dta" }


## Quick preview
<div class="table-wrap">
  <table id="previewTable"></table>
</div>
<script>
document.addEventListener('DOMContentLoaded', function () {
  renderCSVTable('{{ "/data/snapshot.csv" | relative_url }}', 'previewTable');
});
</script>
