---
layout: default
---

# GitHub Blog Entries

{% for post in site.posts %}

{{ post.date | date: "%-d %B %Y" }} [{{ post.title }}]({{ post.url }}) - {{ post.excerpt | strip_html | truncatewords: 50 }}

{% endfor %}

# Random test

Testing pages...test..@
