---
layout: single
title: Projects
permalink: /projects/
---

Here are some of my key research & software projects:

<ul class="project-list">
{%- for proj in site.data.projects -%}
  <li>
    <h3><a href="{{ proj.url }}">{{ proj.title }}</a></h3>
    <p>{{ proj.description }}</p>
    {%- if proj.tags -%}
      <p>
        {%- for tag in proj.tags -%}
          <span class="tag">{{ tag }}</span>
        {%- endfor -%}
      </p>
    {%- endif -%}
  </li>
{%- endfor -%}
</ul>
