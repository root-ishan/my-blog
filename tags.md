---
layout: page
title: "Tags"
permalink: /tags/
---

<h2>Browse by Tags</h2>
<ul>
  {% assign tags_list = site.tags %}
  {% for tag in tags_list %}
    <li><a href="/tags/{{ tag[0] | slugify }}/">{{ tag[0] }}</a> ({{ tag[1].size }})</li>
  {% endfor %}
</ul>
