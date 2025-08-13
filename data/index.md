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
  <li><a href="{{ f.path | relative_url }}">{{ f.name }}</a></li>
{% endfor %}
</ul>
