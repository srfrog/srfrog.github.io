---
layout: page
title: Archive
permalink: /archive/
---

<ul class="post-list">
{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
{%- for post in site.posts -%}

  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}

  {%- if year != prev_year -%}
  <li>
    <h2 class="post-list-heading" style="margin-top:0;">{{ year }}</h2>
  </li>
  {%- endif -%}
  
  <li>
    <h3 style="margin:0;">
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h3>
    <span class="post-meta">{{ post.date | date: date_format }}</span>
  </li>  
  
  {% capture prev_year %}{{ year }}{% endcapture %}

{%- endfor -%}
</ul>
