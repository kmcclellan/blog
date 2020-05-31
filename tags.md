---
layout: page
title: Tags
permalink: /tags
---
{%- for tag in site.tags -%}
  <div id="tag-{{tag[0]}}">
    {%- assign list-title = tag[0] -%}
    {%- assign list-posts = tag[1] -%}
    {% include post-list.html title=list-title posts=list-posts %}
  </div>
{%- endfor -%}
