---
layout: page
---
<h2>Posts tagged with "{{ page.tag }}"</h2>
<ul>
  {% for post in site.tags[page.tag] %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date: "%b %-d, %Y" }})</li>
  {% endfor %}
</ul>
