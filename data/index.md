---
layout: default
title: Data Downloads
permalink: /data/
---
# Data Downloads

<ul>
{% assign files = site.static_files 
  | where_exp: "f", "f.path contains '/data/'" 
  | where_exp: "f", "f.name != 'index.md'" %}
{% for f in files %}
  <li>
    {% if f.extname == ".dta" %}
      <a class="btn"
         href="https://github.com/OrganizationDesign/homepage/releases/download/v20260721/20260721_OD_Database_1993_2024.dta"
         download="20260721_OD_Database_1993_2024.dta"
         type="application/octet-stream">
         Stata (.dta)
      </a>
    {% elsif f.extname == ".xlsx" %}
      <a class="btn"
        href="https://github.com/OrganizationDesign/homepage/releases/download/v20260721/20260721_OD_Database_1993_2024b.xlsx"
        download="20260721_OD_Database_1993_2024b.xlsx"
         type="application/vnd.openxmlformats-officedocument.spreadsheetml.sheet">
         Excel (.xlsx)
      </a>
    {% else %}
      <a class="btn"
         href="{{ f.path | relative_url }}"
         download="{{ f.name }}">
         {{ f.name }}
      </a>
    {% endif %}
  </li>
{% endfor %}
</ul>
