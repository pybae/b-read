---
layout: default
title: Archive
---

# archive

<ul>
{% assign sorted_posts = site.posts | sort: 'date' | reverse %}
{% for post in sorted_posts %}
<li>
<span>{{- post.date | date: "%Y-%m-%d"-}}: </span>
<a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
