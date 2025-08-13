---
layout: default
title: Codebook
permalink: /pages/codebook
---

# Codebook

<div class="table-wrap">
  <table id="codebookTable"></table>
</div>
<script>
document.addEventListener('DOMContentLoaded', function () {
  renderCSVTable('{{ "/data/codebook.csv" | relative_url }}', 'codebookTable');
});
</script>

