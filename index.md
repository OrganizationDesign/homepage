## Quick preview

<div class="table-wrap">
  <table id="previewTable"></table>
</div>

<script>
document.addEventListener('DOMContentLoaded', function () {
  renderCSVTable('{{ "/data/snapshot.csv" | relative_url }}', 'previewTable');
});
</script>
