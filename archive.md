---
layout: default
title: Archive
permalink: /archive
---

Below is the full archive of my articles/essays in chronological
order.


## Archive

{% assign sorted_posts = site.posts | sort: 'date'  %}
{% for post in sorted_posts %}
## [{{ post.title }}]({{ post.url | relative_url }})
{{ post.excerpt }}
<p style='text-align: right'>Published: {{ post.date | date: '%B %-d, %Y' }}</p>
{% endfor %}

----

{% include rss.md %}

----

{% include discuss.md %}
