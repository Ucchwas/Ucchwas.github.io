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


<style>
body, p, li, h1, h2, h3, h4, h5, h6 {
  font-family: 'Times New Roman', Times, serif !important;
}
.sidebar, .author__content {
  filter: none !important;
  opacity: 1 !important;
  transition: none !important;
}
</style>