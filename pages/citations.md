---
layout: default
title: Citations & Uses
permalink: /pages/citations
---

# Citations & Works Using This Database

- **Google Scholar tracking:**  
  Provisional link: <https://scholar.google.com/citations?view_op=view_citation&hl=en&user=55pBI1MAAAAJ&sortby=pubdate&citation_for_view=55pBI1MAAAAJ:zA6iFVUQeVQC>

> Scholar doesn’t provide an official free API for embedding the list here; we’ll update the list below periodically. (We also accept PRs adding new citations.)

## Curated list

<div class="table-wrap">
  <table id="citeTable"></table>
</div>

<script>
document.addEventListener('DOMContentLoaded', function () {
  renderCSVTable('{{ "/data/citations.csv" | relative_url }}', 'citeTable');
});
</script>
