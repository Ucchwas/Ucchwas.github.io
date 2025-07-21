---
layout: single
title: Publications
permalink: /publications/
---

A selection of my peer‐reviewed publications:

<ul class="publication-list">
{%- for p in site.data.publications -%}
  <li>
    <p>
      **{{ p.title }}**  
      _{{ p.journal }}_  
      {% if p.authors %}— {{ p.authors }}{% endif %}
      {%- if p.url -%}
        • [PDF]({{ p.url }})
      {%- endif -%}
    </p>
  </li>
{%- endfor -%}
</ul>
