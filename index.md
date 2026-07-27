---
layout: default
title: Home
---

<div class="hero">
  <h1>Public Org-Structure Database</h1>
  <p>
    This prototype site hosts documentation and (optionally) public snapshots of a research database on senior management team structure. Use the downloads below or browse the navigation for the complete documentation.
  </p>
  <p>
    <a class="btn solid" href="{{ '/data/' | relative_url }}">Browse data</a>
  </p>
</div>

## About
We introduce a public, hand-collected organizational-structure database covering 612 S&P 500 firms (1993–2024) with 216,018 executive-firm-year observations across 15,317 firm-years. Executive lists are compiled from annual SEC filings and company reports and standardized into comparable role categories over time.

- Coverage: **1993–2024**, **612 firms**, **15,317 firm-years**, **216,018 executive-firm-year observations**  
- Identifiers: `GVKEY`, `CUSIP`, `ticker`  
- Sources: 10-K, DEF 14A (proxy statements), Annual Reports  
- Motivation: Public provision of a large hand-collected dataset on top-management team roles and hierarchy to enable organization-design/strategy research

> *This database is freely available and provided for general informational, educational, and research purposes only.*

> *This database is provided “as is” and may contain errors. Errors naturally occur in the research process and, for this database, can come from sources such as:*
> 
> *• Incorrect manual entry of data*  
> *• Revisions of financial statements not captured in the database*  
> *• LLM models incorrectly coding roles into different categories*  
> 
> *We have endeavored to limit these errors but recognize the database is not error free.*

> *To the fullest extent permitted by law, the maintainers and contributors disclaim all warranties, whether expressed or implied (including but not limited to accuracy, completeness, merchantability, fitness for a particular purpose, and noninfringement), and shall not be liable for any direct, indirect, incidental, consequential, or special damages arising from use of the database.*

> *Public use or distribution of a substantial portion or derivative work from the database requires clear acknowledgment of **{{ site.ack_source | default: "XXXX" }}** as the source.*

The dataset is larger than the dataset used in the accompanying Strategic Management Journal paper as it includes three additional GICS sectors: Energy (10), Materials (15), and Real Estate (60).
You can read the accompanying paper here: [https://sms.onlinelibrary.wiley.com/doi/10.1002/smj.70029](https://sms.onlinelibrary.wiley.com/doi/10.1002/smj.70029)

## Downloads
- [CSV (20260721_OD_Database_1993_2024.csv)]({{ "/data/20260721_OD_Database_1993_2024.csv" | absolute_url }}){: .btn download="20260721_OD_Database_1993_2024.csv" type="text/csv" }
- [Stata (.dta)](https://raw.githubusercontent.com/OrganizationDesign/homepage/main/data/20260721_OD_Database_1993_2024.dta){: .btn download="20260721_OD_Database_1993_2024.dta" type="application/octet-stream" }

> **Note:** If downloading .csv file to Stata use `bindquote(strict)` option
  
**License:** Data are released under **CC BY-NC 4.0**.
See the [LICENSE]({{ '/LICENSE' | absolute_url }}) file and our
[Terms & Disclaimer]({{ '/pages/terms' | relative_url }}).




## Quick preview
<div class="table-wrap">
  <table id="previewTable"></table>
</div>
<script>
document.addEventListener('DOMContentLoaded', function () {
  renderCSVTable('{{ "/data/snapshot.csv" | relative_url }}', 'previewTable');
});
</script>
