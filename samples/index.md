---
layout: default
title: Sample Files
permalink: /samples/
---

# Sample Files

<ul>
{% assign sample_files = site.static_files 
   | where_exp: "f", "f.path contains '/samples/'" 
   | where_exp: "f", "f.name != 'index.md'" %}
{% for f in sample_files %}
  <li><a href="{{ f.path | relative_url }}">{{ f.name }}</a></li>
{% endfor %}
</ul>
