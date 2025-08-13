---
layout: default
title: Coverage
permalink: /pages/coverage
---

# Coverage

## By Year
<div class="table-wrap">
  <table id="yearTable"></table>
</div>

## By Sector
<div class="table-wrap">
  <table id="sectorTable"></table>
</div>

<script>
document.addEventListener('DOMContentLoaded', function () {
  renderCSVTable('{{ "/data/coverage_by_year.csv" | relative_url }}', 'yearTable');
  renderCSVTable('{{ "/data/coverage_by_sector.csv" | relative_url }}', 'sectorTable');
});
</script>
