---
title: Blog
layout: default
---

# Blog

{% for post in site.posts %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>
	<em>{{ post.date | date: "%B %d, %Y" }}</em> -
	{{ post.excerpt | strip_html }} 
	<a href="{{ post.url }}">Read on ...</a>
</p>
{% endfor %}

<p class="menulike">Subscribe to our feed: {% include subscribe-to-feed-links.html %}</p>
