---
layout: single
title: Publications
permalink: /publications/
---

<ul class="collection-list">
{% for p in site.data.publications %}
<li>
  <strong>{{ p.title }}</strong>  
  {% if p.journal %}<em>{{ p.journal }}</em>{% endif %}  
  <small>{{ p.date }}</small>  
  {% if p.url %}[DOI]({{ p.url }}){% endif %}
</li>
{% endfor %}
</ul>
